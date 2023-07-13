# Comparing `tmp/jupyterlab_quarto-0.2.7.tar.gz` & `tmp/jupyterlab_quarto-0.2.8.tar.gz`

## Comparing `jupyterlab_quarto-0.2.7.tar` & `jupyterlab_quarto-0.2.8.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.copier-answers.yml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.yarnrc.yml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/CHANGELOG.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jest.config.js
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/setup.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/tsconfig.test.json
--rw-r--r--   0        0        0   414691 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/yarn.lock
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/_version.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/package.json
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js
--rw-r--r--   0        0        0   854820 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js.LICENSE.txt
--rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js
--rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js
--rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js
--rw-r--r--   0        0        0  1402360 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js
--rw-r--r--   0        0        0    42379 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js.LICENSE.txt
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js
--rw-r--r--   0        0        0   456694 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js.LICENSE.txt
--rw-r--r--   0        0        0    28859 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js
--rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js
--rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/remoteEntry.110f607f4dd53733e5a3.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/style.js
--rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/const.ts
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/index.ts
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/manager.ts
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/types.ts
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/widgets.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-deflist.d.ts
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-footnote.d.ts
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-gridtables.d.ts
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-implicit-figures.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-sub.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-sup.d.ts
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-task-lists.d.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/__tests__/jupyterlab-quarto.spec.ts
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/ast/ast.ts
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/hooks/codemirror.ts
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/callouts.ts
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/cites.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/decorator.ts
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/divs.ts
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/figure-divs.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/figures.ts
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/index.ts
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/math.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/shortcodes.ts
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/spans.ts
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/table-captions.ts
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/yaml.ts
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/index.ts
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetCells.ts
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/EmitTable.ts
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetLine.ts
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTable.ts
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/IState.ts
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/rules/gridtable.ts
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/mermaid/index.ts
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/utils/html.ts
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/utils/markdownit.ts
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/utils/tok.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/attrs.ts
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/callouts.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/cites.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/decorator.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/deflist.ts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/divs.ts
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/figure-divs.ts
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/figures.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/footnotes.ts
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/gridtables.ts
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/math.ts
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/mermaid.ts
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/provider.ts
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/shortcodes.ts
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/spans.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/sub.ts
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/sup.ts
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/table-captions.ts
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/tasklists.ts
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/yaml.ts
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/yarn.lock
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/tests/jupyterlab-quarto.spec.ts
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/LICENSE
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/README.md
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/.copier-answers.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/.yarnrc.yml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jest.config.js
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/tsconfig.test.json
+-rw-r--r--   0        0        0   414691 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/yarn.lock
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/_version.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/package.json
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js
+-rw-r--r--   0        0        0   854820 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js.LICENSE.txt
+-rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js
+-rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js
+-rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js
+-rw-r--r--   0        0        0  1402360 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js
+-rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/573.c159bf4028ff12850190.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/573.c159bf4028ff12850190.js.LICENSE.txt
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js
+-rw-r--r--   0        0        0   456694 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js.LICENSE.txt
+-rw-r--r--   0        0        0    29145 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/923.1e1a92e9bcd196793c79.js
+-rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js
+-rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/remoteEntry.7156007e7b025a17b2e3.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/style.js
+-rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/const.ts
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/index.ts
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/manager.ts
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/types.ts
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/widgets.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/@types/markdown-it-deflist.d.ts
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/@types/markdown-it-footnote.d.ts
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/@types/markdown-it-gridtables.d.ts
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/@types/markdown-it-implicit-figures.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/@types/markdown-it-sub.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/@types/markdown-it-sup.d.ts
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/@types/markdown-it-task-lists.d.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/__tests__/jupyterlab-quarto.spec.ts
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/ast/ast.ts
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/hooks/codemirror.ts
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/callouts.ts
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/cites.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/decorator.ts
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/divs.ts
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/figure-divs.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/figures.ts
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/index.ts
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/math.ts
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/shortcodes.ts
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/spans.ts
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/table-captions.ts
+-rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/yaml.ts
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/index.ts
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/gridtables/GetCells.ts
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/EmitTable.ts
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/GetLine.ts
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/ParseTable.ts
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/interfaces/markdown-it/IState.ts
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/gridtables/rules/gridtable.ts
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/mermaid/index.ts
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/utils/html.ts
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/utils/markdownit.ts
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/plugins/utils/tok.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/attrs.ts
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/callouts.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/cites.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/decorator.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/deflist.ts
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/divs.ts
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/figure-divs.ts
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/figures.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/footnotes.ts
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/gridtables.ts
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/math.ts
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/mermaid.ts
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/provider.ts
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/shortcodes.ts
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/spans.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/sub.ts
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/sup.ts
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/table-captions.ts
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/tasklists.ts
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/src/providers/yaml.ts
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/ui-tests/tests/jupyterlab-quarto.spec.ts
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/README.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.8/PKG-INFO
```

### Comparing `jupyterlab_quarto-0.2.7/.copier-answers.yml` & `jupyterlab_quarto-0.2.8/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/RELEASE.md` & `jupyterlab_quarto-0.2.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jest.config.js` & `jupyterlab_quarto-0.2.8/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/package.json` & `jupyterlab_quarto-0.2.8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.8'"}*

```diff
@@ -183,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.7"
+    "version": "0.2.8"
 }
```

### Comparing `jupyterlab_quarto-0.2.7/tsconfig.json` & `jupyterlab_quarto-0.2.8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/yarn.lock` & `jupyterlab_quarto-0.2.8/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/__init__.py` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/package.json` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7156007e7b025a17b2e3.js'}}",*

 * * "'version'": "'0.2.8'"}*

```diff
@@ -109,15 +109,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/quarto-dev/jupyterlab-quarto",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.110f607f4dd53733e5a3.js",
+            "load": "static/remoteEntry.7156007e7b025a17b2e3.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-myst:plugin",
             "jupyterlab-myst:legacyPlugin",
             "jupyterlab-myst:executor"
         ],
@@ -188,9 +188,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.7"
+    "version": "0.2.8"
 }
```

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/573.c159bf4028ff12850190.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,219 +1,218 @@
-/*! For license information please see 573.79885c9e9fcb552239cd.js.LICENSE.txt */
+/*! For license information please see 573.c159bf4028ff12850190.js.LICENSE.txt */
 "use strict";
 (self.webpackChunkjupyterlab_quarto = self.webpackChunkjupyterlab_quarto || []).push([
     [573], {
-        3645: e => {
-            e.exports = function(e) {
-                var t = [];
-                return t.toString = function() {
-                    return this.map((function(t) {
+        3645: t => {
+            t.exports = function(t) {
+                var e = [];
+                return e.toString = function() {
+                    return this.map((function(e) {
                         var n = "",
-                            i = void 0 !== t[5];
-                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), i && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), i && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
+                            i = void 0 !== e[5];
+                        return e[4] && (n += "@supports (".concat(e[4], ") {")), e[2] && (n += "@media ".concat(e[2], " {")), i && (n += "@layer".concat(e[5].length > 0 ? " ".concat(e[5]) : "", " {")), n += t(e), i && (n += "}"), e[2] && (n += "}"), e[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, n, i, r, o) {
-                    "string" == typeof e && (e = [
-                        [null, e, void 0]
+                }, e.i = function(t, n, i, r, o) {
+                    "string" == typeof t && (t = [
+                        [null, t, void 0]
                     ]);
                     var a = {};
                     if (i)
-                        for (var l = 0; l < this.length; l++) {
-                            var c = this[l][0];
-                            null != c && (a[c] = !0)
-                        }
-                    for (var s = 0; s < e.length; s++) {
-                        var u = [].concat(e[s]);
-                        i && a[u[0]] || (void 0 !== o && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = o), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), r && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = r) : u[4] = "".concat(r)), t.push(u))
+                        for (var c = 0; c < this.length; c++) {
+                            var l = this[c][0];
+                            null != l && (a[l] = !0)
+                        }
+                    for (var s = 0; s < t.length; s++) {
+                        var u = [].concat(t[s]);
+                        i && a[u[0]] || (void 0 !== o && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = o), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), r && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = r) : u[4] = "".concat(r)), e.push(u))
                     }
-                }, t
+                }, e
             }
         },
-        1667: e => {
-            e.exports = function(e, t) {
-                return t || (t = {}), e ? (e = String(e.__esModule ? e.default : e), /^['"].*['"]$/.test(e) && (e = e.slice(1, -1)), t.hash && (e += t.hash), /["'() \t\n]|(%20)/.test(e) || t.needQuotes ? '"'.concat(e.replace(/"/g, '\\"').replace(/\n/g, "\\n"), '"') : e) : e
+        1667: t => {
+            t.exports = function(t, e) {
+                return e || (e = {}), t ? (t = String(t.__esModule ? t.default : t), /^['"].*['"]$/.test(t) && (t = t.slice(1, -1)), e.hash && (t += e.hash), /["'() \t\n]|(%20)/.test(t) || e.needQuotes ? '"'.concat(t.replace(/"/g, '\\"').replace(/\n/g, "\\n"), '"') : t) : t
             }
         },
-        8081: e => {
-            e.exports = function(e) {
-                return e[1]
+        8081: t => {
+            t.exports = function(t) {
+                return t[1]
             }
         },
-        7180: (e, t, n) => {
-            function i(e) {
-                return null == e
-            }
-            n.d(t, {
-                $w: () => Lt,
-                bI: () => Ft,
-                zD: () => Mt
+        7180: (t, e, n) => {
+            function i(t) {
+                return null == t
+            }
+            n.d(e, {
+                bI: () => Nt,
+                zD: () => Et
             });
             var r = {
                 isNothing: i,
-                isObject: function(e) {
-                    return "object" == typeof e && null !== e
+                isObject: function(t) {
+                    return "object" == typeof t && null !== t
                 },
-                toArray: function(e) {
-                    return Array.isArray(e) ? e : i(e) ? [] : [e]
+                toArray: function(t) {
+                    return Array.isArray(t) ? t : i(t) ? [] : [t]
                 },
-                repeat: function(e, t) {
+                repeat: function(t, e) {
                     var n, i = "";
-                    for (n = 0; n < t; n += 1) i += e;
+                    for (n = 0; n < e; n += 1) i += t;
                     return i
                 },
-                isNegativeZero: function(e) {
-                    return 0 === e && Number.NEGATIVE_INFINITY === 1 / e
+                isNegativeZero: function(t) {
+                    return 0 === t && Number.NEGATIVE_INFINITY === 1 / t
                 },
-                extend: function(e, t) {
+                extend: function(t, e) {
                     var n, i, r, o;
-                    if (t)
-                        for (n = 0, i = (o = Object.keys(t)).length; n < i; n += 1) e[r = o[n]] = t[r];
-                    return e
+                    if (e)
+                        for (n = 0, i = (o = Object.keys(e)).length; n < i; n += 1) t[r = o[n]] = e[r];
+                    return t
                 }
             };
 
-            function o(e, t) {
+            function o(t, e) {
                 var n = "",
-                    i = e.reason || "(unknown reason)";
-                return e.mark ? (e.mark.name && (n += 'in "' + e.mark.name + '" '), n += "(" + (e.mark.line + 1) + ":" + (e.mark.column + 1) + ")", !t && e.mark.snippet && (n += "\n\n" + e.mark.snippet), i + " " + n) : i
+                    i = t.reason || "(unknown reason)";
+                return t.mark ? (t.mark.name && (n += 'in "' + t.mark.name + '" '), n += "(" + (t.mark.line + 1) + ":" + (t.mark.column + 1) + ")", !e && t.mark.snippet && (n += "\n\n" + t.mark.snippet), i + " " + n) : i
             }
 
-            function a(e, t) {
-                Error.call(this), this.name = "YAMLException", this.reason = e, this.mark = t, this.message = o(this, !1), Error.captureStackTrace ? Error.captureStackTrace(this, this.constructor) : this.stack = (new Error).stack || ""
+            function a(t, e) {
+                Error.call(this), this.name = "YAMLException", this.reason = t, this.mark = e, this.message = o(this, !1), Error.captureStackTrace ? Error.captureStackTrace(this, this.constructor) : this.stack = (new Error).stack || ""
             }
-            a.prototype = Object.create(Error.prototype), a.prototype.constructor = a, a.prototype.toString = function(e) {
-                return this.name + ": " + o(this, e)
+            a.prototype = Object.create(Error.prototype), a.prototype.constructor = a, a.prototype.toString = function(t) {
+                return this.name + ": " + o(this, t)
             };
-            var l = a;
+            var c = a;
 
-            function c(e, t, n, i, r) {
+            function l(t, e, n, i, r) {
                 var o = "",
                     a = "",
-                    l = Math.floor(r / 2) - 1;
-                return i - t > l && (t = i - l + (o = " ... ").length), n - i > l && (n = i + l - (a = " ...").length), {
-                    str: o + e.slice(t, n).replace(/\t/g, "→") + a,
-                    pos: i - t + o.length
+                    c = Math.floor(r / 2) - 1;
+                return i - e > c && (e = i - c + (o = " ... ").length), n - i > c && (n = i + c - (a = " ...").length), {
+                    str: o + t.slice(e, n).replace(/\t/g, "→") + a,
+                    pos: i - e + o.length
                 }
             }
 
-            function s(e, t) {
-                return r.repeat(" ", t - e.length) + e
+            function s(t, e) {
+                return r.repeat(" ", e - t.length) + t
             }
-            var u = function(e, t) {
-                    if (t = Object.create(t || null), !e.buffer) return null;
-                    t.maxLength || (t.maxLength = 79), "number" != typeof t.indent && (t.indent = 1), "number" != typeof t.linesBefore && (t.linesBefore = 3), "number" != typeof t.linesAfter && (t.linesAfter = 2);
-                    for (var n, i = /\r?\n|\r|\0/g, o = [0], a = [], l = -1; n = i.exec(e.buffer);) a.push(n.index), o.push(n.index + n[0].length), e.position <= n.index && l < 0 && (l = o.length - 2);
-                    l < 0 && (l = o.length - 1);
+            var u = function(t, e) {
+                    if (e = Object.create(e || null), !t.buffer) return null;
+                    e.maxLength || (e.maxLength = 79), "number" != typeof e.indent && (e.indent = 1), "number" != typeof e.linesBefore && (e.linesBefore = 3), "number" != typeof e.linesAfter && (e.linesAfter = 2);
+                    for (var n, i = /\r?\n|\r|\0/g, o = [0], a = [], c = -1; n = i.exec(t.buffer);) a.push(n.index), o.push(n.index + n[0].length), t.position <= n.index && c < 0 && (c = o.length - 2);
+                    c < 0 && (c = o.length - 1);
                     var u, p, f = "",
-                        d = Math.min(e.line + t.linesAfter, a.length).toString().length,
-                        h = t.maxLength - (t.indent + d + 3);
-                    for (u = 1; u <= t.linesBefore && !(l - u < 0); u++) p = c(e.buffer, o[l - u], a[l - u], e.position - (o[l] - o[l - u]), h), f = r.repeat(" ", t.indent) + s((e.line - u + 1).toString(), d) + " | " + p.str + "\n" + f;
-                    for (p = c(e.buffer, o[l], a[l], e.position, h), f += r.repeat(" ", t.indent) + s((e.line + 1).toString(), d) + " | " + p.str + "\n", f += r.repeat("-", t.indent + d + 3 + p.pos) + "^\n", u = 1; u <= t.linesAfter && !(l + u >= a.length); u++) p = c(e.buffer, o[l + u], a[l + u], e.position - (o[l] - o[l + u]), h), f += r.repeat(" ", t.indent) + s((e.line + u + 1).toString(), d) + " | " + p.str + "\n";
+                        d = Math.min(t.line + e.linesAfter, a.length).toString().length,
+                        h = e.maxLength - (e.indent + d + 3);
+                    for (u = 1; u <= e.linesBefore && !(c - u < 0); u++) p = l(t.buffer, o[c - u], a[c - u], t.position - (o[c] - o[c - u]), h), f = r.repeat(" ", e.indent) + s((t.line - u + 1).toString(), d) + " | " + p.str + "\n" + f;
+                    for (p = l(t.buffer, o[c], a[c], t.position, h), f += r.repeat(" ", e.indent) + s((t.line + 1).toString(), d) + " | " + p.str + "\n", f += r.repeat("-", e.indent + d + 3 + p.pos) + "^\n", u = 1; u <= e.linesAfter && !(c + u >= a.length); u++) p = l(t.buffer, o[c + u], a[c + u], t.position - (o[c] - o[c + u]), h), f += r.repeat(" ", e.indent) + s((t.line + u + 1).toString(), d) + " | " + p.str + "\n";
                     return f.replace(/\n$/, "")
                 },
                 p = ["kind", "multi", "resolve", "construct", "instanceOf", "predicate", "represent", "representName", "defaultStyle", "styleAliases"],
                 f = ["scalar", "sequence", "mapping"],
-                d = function(e, t) {
-                    if (t = t || {}, Object.keys(t).forEach((function(t) {
-                            if (-1 === p.indexOf(t)) throw new l('Unknown option "' + t + '" is met in definition of "' + e + '" YAML type.')
-                        })), this.options = t, this.tag = e, this.kind = t.kind || null, this.resolve = t.resolve || function() {
+                d = function(t, e) {
+                    if (e = e || {}, Object.keys(e).forEach((function(e) {
+                            if (-1 === p.indexOf(e)) throw new c('Unknown option "' + e + '" is met in definition of "' + t + '" YAML type.')
+                        })), this.options = e, this.tag = t, this.kind = e.kind || null, this.resolve = e.resolve || function() {
                             return !0
-                        }, this.construct = t.construct || function(e) {
-                            return e
-                        }, this.instanceOf = t.instanceOf || null, this.predicate = t.predicate || null, this.represent = t.represent || null, this.representName = t.representName || null, this.defaultStyle = t.defaultStyle || null, this.multi = t.multi || !1, this.styleAliases = function(e) {
-                            var t = {};
-                            return null !== e && Object.keys(e).forEach((function(n) {
-                                e[n].forEach((function(e) {
-                                    t[String(e)] = n
+                        }, this.construct = e.construct || function(t) {
+                            return t
+                        }, this.instanceOf = e.instanceOf || null, this.predicate = e.predicate || null, this.represent = e.represent || null, this.representName = e.representName || null, this.defaultStyle = e.defaultStyle || null, this.multi = e.multi || !1, this.styleAliases = function(t) {
+                            var e = {};
+                            return null !== t && Object.keys(t).forEach((function(n) {
+                                t[n].forEach((function(t) {
+                                    e[String(t)] = n
                                 }))
-                            })), t
-                        }(t.styleAliases || null), -1 === f.indexOf(this.kind)) throw new l('Unknown kind "' + this.kind + '" is specified for "' + e + '" YAML type.')
+                            })), e
+                        }(e.styleAliases || null), -1 === f.indexOf(this.kind)) throw new c('Unknown kind "' + this.kind + '" is specified for "' + t + '" YAML type.')
                 };
 
-            function h(e, t) {
+            function h(t, e) {
                 var n = [];
-                return e[t].forEach((function(e) {
-                    var t = n.length;
+                return t[e].forEach((function(t) {
+                    var e = n.length;
                     n.forEach((function(n, i) {
-                        n.tag === e.tag && n.kind === e.kind && n.multi === e.multi && (t = i)
-                    })), n[t] = e
+                        n.tag === t.tag && n.kind === t.kind && n.multi === t.multi && (e = i)
+                    })), n[e] = t
                 })), n
             }
 
-            function g(e) {
-                return this.extend(e)
+            function g(t) {
+                return this.extend(t)
             }
-            g.prototype.extend = function(e) {
-                var t = [],
+            g.prototype.extend = function(t) {
+                var e = [],
                     n = [];
-                if (e instanceof d) n.push(e);
-                else if (Array.isArray(e)) n = n.concat(e);
+                if (t instanceof d) n.push(t);
+                else if (Array.isArray(t)) n = n.concat(t);
                 else {
-                    if (!e || !Array.isArray(e.implicit) && !Array.isArray(e.explicit)) throw new l("Schema.extend argument should be a Type, [ Type ], or a schema definition ({ implicit: [...], explicit: [...] })");
-                    e.implicit && (t = t.concat(e.implicit)), e.explicit && (n = n.concat(e.explicit))
+                    if (!t || !Array.isArray(t.implicit) && !Array.isArray(t.explicit)) throw new c("Schema.extend argument should be a Type, [ Type ], or a schema definition ({ implicit: [...], explicit: [...] })");
+                    t.implicit && (e = e.concat(t.implicit)), t.explicit && (n = n.concat(t.explicit))
                 }
-                t.forEach((function(e) {
-                    if (!(e instanceof d)) throw new l("Specified list of YAML types (or a single Type object) contains a non-Type object.");
-                    if (e.loadKind && "scalar" !== e.loadKind) throw new l("There is a non-scalar type in the implicit list of a schema. Implicit resolving of such types is not supported.");
-                    if (e.multi) throw new l("There is a multi type in the implicit list of a schema. Multi tags can only be listed as explicit.")
-                })), n.forEach((function(e) {
-                    if (!(e instanceof d)) throw new l("Specified list of YAML types (or a single Type object) contains a non-Type object.")
+                e.forEach((function(t) {
+                    if (!(t instanceof d)) throw new c("Specified list of YAML types (or a single Type object) contains a non-Type object.");
+                    if (t.loadKind && "scalar" !== t.loadKind) throw new c("There is a non-scalar type in the implicit list of a schema. Implicit resolving of such types is not supported.");
+                    if (t.multi) throw new c("There is a multi type in the implicit list of a schema. Multi tags can only be listed as explicit.")
+                })), n.forEach((function(t) {
+                    if (!(t instanceof d)) throw new c("Specified list of YAML types (or a single Type object) contains a non-Type object.")
                 }));
                 var i = Object.create(g.prototype);
-                return i.implicit = (this.implicit || []).concat(t), i.explicit = (this.explicit || []).concat(n), i.compiledImplicit = h(i, "implicit"), i.compiledExplicit = h(i, "explicit"), i.compiledTypeMap = function() {
-                    var e, t, n = {
+                return i.implicit = (this.implicit || []).concat(e), i.explicit = (this.explicit || []).concat(n), i.compiledImplicit = h(i, "implicit"), i.compiledExplicit = h(i, "explicit"), i.compiledTypeMap = function() {
+                    var t, e, n = {
                         scalar: {},
                         sequence: {},
                         mapping: {},
                         fallback: {},
                         multi: {
                             scalar: [],
                             sequence: [],
                             mapping: [],
                             fallback: []
                         }
                     };
 
-                    function i(e) {
-                        e.multi ? (n.multi[e.kind].push(e), n.multi.fallback.push(e)) : n[e.kind][e.tag] = n.fallback[e.tag] = e
+                    function i(t) {
+                        t.multi ? (n.multi[t.kind].push(t), n.multi.fallback.push(t)) : n[t.kind][t.tag] = n.fallback[t.tag] = t
                     }
-                    for (e = 0, t = arguments.length; e < t; e += 1) arguments[e].forEach(i);
+                    for (t = 0, e = arguments.length; t < e; t += 1) arguments[t].forEach(i);
                     return n
                 }(i.compiledImplicit, i.compiledExplicit), i
             };
             var m = new g({
                     explicit: [new d("tag:yaml.org,2002:str", {
                         kind: "scalar",
-                        construct: function(e) {
-                            return null !== e ? e : ""
+                        construct: function(t) {
+                            return null !== t ? t : ""
                         }
                     }), new d("tag:yaml.org,2002:seq", {
                         kind: "sequence",
-                        construct: function(e) {
-                            return null !== e ? e : []
+                        construct: function(t) {
+                            return null !== t ? t : []
                         }
                     }), new d("tag:yaml.org,2002:map", {
                         kind: "mapping",
-                        construct: function(e) {
-                            return null !== e ? e : {}
+                        construct: function(t) {
+                            return null !== t ? t : {}
                         }
                     })]
                 }),
                 y = new d("tag:yaml.org,2002:null", {
                     kind: "scalar",
-                    resolve: function(e) {
-                        if (null === e) return !0;
-                        var t = e.length;
-                        return 1 === t && "~" === e || 4 === t && ("null" === e || "Null" === e || "NULL" === e)
+                    resolve: function(t) {
+                        if (null === t) return !0;
+                        var e = t.length;
+                        return 1 === e && "~" === t || 4 === e && ("null" === t || "Null" === t || "NULL" === t)
                     },
                     construct: function() {
                         return null
                     },
-                    predicate: function(e) {
-                        return null === e
+                    predicate: function(t) {
+                        return null === t
                     },
                     represent: {
                         canonical: function() {
                             return "~"
                         },
                         lowercase: function() {
                             return "null"
@@ -228,1098 +227,820 @@
                             return ""
                         }
                     },
                     defaultStyle: "lowercase"
                 }),
                 b = new d("tag:yaml.org,2002:bool", {
                     kind: "scalar",
-                    resolve: function(e) {
-                        if (null === e) return !1;
-                        var t = e.length;
-                        return 4 === t && ("true" === e || "True" === e || "TRUE" === e) || 5 === t && ("false" === e || "False" === e || "FALSE" === e)
+                    resolve: function(t) {
+                        if (null === t) return !1;
+                        var e = t.length;
+                        return 4 === e && ("true" === t || "True" === t || "TRUE" === t) || 5 === e && ("false" === t || "False" === t || "FALSE" === t)
                     },
-                    construct: function(e) {
-                        return "true" === e || "True" === e || "TRUE" === e
+                    construct: function(t) {
+                        return "true" === t || "True" === t || "TRUE" === t
                     },
-                    predicate: function(e) {
-                        return "[object Boolean]" === Object.prototype.toString.call(e)
+                    predicate: function(t) {
+                        return "[object Boolean]" === Object.prototype.toString.call(t)
                     },
                     represent: {
-                        lowercase: function(e) {
-                            return e ? "true" : "false"
+                        lowercase: function(t) {
+                            return t ? "true" : "false"
                         },
-                        uppercase: function(e) {
-                            return e ? "TRUE" : "FALSE"
+                        uppercase: function(t) {
+                            return t ? "TRUE" : "FALSE"
                         },
-                        camelcase: function(e) {
-                            return e ? "True" : "False"
+                        camelcase: function(t) {
+                            return t ? "True" : "False"
                         }
                     },
                     defaultStyle: "lowercase"
                 });
 
-            function v(e) {
-                return 48 <= e && e <= 55
+            function v(t) {
+                return 48 <= t && t <= 55
             }
 
-            function A(e) {
-                return 48 <= e && e <= 57
+            function A(t) {
+                return 48 <= t && t <= 57
             }
-            var w = new d("tag:yaml.org,2002:int", {
+            var k = new d("tag:yaml.org,2002:int", {
                     kind: "scalar",
-                    resolve: function(e) {
-                        if (null === e) return !1;
-                        var t, n, i = e.length,
+                    resolve: function(t) {
+                        if (null === t) return !1;
+                        var e, n, i = t.length,
                             r = 0,
                             o = !1;
                         if (!i) return !1;
-                        if ("-" !== (t = e[r]) && "+" !== t || (t = e[++r]), "0" === t) {
+                        if ("-" !== (e = t[r]) && "+" !== e || (e = t[++r]), "0" === e) {
                             if (r + 1 === i) return !0;
-                            if ("b" === (t = e[++r])) {
+                            if ("b" === (e = t[++r])) {
                                 for (r++; r < i; r++)
-                                    if ("_" !== (t = e[r])) {
-                                        if ("0" !== t && "1" !== t) return !1;
+                                    if ("_" !== (e = t[r])) {
+                                        if ("0" !== e && "1" !== e) return !1;
                                         o = !0
-                                    } return o && "_" !== t
+                                    } return o && "_" !== e
                             }
-                            if ("x" === t) {
+                            if ("x" === e) {
                                 for (r++; r < i; r++)
-                                    if ("_" !== (t = e[r])) {
-                                        if (!(48 <= (n = e.charCodeAt(r)) && n <= 57 || 65 <= n && n <= 70 || 97 <= n && n <= 102)) return !1;
+                                    if ("_" !== (e = t[r])) {
+                                        if (!(48 <= (n = t.charCodeAt(r)) && n <= 57 || 65 <= n && n <= 70 || 97 <= n && n <= 102)) return !1;
                                         o = !0
-                                    } return o && "_" !== t
+                                    } return o && "_" !== e
                             }
-                            if ("o" === t) {
+                            if ("o" === e) {
                                 for (r++; r < i; r++)
-                                    if ("_" !== (t = e[r])) {
-                                        if (!v(e.charCodeAt(r))) return !1;
+                                    if ("_" !== (e = t[r])) {
+                                        if (!v(t.charCodeAt(r))) return !1;
                                         o = !0
-                                    } return o && "_" !== t
+                                    } return o && "_" !== e
                             }
                         }
-                        if ("_" === t) return !1;
+                        if ("_" === e) return !1;
                         for (; r < i; r++)
-                            if ("_" !== (t = e[r])) {
-                                if (!A(e.charCodeAt(r))) return !1;
+                            if ("_" !== (e = t[r])) {
+                                if (!A(t.charCodeAt(r))) return !1;
                                 o = !0
-                            } return !(!o || "_" === t)
+                            } return !(!o || "_" === e)
                     },
-                    construct: function(e) {
-                        var t, n = e,
+                    construct: function(t) {
+                        var e, n = t,
                             i = 1;
-                        if (-1 !== n.indexOf("_") && (n = n.replace(/_/g, "")), "-" !== (t = n[0]) && "+" !== t || ("-" === t && (i = -1), t = (n = n.slice(1))[0]), "0" === n) return 0;
-                        if ("0" === t) {
+                        if (-1 !== n.indexOf("_") && (n = n.replace(/_/g, "")), "-" !== (e = n[0]) && "+" !== e || ("-" === e && (i = -1), e = (n = n.slice(1))[0]), "0" === n) return 0;
+                        if ("0" === e) {
                             if ("b" === n[1]) return i * parseInt(n.slice(2), 2);
                             if ("x" === n[1]) return i * parseInt(n.slice(2), 16);
                             if ("o" === n[1]) return i * parseInt(n.slice(2), 8)
                         }
                         return i * parseInt(n, 10)
                     },
-                    predicate: function(e) {
-                        return "[object Number]" === Object.prototype.toString.call(e) && e % 1 == 0 && !r.isNegativeZero(e)
+                    predicate: function(t) {
+                        return "[object Number]" === Object.prototype.toString.call(t) && t % 1 == 0 && !r.isNegativeZero(t)
                     },
                     represent: {
-                        binary: function(e) {
-                            return e >= 0 ? "0b" + e.toString(2) : "-0b" + e.toString(2).slice(1)
+                        binary: function(t) {
+                            return t >= 0 ? "0b" + t.toString(2) : "-0b" + t.toString(2).slice(1)
                         },
-                        octal: function(e) {
-                            return e >= 0 ? "0o" + e.toString(8) : "-0o" + e.toString(8).slice(1)
+                        octal: function(t) {
+                            return t >= 0 ? "0o" + t.toString(8) : "-0o" + t.toString(8).slice(1)
                         },
-                        decimal: function(e) {
-                            return e.toString(10)
+                        decimal: function(t) {
+                            return t.toString(10)
                         },
-                        hexadecimal: function(e) {
-                            return e >= 0 ? "0x" + e.toString(16).toUpperCase() : "-0x" + e.toString(16).toUpperCase().slice(1)
+                        hexadecimal: function(t) {
+                            return t >= 0 ? "0x" + t.toString(16).toUpperCase() : "-0x" + t.toString(16).toUpperCase().slice(1)
                         }
                     },
                     defaultStyle: "decimal",
                     styleAliases: {
                         binary: [2, "bin"],
                         octal: [8, "oct"],
                         decimal: [10, "dec"],
                         hexadecimal: [16, "hex"]
                     }
                 }),
-                k = new RegExp("^(?:[-+]?(?:[0-9][0-9_]*)(?:\\.[0-9_]*)?(?:[eE][-+]?[0-9]+)?|\\.[0-9_]+(?:[eE][-+]?[0-9]+)?|[-+]?\\.(?:inf|Inf|INF)|\\.(?:nan|NaN|NAN))$"),
-                x = /^[-+]?[0-9]+e/,
-                C = new d("tag:yaml.org,2002:float", {
+                C = new RegExp("^(?:[-+]?(?:[0-9][0-9_]*)(?:\\.[0-9_]*)?(?:[eE][-+]?[0-9]+)?|\\.[0-9_]+(?:[eE][-+]?[0-9]+)?|[-+]?\\.(?:inf|Inf|INF)|\\.(?:nan|NaN|NAN))$"),
+                w = /^[-+]?[0-9]+e/,
+                x = new d("tag:yaml.org,2002:float", {
                     kind: "scalar",
-                    resolve: function(e) {
-                        return null !== e && !(!k.test(e) || "_" === e[e.length - 1])
+                    resolve: function(t) {
+                        return null !== t && !(!C.test(t) || "_" === t[t.length - 1])
                     },
-                    construct: function(e) {
-                        var t, n;
-                        return n = "-" === (t = e.replace(/_/g, "").toLowerCase())[0] ? -1 : 1, "+-".indexOf(t[0]) >= 0 && (t = t.slice(1)), ".inf" === t ? 1 === n ? Number.POSITIVE_INFINITY : Number.NEGATIVE_INFINITY : ".nan" === t ? NaN : n * parseFloat(t, 10)
+                    construct: function(t) {
+                        var e, n;
+                        return n = "-" === (e = t.replace(/_/g, "").toLowerCase())[0] ? -1 : 1, "+-".indexOf(e[0]) >= 0 && (e = e.slice(1)), ".inf" === e ? 1 === n ? Number.POSITIVE_INFINITY : Number.NEGATIVE_INFINITY : ".nan" === e ? NaN : n * parseFloat(e, 10)
                     },
-                    predicate: function(e) {
-                        return "[object Number]" === Object.prototype.toString.call(e) && (e % 1 != 0 || r.isNegativeZero(e))
+                    predicate: function(t) {
+                        return "[object Number]" === Object.prototype.toString.call(t) && (t % 1 != 0 || r.isNegativeZero(t))
                     },
-                    represent: function(e, t) {
+                    represent: function(t, e) {
                         var n;
-                        if (isNaN(e)) switch (t) {
+                        if (isNaN(t)) switch (e) {
                             case "lowercase":
                                 return ".nan";
                             case "uppercase":
                                 return ".NAN";
                             case "camelcase":
                                 return ".NaN"
-                        } else if (Number.POSITIVE_INFINITY === e) switch (t) {
+                        } else if (Number.POSITIVE_INFINITY === t) switch (e) {
                             case "lowercase":
                                 return ".inf";
                             case "uppercase":
                                 return ".INF";
                             case "camelcase":
                                 return ".Inf"
-                        } else if (Number.NEGATIVE_INFINITY === e) switch (t) {
+                        } else if (Number.NEGATIVE_INFINITY === t) switch (e) {
                             case "lowercase":
                                 return "-.inf";
                             case "uppercase":
                                 return "-.INF";
                             case "camelcase":
                                 return "-.Inf"
-                        } else if (r.isNegativeZero(e)) return "-0.0";
-                        return n = e.toString(10), x.test(n) ? n.replace("e", ".e") : n
+                        } else if (r.isNegativeZero(t)) return "-0.0";
+                        return n = t.toString(10), w.test(n) ? n.replace("e", ".e") : n
                     },
                     defaultStyle: "lowercase"
                 }),
                 I = m.extend({
-                    implicit: [y, b, w, C]
+                    implicit: [y, b, k, x]
                 }),
-                j = new RegExp("^([0-9][0-9][0-9][0-9])-([0-9][0-9])-([0-9][0-9])$"),
-                O = new RegExp("^([0-9][0-9][0-9][0-9])-([0-9][0-9]?)-([0-9][0-9]?)(?:[Tt]|[ \\t]+)([0-9][0-9]?):([0-9][0-9]):([0-9][0-9])(?:\\.([0-9]*))?(?:[ \\t]*(Z|([-+])([0-9][0-9]?)(?::([0-9][0-9]))?))?$"),
-                S = new d("tag:yaml.org,2002:timestamp", {
+                S = new RegExp("^([0-9][0-9][0-9][0-9])-([0-9][0-9])-([0-9][0-9])$"),
+                j = new RegExp("^([0-9][0-9][0-9][0-9])-([0-9][0-9]?)-([0-9][0-9]?)(?:[Tt]|[ \\t]+)([0-9][0-9]?):([0-9][0-9]):([0-9][0-9])(?:\\.([0-9]*))?(?:[ \\t]*(Z|([-+])([0-9][0-9]?)(?::([0-9][0-9]))?))?$"),
+                T = new d("tag:yaml.org,2002:timestamp", {
                     kind: "scalar",
-                    resolve: function(e) {
-                        return null !== e && (null !== j.exec(e) || null !== O.exec(e))
+                    resolve: function(t) {
+                        return null !== t && (null !== S.exec(t) || null !== j.exec(t))
                     },
-                    construct: function(e) {
-                        var t, n, i, r, o, a, l, c, s = 0,
+                    construct: function(t) {
+                        var e, n, i, r, o, a, c, l, s = 0,
                             u = null;
-                        if (null === (t = j.exec(e)) && (t = O.exec(e)), null === t) throw new Error("Date resolve error");
-                        if (n = +t[1], i = +t[2] - 1, r = +t[3], !t[4]) return new Date(Date.UTC(n, i, r));
-                        if (o = +t[4], a = +t[5], l = +t[6], t[7]) {
-                            for (s = t[7].slice(0, 3); s.length < 3;) s += "0";
+                        if (null === (e = S.exec(t)) && (e = j.exec(t)), null === e) throw new Error("Date resolve error");
+                        if (n = +e[1], i = +e[2] - 1, r = +e[3], !e[4]) return new Date(Date.UTC(n, i, r));
+                        if (o = +e[4], a = +e[5], c = +e[6], e[7]) {
+                            for (s = e[7].slice(0, 3); s.length < 3;) s += "0";
                             s = +s
                         }
-                        return t[9] && (u = 6e4 * (60 * +t[10] + +(t[11] || 0)), "-" === t[9] && (u = -u)), c = new Date(Date.UTC(n, i, r, o, a, l, s)), u && c.setTime(c.getTime() - u), c
+                        return e[9] && (u = 6e4 * (60 * +e[10] + +(e[11] || 0)), "-" === e[9] && (u = -u)), l = new Date(Date.UTC(n, i, r, o, a, c, s)), u && l.setTime(l.getTime() - u), l
                     },
                     instanceOf: Date,
-                    represent: function(e) {
-                        return e.toISOString()
+                    represent: function(t) {
+                        return t.toISOString()
                     }
                 }),
-                T = new d("tag:yaml.org,2002:merge", {
+                O = new d("tag:yaml.org,2002:merge", {
                     kind: "scalar",
-                    resolve: function(e) {
-                        return "<<" === e || null === e
+                    resolve: function(t) {
+                        return "<<" === t || null === t
                     }
                 }),
                 N = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=\n\r",
-                F = new d("tag:yaml.org,2002:binary", {
+                E = new d("tag:yaml.org,2002:binary", {
                     kind: "scalar",
-                    resolve: function(e) {
-                        if (null === e) return !1;
-                        var t, n, i = 0,
-                            r = e.length,
+                    resolve: function(t) {
+                        if (null === t) return !1;
+                        var e, n, i = 0,
+                            r = t.length,
                             o = N;
                         for (n = 0; n < r; n++)
-                            if (!((t = o.indexOf(e.charAt(n))) > 64)) {
-                                if (t < 0) return !1;
+                            if (!((e = o.indexOf(t.charAt(n))) > 64)) {
+                                if (e < 0) return !1;
                                 i += 6
                             } return i % 8 == 0
                     },
-                    construct: function(e) {
-                        var t, n, i = e.replace(/[\r\n=]/g, ""),
+                    construct: function(t) {
+                        var e, n, i = t.replace(/[\r\n=]/g, ""),
                             r = i.length,
                             o = N,
                             a = 0,
-                            l = [];
-                        for (t = 0; t < r; t++) t % 4 == 0 && t && (l.push(a >> 16 & 255), l.push(a >> 8 & 255), l.push(255 & a)), a = a << 6 | o.indexOf(i.charAt(t));
-                        return 0 == (n = r % 4 * 6) ? (l.push(a >> 16 & 255), l.push(a >> 8 & 255), l.push(255 & a)) : 18 === n ? (l.push(a >> 10 & 255), l.push(a >> 2 & 255)) : 12 === n && l.push(a >> 4 & 255), new Uint8Array(l)
+                            c = [];
+                        for (e = 0; e < r; e++) e % 4 == 0 && e && (c.push(a >> 16 & 255), c.push(a >> 8 & 255), c.push(255 & a)), a = a << 6 | o.indexOf(i.charAt(e));
+                        return 0 == (n = r % 4 * 6) ? (c.push(a >> 16 & 255), c.push(a >> 8 & 255), c.push(255 & a)) : 18 === n ? (c.push(a >> 10 & 255), c.push(a >> 2 & 255)) : 12 === n && c.push(a >> 4 & 255), new Uint8Array(c)
                     },
-                    predicate: function(e) {
-                        return "[object Uint8Array]" === Object.prototype.toString.call(e)
+                    predicate: function(t) {
+                        return "[object Uint8Array]" === Object.prototype.toString.call(t)
                     },
-                    represent: function(e) {
-                        var t, n, i = "",
+                    represent: function(t) {
+                        var e, n, i = "",
                             r = 0,
-                            o = e.length,
+                            o = t.length,
                             a = N;
-                        for (t = 0; t < o; t++) t % 3 == 0 && t && (i += a[r >> 18 & 63], i += a[r >> 12 & 63], i += a[r >> 6 & 63], i += a[63 & r]), r = (r << 8) + e[t];
+                        for (e = 0; e < o; e++) e % 3 == 0 && e && (i += a[r >> 18 & 63], i += a[r >> 12 & 63], i += a[r >> 6 & 63], i += a[63 & r]), r = (r << 8) + t[e];
                         return 0 == (n = o % 3) ? (i += a[r >> 18 & 63], i += a[r >> 12 & 63], i += a[r >> 6 & 63], i += a[63 & r]) : 2 === n ? (i += a[r >> 10 & 63], i += a[r >> 4 & 63], i += a[r << 2 & 63], i += a[64]) : 1 === n && (i += a[r >> 2 & 63], i += a[r << 4 & 63], i += a[64], i += a[64]), i
                     }
                 }),
                 M = Object.prototype.hasOwnProperty,
                 L = Object.prototype.toString,
-                E = new d("tag:yaml.org,2002:omap", {
+                F = new d("tag:yaml.org,2002:omap", {
                     kind: "sequence",
-                    resolve: function(e) {
-                        if (null === e) return !0;
-                        var t, n, i, r, o, a = [],
-                            l = e;
-                        for (t = 0, n = l.length; t < n; t += 1) {
-                            if (i = l[t], o = !1, "[object Object]" !== L.call(i)) return !1;
+                    resolve: function(t) {
+                        if (null === t) return !0;
+                        var e, n, i, r, o, a = [],
+                            c = t;
+                        for (e = 0, n = c.length; e < n; e += 1) {
+                            if (i = c[e], o = !1, "[object Object]" !== L.call(i)) return !1;
                             for (r in i)
                                 if (M.call(i, r)) {
                                     if (o) return !1;
                                     o = !0
                                 } if (!o) return !1;
                             if (-1 !== a.indexOf(r)) return !1;
                             a.push(r)
                         }
                         return !0
                     },
-                    construct: function(e) {
-                        return null !== e ? e : []
+                    construct: function(t) {
+                        return null !== t ? t : []
                     }
                 }),
                 _ = Object.prototype.toString,
                 q = new d("tag:yaml.org,2002:pairs", {
                     kind: "sequence",
-                    resolve: function(e) {
-                        if (null === e) return !0;
-                        var t, n, i, r, o, a = e;
-                        for (o = new Array(a.length), t = 0, n = a.length; t < n; t += 1) {
-                            if (i = a[t], "[object Object]" !== _.call(i)) return !1;
+                    resolve: function(t) {
+                        if (null === t) return !0;
+                        var e, n, i, r, o, a = t;
+                        for (o = new Array(a.length), e = 0, n = a.length; e < n; e += 1) {
+                            if (i = a[e], "[object Object]" !== _.call(i)) return !1;
                             if (1 !== (r = Object.keys(i)).length) return !1;
-                            o[t] = [r[0], i[r[0]]]
+                            o[e] = [r[0], i[r[0]]]
                         }
                         return !0
                     },
-                    construct: function(e) {
-                        if (null === e) return [];
-                        var t, n, i, r, o, a = e;
-                        for (o = new Array(a.length), t = 0, n = a.length; t < n; t += 1) i = a[t], r = Object.keys(i), o[t] = [r[0], i[r[0]]];
+                    construct: function(t) {
+                        if (null === t) return [];
+                        var e, n, i, r, o, a = t;
+                        for (o = new Array(a.length), e = 0, n = a.length; e < n; e += 1) i = a[e], r = Object.keys(i), o[e] = [r[0], i[r[0]]];
                         return o
                     }
                 }),
-                D = Object.prototype.hasOwnProperty,
-                U = new d("tag:yaml.org,2002:set", {
+                U = Object.prototype.hasOwnProperty,
+                D = new d("tag:yaml.org,2002:set", {
                     kind: "mapping",
-                    resolve: function(e) {
-                        if (null === e) return !0;
-                        var t, n = e;
-                        for (t in n)
-                            if (D.call(n, t) && null !== n[t]) return !1;
+                    resolve: function(t) {
+                        if (null === t) return !0;
+                        var e, n = t;
+                        for (e in n)
+                            if (U.call(n, e) && null !== n[e]) return !1;
                         return !0
                     },
-                    construct: function(e) {
-                        return null !== e ? e : {}
+                    construct: function(t) {
+                        return null !== t ? t : {}
                     }
                 }),
                 Y = I.extend({
-                    implicit: [S, T],
-                    explicit: [F, E, q, U]
+                    implicit: [T, O],
+                    explicit: [E, F, q, D]
                 }),
-                R = Object.prototype.hasOwnProperty,
-                B = 1,
-                $ = 2,
-                K = 3,
-                P = 4,
-                W = 1,
-                G = 2,
-                V = 3,
-                Z = /[\x00-\x08\x0B\x0C\x0E-\x1F\x7F-\x84\x86-\x9F\uFFFE\uFFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]/,
-                Q = /[\x85\u2028\u2029]/,
-                z = /[,\[\]\{\}]/,
-                H = /^(?:!|!!|![a-z\-]+!)$/i,
-                J = /^(?:!|[^,\[\]\{\}])(?:%[0-9a-f]{2}|[0-9a-z\-#;\/\?:@&=\+\$,_\.!~\*'\(\)\[\]])*$/i;
+                B = Object.prototype.hasOwnProperty,
+                R = 1,
+                P = 2,
+                $ = 3,
+                G = 4,
+                V = 1,
+                Z = 2,
+                W = 3,
+                z = /[\x00-\x08\x0B\x0C\x0E-\x1F\x7F-\x84\x86-\x9F\uFFFE\uFFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]/,
+                H = /[\x85\u2028\u2029]/,
+                J = /[,\[\]\{\}]/,
+                K = /^(?:!|!!|![a-z\-]+!)$/i,
+                Q = /^(?:!|[^,\[\]\{\}])(?:%[0-9a-f]{2}|[0-9a-z\-#;\/\?:@&=\+\$,_\.!~\*'\(\)\[\]])*$/i;
 
-            function X(e) {
-                return Object.prototype.toString.call(e)
+            function X(t) {
+                return Object.prototype.toString.call(t)
             }
 
-            function ee(e) {
-                return 10 === e || 13 === e
+            function tt(t) {
+                return 10 === t || 13 === t
             }
 
-            function te(e) {
-                return 9 === e || 32 === e
+            function et(t) {
+                return 9 === t || 32 === t
             }
 
-            function ne(e) {
-                return 9 === e || 32 === e || 10 === e || 13 === e
+            function nt(t) {
+                return 9 === t || 32 === t || 10 === t || 13 === t
             }
 
-            function ie(e) {
-                return 44 === e || 91 === e || 93 === e || 123 === e || 125 === e
+            function it(t) {
+                return 44 === t || 91 === t || 93 === t || 123 === t || 125 === t
             }
 
-            function re(e) {
-                var t;
-                return 48 <= e && e <= 57 ? e - 48 : 97 <= (t = 32 | e) && t <= 102 ? t - 97 + 10 : -1
+            function rt(t) {
+                var e;
+                return 48 <= t && t <= 57 ? t - 48 : 97 <= (e = 32 | t) && e <= 102 ? e - 97 + 10 : -1
             }
 
-            function oe(e) {
-                return 48 === e ? "\0" : 97 === e ? "" : 98 === e ? "\b" : 116 === e || 9 === e ? "\t" : 110 === e ? "\n" : 118 === e ? "\v" : 102 === e ? "\f" : 114 === e ? "\r" : 101 === e ? "" : 32 === e ? " " : 34 === e ? '"' : 47 === e ? "/" : 92 === e ? "\\" : 78 === e ? "" : 95 === e ? " " : 76 === e ? "\u2028" : 80 === e ? "\u2029" : ""
+            function ot(t) {
+                return 48 === t ? "\0" : 97 === t ? "" : 98 === t ? "\b" : 116 === t || 9 === t ? "\t" : 110 === t ? "\n" : 118 === t ? "\v" : 102 === t ? "\f" : 114 === t ? "\r" : 101 === t ? "" : 32 === t ? " " : 34 === t ? '"' : 47 === t ? "/" : 92 === t ? "\\" : 78 === t ? "" : 95 === t ? " " : 76 === t ? "\u2028" : 80 === t ? "\u2029" : ""
             }
 
-            function ae(e) {
-                return e <= 65535 ? String.fromCharCode(e) : String.fromCharCode(55296 + (e - 65536 >> 10), 56320 + (e - 65536 & 1023))
+            function at(t) {
+                return t <= 65535 ? String.fromCharCode(t) : String.fromCharCode(55296 + (t - 65536 >> 10), 56320 + (t - 65536 & 1023))
             }
-            for (var le = new Array(256), ce = new Array(256), se = 0; se < 256; se++) le[se] = oe(se) ? 1 : 0, ce[se] = oe(se);
+            for (var ct = new Array(256), lt = new Array(256), st = 0; st < 256; st++) ct[st] = ot(st) ? 1 : 0, lt[st] = ot(st);
 
-            function ue(e, t) {
-                this.input = e, this.filename = t.filename || null, this.schema = t.schema || Y, this.onWarning = t.onWarning || null, this.legacy = t.legacy || !1, this.json = t.json || !1, this.listener = t.listener || null, this.implicitTypes = this.schema.compiledImplicit, this.typeMap = this.schema.compiledTypeMap, this.length = e.length, this.position = 0, this.line = 0, this.lineStart = 0, this.lineIndent = 0, this.firstTabInLine = -1, this.documents = []
+            function ut(t, e) {
+                this.input = t, this.filename = e.filename || null, this.schema = e.schema || Y, this.onWarning = e.onWarning || null, this.legacy = e.legacy || !1, this.json = e.json || !1, this.listener = e.listener || null, this.implicitTypes = this.schema.compiledImplicit, this.typeMap = this.schema.compiledTypeMap, this.length = t.length, this.position = 0, this.line = 0, this.lineStart = 0, this.lineIndent = 0, this.firstTabInLine = -1, this.documents = []
             }
 
-            function pe(e, t) {
+            function pt(t, e) {
                 var n = {
-                    name: e.filename,
-                    buffer: e.input.slice(0, -1),
-                    position: e.position,
-                    line: e.line,
-                    column: e.position - e.lineStart
+                    name: t.filename,
+                    buffer: t.input.slice(0, -1),
+                    position: t.position,
+                    line: t.line,
+                    column: t.position - t.lineStart
                 };
-                return n.snippet = u(n), new l(t, n)
+                return n.snippet = u(n), new c(e, n)
             }
 
-            function fe(e, t) {
-                throw pe(e, t)
+            function ft(t, e) {
+                throw pt(t, e)
             }
 
-            function de(e, t) {
-                e.onWarning && e.onWarning.call(null, pe(e, t))
+            function dt(t, e) {
+                t.onWarning && t.onWarning.call(null, pt(t, e))
             }
-            var he = {
-                YAML: function(e, t, n) {
+            var ht = {
+                YAML: function(t, e, n) {
                     var i, r, o;
-                    null !== e.version && fe(e, "duplication of %YAML directive"), 1 !== n.length && fe(e, "YAML directive accepts exactly one argument"), null === (i = /^([0-9]+)\.([0-9]+)$/.exec(n[0])) && fe(e, "ill-formed argument of the YAML directive"), r = parseInt(i[1], 10), o = parseInt(i[2], 10), 1 !== r && fe(e, "unacceptable YAML version of the document"), e.version = n[0], e.checkLineBreaks = o < 2, 1 !== o && 2 !== o && de(e, "unsupported YAML version of the document")
+                    null !== t.version && ft(t, "duplication of %YAML directive"), 1 !== n.length && ft(t, "YAML directive accepts exactly one argument"), null === (i = /^([0-9]+)\.([0-9]+)$/.exec(n[0])) && ft(t, "ill-formed argument of the YAML directive"), r = parseInt(i[1], 10), o = parseInt(i[2], 10), 1 !== r && ft(t, "unacceptable YAML version of the document"), t.version = n[0], t.checkLineBreaks = o < 2, 1 !== o && 2 !== o && dt(t, "unsupported YAML version of the document")
                 },
-                TAG: function(e, t, n) {
+                TAG: function(t, e, n) {
                     var i, r;
-                    2 !== n.length && fe(e, "TAG directive accepts exactly two arguments"), i = n[0], r = n[1], H.test(i) || fe(e, "ill-formed tag handle (first argument) of the TAG directive"), R.call(e.tagMap, i) && fe(e, 'there is a previously declared suffix for "' + i + '" tag handle'), J.test(r) || fe(e, "ill-formed tag prefix (second argument) of the TAG directive");
+                    2 !== n.length && ft(t, "TAG directive accepts exactly two arguments"), i = n[0], r = n[1], K.test(i) || ft(t, "ill-formed tag handle (first argument) of the TAG directive"), B.call(t.tagMap, i) && ft(t, 'there is a previously declared suffix for "' + i + '" tag handle'), Q.test(r) || ft(t, "ill-formed tag prefix (second argument) of the TAG directive");
                     try {
                         r = decodeURIComponent(r)
-                    } catch (t) {
-                        fe(e, "tag prefix is malformed: " + r)
+                    } catch (e) {
+                        ft(t, "tag prefix is malformed: " + r)
                     }
-                    e.tagMap[i] = r
+                    t.tagMap[i] = r
                 }
             };
 
-            function ge(e, t, n, i) {
-                var r, o, a, l;
-                if (t < n) {
-                    if (l = e.input.slice(t, n), i)
-                        for (r = 0, o = l.length; r < o; r += 1) 9 === (a = l.charCodeAt(r)) || 32 <= a && a <= 1114111 || fe(e, "expected valid JSON character");
-                    else Z.test(l) && fe(e, "the stream contains non-printable characters");
-                    e.result += l
+            function gt(t, e, n, i) {
+                var r, o, a, c;
+                if (e < n) {
+                    if (c = t.input.slice(e, n), i)
+                        for (r = 0, o = c.length; r < o; r += 1) 9 === (a = c.charCodeAt(r)) || 32 <= a && a <= 1114111 || ft(t, "expected valid JSON character");
+                    else z.test(c) && ft(t, "the stream contains non-printable characters");
+                    t.result += c
                 }
             }
 
-            function me(e, t, n, i) {
-                var o, a, l, c;
-                for (r.isObject(n) || fe(e, "cannot merge mappings; the provided source object is unacceptable"), l = 0, c = (o = Object.keys(n)).length; l < c; l += 1) a = o[l], R.call(t, a) || (t[a] = n[a], i[a] = !0)
+            function mt(t, e, n, i) {
+                var o, a, c, l;
+                for (r.isObject(n) || ft(t, "cannot merge mappings; the provided source object is unacceptable"), c = 0, l = (o = Object.keys(n)).length; c < l; c += 1) a = o[c], B.call(e, a) || (e[a] = n[a], i[a] = !0)
             }
 
-            function ye(e, t, n, i, r, o, a, l, c) {
+            function yt(t, e, n, i, r, o, a, c, l) {
                 var s, u;
                 if (Array.isArray(r))
-                    for (s = 0, u = (r = Array.prototype.slice.call(r)).length; s < u; s += 1) Array.isArray(r[s]) && fe(e, "nested arrays are not supported inside keys"), "object" == typeof r && "[object Object]" === X(r[s]) && (r[s] = "[object Object]");
-                if ("object" == typeof r && "[object Object]" === X(r) && (r = "[object Object]"), r = String(r), null === t && (t = {}), "tag:yaml.org,2002:merge" === i)
+                    for (s = 0, u = (r = Array.prototype.slice.call(r)).length; s < u; s += 1) Array.isArray(r[s]) && ft(t, "nested arrays are not supported inside keys"), "object" == typeof r && "[object Object]" === X(r[s]) && (r[s] = "[object Object]");
+                if ("object" == typeof r && "[object Object]" === X(r) && (r = "[object Object]"), r = String(r), null === e && (e = {}), "tag:yaml.org,2002:merge" === i)
                     if (Array.isArray(o))
-                        for (s = 0, u = o.length; s < u; s += 1) me(e, t, o[s], n);
-                    else me(e, t, o, n);
-                else e.json || R.call(n, r) || !R.call(t, r) || (e.line = a || e.line, e.lineStart = l || e.lineStart, e.position = c || e.position, fe(e, "duplicated mapping key")), "__proto__" === r ? Object.defineProperty(t, r, {
+                        for (s = 0, u = o.length; s < u; s += 1) mt(t, e, o[s], n);
+                    else mt(t, e, o, n);
+                else t.json || B.call(n, r) || !B.call(e, r) || (t.line = a || t.line, t.lineStart = c || t.lineStart, t.position = l || t.position, ft(t, "duplicated mapping key")), "__proto__" === r ? Object.defineProperty(e, r, {
                     configurable: !0,
                     enumerable: !0,
                     writable: !0,
                     value: o
-                }) : t[r] = o, delete n[r];
-                return t
+                }) : e[r] = o, delete n[r];
+                return e
             }
 
-            function be(e) {
-                var t;
-                10 === (t = e.input.charCodeAt(e.position)) ? e.position++ : 13 === t ? (e.position++, 10 === e.input.charCodeAt(e.position) && e.position++) : fe(e, "a line break is expected"), e.line += 1, e.lineStart = e.position, e.firstTabInLine = -1
+            function bt(t) {
+                var e;
+                10 === (e = t.input.charCodeAt(t.position)) ? t.position++ : 13 === e ? (t.position++, 10 === t.input.charCodeAt(t.position) && t.position++) : ft(t, "a line break is expected"), t.line += 1, t.lineStart = t.position, t.firstTabInLine = -1
             }
 
-            function ve(e, t, n) {
-                for (var i = 0, r = e.input.charCodeAt(e.position); 0 !== r;) {
-                    for (; te(r);) 9 === r && -1 === e.firstTabInLine && (e.firstTabInLine = e.position), r = e.input.charCodeAt(++e.position);
-                    if (t && 35 === r)
+            function vt(t, e, n) {
+                for (var i = 0, r = t.input.charCodeAt(t.position); 0 !== r;) {
+                    for (; et(r);) 9 === r && -1 === t.firstTabInLine && (t.firstTabInLine = t.position), r = t.input.charCodeAt(++t.position);
+                    if (e && 35 === r)
                         do {
-                            r = e.input.charCodeAt(++e.position)
+                            r = t.input.charCodeAt(++t.position)
                         } while (10 !== r && 13 !== r && 0 !== r);
-                    if (!ee(r)) break;
-                    for (be(e), r = e.input.charCodeAt(e.position), i++, e.lineIndent = 0; 32 === r;) e.lineIndent++, r = e.input.charCodeAt(++e.position)
+                    if (!tt(r)) break;
+                    for (bt(t), r = t.input.charCodeAt(t.position), i++, t.lineIndent = 0; 32 === r;) t.lineIndent++, r = t.input.charCodeAt(++t.position)
                 }
-                return -1 !== n && 0 !== i && e.lineIndent < n && de(e, "deficient indentation"), i
+                return -1 !== n && 0 !== i && t.lineIndent < n && dt(t, "deficient indentation"), i
             }
 
-            function Ae(e) {
-                var t, n = e.position;
-                return !(45 !== (t = e.input.charCodeAt(n)) && 46 !== t || t !== e.input.charCodeAt(n + 1) || t !== e.input.charCodeAt(n + 2) || (n += 3, 0 !== (t = e.input.charCodeAt(n)) && !ne(t)))
+            function At(t) {
+                var e, n = t.position;
+                return !(45 !== (e = t.input.charCodeAt(n)) && 46 !== e || e !== t.input.charCodeAt(n + 1) || e !== t.input.charCodeAt(n + 2) || (n += 3, 0 !== (e = t.input.charCodeAt(n)) && !nt(e)))
             }
 
-            function we(e, t) {
-                1 === t ? e.result += " " : t > 1 && (e.result += r.repeat("\n", t - 1))
+            function kt(t, e) {
+                1 === e ? t.result += " " : e > 1 && (t.result += r.repeat("\n", e - 1))
             }
 
-            function ke(e, t) {
-                var n, i, r = e.tag,
-                    o = e.anchor,
+            function Ct(t, e) {
+                var n, i, r = t.tag,
+                    o = t.anchor,
                     a = [],
-                    l = !1;
-                if (-1 !== e.firstTabInLine) return !1;
-                for (null !== e.anchor && (e.anchorMap[e.anchor] = a), i = e.input.charCodeAt(e.position); 0 !== i && (-1 !== e.firstTabInLine && (e.position = e.firstTabInLine, fe(e, "tab characters must not be used in indentation")), 45 === i) && ne(e.input.charCodeAt(e.position + 1));)
-                    if (l = !0, e.position++, ve(e, !0, -1) && e.lineIndent <= t) a.push(null), i = e.input.charCodeAt(e.position);
-                    else if (n = e.line, Ie(e, t, K, !1, !0), a.push(e.result), ve(e, !0, -1), i = e.input.charCodeAt(e.position), (e.line === n || e.lineIndent > t) && 0 !== i) fe(e, "bad indentation of a sequence entry");
-                else if (e.lineIndent < t) break;
-                return !!l && (e.tag = r, e.anchor = o, e.kind = "sequence", e.result = a, !0)
+                    c = !1;
+                if (-1 !== t.firstTabInLine) return !1;
+                for (null !== t.anchor && (t.anchorMap[t.anchor] = a), i = t.input.charCodeAt(t.position); 0 !== i && (-1 !== t.firstTabInLine && (t.position = t.firstTabInLine, ft(t, "tab characters must not be used in indentation")), 45 === i) && nt(t.input.charCodeAt(t.position + 1));)
+                    if (c = !0, t.position++, vt(t, !0, -1) && t.lineIndent <= e) a.push(null), i = t.input.charCodeAt(t.position);
+                    else if (n = t.line, It(t, e, $, !1, !0), a.push(t.result), vt(t, !0, -1), i = t.input.charCodeAt(t.position), (t.line === n || t.lineIndent > e) && 0 !== i) ft(t, "bad indentation of a sequence entry");
+                else if (t.lineIndent < e) break;
+                return !!c && (t.tag = r, t.anchor = o, t.kind = "sequence", t.result = a, !0)
             }
 
-            function xe(e) {
-                var t, n, i, r, o = !1,
+            function wt(t) {
+                var e, n, i, r, o = !1,
                     a = !1;
-                if (33 !== (r = e.input.charCodeAt(e.position))) return !1;
-                if (null !== e.tag && fe(e, "duplication of a tag property"), 60 === (r = e.input.charCodeAt(++e.position)) ? (o = !0, r = e.input.charCodeAt(++e.position)) : 33 === r ? (a = !0, n = "!!", r = e.input.charCodeAt(++e.position)) : n = "!", t = e.position, o) {
+                if (33 !== (r = t.input.charCodeAt(t.position))) return !1;
+                if (null !== t.tag && ft(t, "duplication of a tag property"), 60 === (r = t.input.charCodeAt(++t.position)) ? (o = !0, r = t.input.charCodeAt(++t.position)) : 33 === r ? (a = !0, n = "!!", r = t.input.charCodeAt(++t.position)) : n = "!", e = t.position, o) {
                     do {
-                        r = e.input.charCodeAt(++e.position)
+                        r = t.input.charCodeAt(++t.position)
                     } while (0 !== r && 62 !== r);
-                    e.position < e.length ? (i = e.input.slice(t, e.position), r = e.input.charCodeAt(++e.position)) : fe(e, "unexpected end of the stream within a verbatim tag")
+                    t.position < t.length ? (i = t.input.slice(e, t.position), r = t.input.charCodeAt(++t.position)) : ft(t, "unexpected end of the stream within a verbatim tag")
                 } else {
-                    for (; 0 !== r && !ne(r);) 33 === r && (a ? fe(e, "tag suffix cannot contain exclamation marks") : (n = e.input.slice(t - 1, e.position + 1), H.test(n) || fe(e, "named tag handle cannot contain such characters"), a = !0, t = e.position + 1)), r = e.input.charCodeAt(++e.position);
-                    i = e.input.slice(t, e.position), z.test(i) && fe(e, "tag suffix cannot contain flow indicator characters")
+                    for (; 0 !== r && !nt(r);) 33 === r && (a ? ft(t, "tag suffix cannot contain exclamation marks") : (n = t.input.slice(e - 1, t.position + 1), K.test(n) || ft(t, "named tag handle cannot contain such characters"), a = !0, e = t.position + 1)), r = t.input.charCodeAt(++t.position);
+                    i = t.input.slice(e, t.position), J.test(i) && ft(t, "tag suffix cannot contain flow indicator characters")
                 }
-                i && !J.test(i) && fe(e, "tag name cannot contain such characters: " + i);
+                i && !Q.test(i) && ft(t, "tag name cannot contain such characters: " + i);
                 try {
                     i = decodeURIComponent(i)
-                } catch (t) {
-                    fe(e, "tag name is malformed: " + i)
+                } catch (e) {
+                    ft(t, "tag name is malformed: " + i)
                 }
-                return o ? e.tag = i : R.call(e.tagMap, n) ? e.tag = e.tagMap[n] + i : "!" === n ? e.tag = "!" + i : "!!" === n ? e.tag = "tag:yaml.org,2002:" + i : fe(e, 'undeclared tag handle "' + n + '"'), !0
+                return o ? t.tag = i : B.call(t.tagMap, n) ? t.tag = t.tagMap[n] + i : "!" === n ? t.tag = "!" + i : "!!" === n ? t.tag = "tag:yaml.org,2002:" + i : ft(t, 'undeclared tag handle "' + n + '"'), !0
             }
 
-            function Ce(e) {
-                var t, n;
-                if (38 !== (n = e.input.charCodeAt(e.position))) return !1;
-                for (null !== e.anchor && fe(e, "duplication of an anchor property"), n = e.input.charCodeAt(++e.position), t = e.position; 0 !== n && !ne(n) && !ie(n);) n = e.input.charCodeAt(++e.position);
-                return e.position === t && fe(e, "name of an anchor node must contain at least one character"), e.anchor = e.input.slice(t, e.position), !0
+            function xt(t) {
+                var e, n;
+                if (38 !== (n = t.input.charCodeAt(t.position))) return !1;
+                for (null !== t.anchor && ft(t, "duplication of an anchor property"), n = t.input.charCodeAt(++t.position), e = t.position; 0 !== n && !nt(n) && !it(n);) n = t.input.charCodeAt(++t.position);
+                return t.position === e && ft(t, "name of an anchor node must contain at least one character"), t.anchor = t.input.slice(e, t.position), !0
             }
 
-            function Ie(e, t, n, i, o) {
-                var a, l, c, s, u, p, f, d, h, g = 1,
+            function It(t, e, n, i, o) {
+                var a, c, l, s, u, p, f, d, h, g = 1,
                     m = !1,
                     y = !1;
-                if (null !== e.listener && e.listener("open", e), e.tag = null, e.anchor = null, e.kind = null, e.result = null, a = l = c = P === n || K === n, i && ve(e, !0, -1) && (m = !0, e.lineIndent > t ? g = 1 : e.lineIndent === t ? g = 0 : e.lineIndent < t && (g = -1)), 1 === g)
-                    for (; xe(e) || Ce(e);) ve(e, !0, -1) ? (m = !0, c = a, e.lineIndent > t ? g = 1 : e.lineIndent === t ? g = 0 : e.lineIndent < t && (g = -1)) : c = !1;
-                if (c && (c = m || o), 1 !== g && P !== n || (d = B === n || $ === n ? t : t + 1, h = e.position - e.lineStart, 1 === g ? c && (ke(e, h) || function(e, t, n) {
-                        var i, r, o, a, l, c, s, u = e.tag,
-                            p = e.anchor,
+                if (null !== t.listener && t.listener("open", t), t.tag = null, t.anchor = null, t.kind = null, t.result = null, a = c = l = G === n || $ === n, i && vt(t, !0, -1) && (m = !0, t.lineIndent > e ? g = 1 : t.lineIndent === e ? g = 0 : t.lineIndent < e && (g = -1)), 1 === g)
+                    for (; wt(t) || xt(t);) vt(t, !0, -1) ? (m = !0, l = a, t.lineIndent > e ? g = 1 : t.lineIndent === e ? g = 0 : t.lineIndent < e && (g = -1)) : l = !1;
+                if (l && (l = m || o), 1 !== g && G !== n || (d = R === n || P === n ? e : e + 1, h = t.position - t.lineStart, 1 === g ? l && (Ct(t, h) || function(t, e, n) {
+                        var i, r, o, a, c, l, s, u = t.tag,
+                            p = t.anchor,
                             f = {},
                             d = Object.create(null),
                             h = null,
                             g = null,
                             m = null,
                             y = !1,
                             b = !1;
-                        if (-1 !== e.firstTabInLine) return !1;
-                        for (null !== e.anchor && (e.anchorMap[e.anchor] = f), s = e.input.charCodeAt(e.position); 0 !== s;) {
-                            if (y || -1 === e.firstTabInLine || (e.position = e.firstTabInLine, fe(e, "tab characters must not be used in indentation")), i = e.input.charCodeAt(e.position + 1), o = e.line, 63 !== s && 58 !== s || !ne(i)) {
-                                if (a = e.line, l = e.lineStart, c = e.position, !Ie(e, n, $, !1, !0)) break;
-                                if (e.line === o) {
-                                    for (s = e.input.charCodeAt(e.position); te(s);) s = e.input.charCodeAt(++e.position);
-                                    if (58 === s) ne(s = e.input.charCodeAt(++e.position)) || fe(e, "a whitespace character is expected after the key-value separator within a block mapping"), y && (ye(e, f, d, h, g, null, a, l, c), h = g = m = null), b = !0, y = !1, r = !1, h = e.tag, g = e.result;
+                        if (-1 !== t.firstTabInLine) return !1;
+                        for (null !== t.anchor && (t.anchorMap[t.anchor] = f), s = t.input.charCodeAt(t.position); 0 !== s;) {
+                            if (y || -1 === t.firstTabInLine || (t.position = t.firstTabInLine, ft(t, "tab characters must not be used in indentation")), i = t.input.charCodeAt(t.position + 1), o = t.line, 63 !== s && 58 !== s || !nt(i)) {
+                                if (a = t.line, c = t.lineStart, l = t.position, !It(t, n, P, !1, !0)) break;
+                                if (t.line === o) {
+                                    for (s = t.input.charCodeAt(t.position); et(s);) s = t.input.charCodeAt(++t.position);
+                                    if (58 === s) nt(s = t.input.charCodeAt(++t.position)) || ft(t, "a whitespace character is expected after the key-value separator within a block mapping"), y && (yt(t, f, d, h, g, null, a, c, l), h = g = m = null), b = !0, y = !1, r = !1, h = t.tag, g = t.result;
                                     else {
-                                        if (!b) return e.tag = u, e.anchor = p, !0;
-                                        fe(e, "can not read an implicit mapping pair; a colon is missed")
+                                        if (!b) return t.tag = u, t.anchor = p, !0;
+                                        ft(t, "can not read an implicit mapping pair; a colon is missed")
                                     }
                                 } else {
-                                    if (!b) return e.tag = u, e.anchor = p, !0;
-                                    fe(e, "can not read a block mapping entry; a multiline key may not be an implicit key")
+                                    if (!b) return t.tag = u, t.anchor = p, !0;
+                                    ft(t, "can not read a block mapping entry; a multiline key may not be an implicit key")
                                 }
-                            } else 63 === s ? (y && (ye(e, f, d, h, g, null, a, l, c), h = g = m = null), b = !0, y = !0, r = !0) : y ? (y = !1, r = !0) : fe(e, "incomplete explicit mapping pair; a key node is missed; or followed by a non-tabulated empty line"), e.position += 1, s = i;
-                            if ((e.line === o || e.lineIndent > t) && (y && (a = e.line, l = e.lineStart, c = e.position), Ie(e, t, P, !0, r) && (y ? g = e.result : m = e.result), y || (ye(e, f, d, h, g, m, a, l, c), h = g = m = null), ve(e, !0, -1), s = e.input.charCodeAt(e.position)), (e.line === o || e.lineIndent > t) && 0 !== s) fe(e, "bad indentation of a mapping entry");
-                            else if (e.lineIndent < t) break
-                        }
-                        return y && ye(e, f, d, h, g, null, a, l, c), b && (e.tag = u, e.anchor = p, e.kind = "mapping", e.result = f), b
-                    }(e, h, d)) || function(e, t) {
-                        var n, i, r, o, a, l, c, s, u, p, f, d, h = !0,
-                            g = e.tag,
-                            m = e.anchor,
+                            } else 63 === s ? (y && (yt(t, f, d, h, g, null, a, c, l), h = g = m = null), b = !0, y = !0, r = !0) : y ? (y = !1, r = !0) : ft(t, "incomplete explicit mapping pair; a key node is missed; or followed by a non-tabulated empty line"), t.position += 1, s = i;
+                            if ((t.line === o || t.lineIndent > e) && (y && (a = t.line, c = t.lineStart, l = t.position), It(t, e, G, !0, r) && (y ? g = t.result : m = t.result), y || (yt(t, f, d, h, g, m, a, c, l), h = g = m = null), vt(t, !0, -1), s = t.input.charCodeAt(t.position)), (t.line === o || t.lineIndent > e) && 0 !== s) ft(t, "bad indentation of a mapping entry");
+                            else if (t.lineIndent < e) break
+                        }
+                        return y && yt(t, f, d, h, g, null, a, c, l), b && (t.tag = u, t.anchor = p, t.kind = "mapping", t.result = f), b
+                    }(t, h, d)) || function(t, e) {
+                        var n, i, r, o, a, c, l, s, u, p, f, d, h = !0,
+                            g = t.tag,
+                            m = t.anchor,
                             y = Object.create(null);
-                        if (91 === (d = e.input.charCodeAt(e.position))) a = 93, s = !1, o = [];
+                        if (91 === (d = t.input.charCodeAt(t.position))) a = 93, s = !1, o = [];
                         else {
                             if (123 !== d) return !1;
                             a = 125, s = !0, o = {}
                         }
-                        for (null !== e.anchor && (e.anchorMap[e.anchor] = o), d = e.input.charCodeAt(++e.position); 0 !== d;) {
-                            if (ve(e, !0, t), (d = e.input.charCodeAt(e.position)) === a) return e.position++, e.tag = g, e.anchor = m, e.kind = s ? "mapping" : "sequence", e.result = o, !0;
-                            h ? 44 === d && fe(e, "expected the node content, but found ','") : fe(e, "missed comma between flow collection entries"), f = null, l = c = !1, 63 === d && ne(e.input.charCodeAt(e.position + 1)) && (l = c = !0, e.position++, ve(e, !0, t)), n = e.line, i = e.lineStart, r = e.position, Ie(e, t, B, !1, !0), p = e.tag, u = e.result, ve(e, !0, t), d = e.input.charCodeAt(e.position), !c && e.line !== n || 58 !== d || (l = !0, d = e.input.charCodeAt(++e.position), ve(e, !0, t), Ie(e, t, B, !1, !0), f = e.result), s ? ye(e, o, y, p, u, f, n, i, r) : l ? o.push(ye(e, null, y, p, u, f, n, i, r)) : o.push(u), ve(e, !0, t), 44 === (d = e.input.charCodeAt(e.position)) ? (h = !0, d = e.input.charCodeAt(++e.position)) : h = !1
-                        }
-                        fe(e, "unexpected end of the stream within a flow collection")
-                    }(e, d) ? y = !0 : (l && function(e, t) {
-                        var n, i, o, a, l, c = W,
+                        for (null !== t.anchor && (t.anchorMap[t.anchor] = o), d = t.input.charCodeAt(++t.position); 0 !== d;) {
+                            if (vt(t, !0, e), (d = t.input.charCodeAt(t.position)) === a) return t.position++, t.tag = g, t.anchor = m, t.kind = s ? "mapping" : "sequence", t.result = o, !0;
+                            h ? 44 === d && ft(t, "expected the node content, but found ','") : ft(t, "missed comma between flow collection entries"), f = null, c = l = !1, 63 === d && nt(t.input.charCodeAt(t.position + 1)) && (c = l = !0, t.position++, vt(t, !0, e)), n = t.line, i = t.lineStart, r = t.position, It(t, e, R, !1, !0), p = t.tag, u = t.result, vt(t, !0, e), d = t.input.charCodeAt(t.position), !l && t.line !== n || 58 !== d || (c = !0, d = t.input.charCodeAt(++t.position), vt(t, !0, e), It(t, e, R, !1, !0), f = t.result), s ? yt(t, o, y, p, u, f, n, i, r) : c ? o.push(yt(t, null, y, p, u, f, n, i, r)) : o.push(u), vt(t, !0, e), 44 === (d = t.input.charCodeAt(t.position)) ? (h = !0, d = t.input.charCodeAt(++t.position)) : h = !1
+                        }
+                        ft(t, "unexpected end of the stream within a flow collection")
+                    }(t, d) ? y = !0 : (c && function(t, e) {
+                        var n, i, o, a, c, l = V,
                             s = !1,
                             u = !1,
-                            p = t,
+                            p = e,
                             f = 0,
                             d = !1;
-                        if (124 === (a = e.input.charCodeAt(e.position))) i = !1;
+                        if (124 === (a = t.input.charCodeAt(t.position))) i = !1;
                         else {
                             if (62 !== a) return !1;
                             i = !0
                         }
-                        for (e.kind = "scalar", e.result = ""; 0 !== a;)
-                            if (43 === (a = e.input.charCodeAt(++e.position)) || 45 === a) W === c ? c = 43 === a ? V : G : fe(e, "repeat of a chomping mode identifier");
+                        for (t.kind = "scalar", t.result = ""; 0 !== a;)
+                            if (43 === (a = t.input.charCodeAt(++t.position)) || 45 === a) V === l ? l = 43 === a ? W : Z : ft(t, "repeat of a chomping mode identifier");
                             else {
-                                if (!((o = 48 <= (l = a) && l <= 57 ? l - 48 : -1) >= 0)) break;
-                                0 === o ? fe(e, "bad explicit indentation width of a block scalar; it cannot be less than one") : u ? fe(e, "repeat of an indentation width identifier") : (p = t + o - 1, u = !0)
-                            } if (te(a)) {
+                                if (!((o = 48 <= (c = a) && c <= 57 ? c - 48 : -1) >= 0)) break;
+                                0 === o ? ft(t, "bad explicit indentation width of a block scalar; it cannot be less than one") : u ? ft(t, "repeat of an indentation width identifier") : (p = e + o - 1, u = !0)
+                            } if (et(a)) {
                             do {
-                                a = e.input.charCodeAt(++e.position)
-                            } while (te(a));
+                                a = t.input.charCodeAt(++t.position)
+                            } while (et(a));
                             if (35 === a)
                                 do {
-                                    a = e.input.charCodeAt(++e.position)
-                                } while (!ee(a) && 0 !== a)
+                                    a = t.input.charCodeAt(++t.position)
+                                } while (!tt(a) && 0 !== a)
                         }
                         for (; 0 !== a;) {
-                            for (be(e), e.lineIndent = 0, a = e.input.charCodeAt(e.position);
-                                (!u || e.lineIndent < p) && 32 === a;) e.lineIndent++, a = e.input.charCodeAt(++e.position);
-                            if (!u && e.lineIndent > p && (p = e.lineIndent), ee(a)) f++;
+                            for (bt(t), t.lineIndent = 0, a = t.input.charCodeAt(t.position);
+                                (!u || t.lineIndent < p) && 32 === a;) t.lineIndent++, a = t.input.charCodeAt(++t.position);
+                            if (!u && t.lineIndent > p && (p = t.lineIndent), tt(a)) f++;
                             else {
-                                if (e.lineIndent < p) {
-                                    c === V ? e.result += r.repeat("\n", s ? 1 + f : f) : c === W && s && (e.result += "\n");
+                                if (t.lineIndent < p) {
+                                    l === W ? t.result += r.repeat("\n", s ? 1 + f : f) : l === V && s && (t.result += "\n");
                                     break
                                 }
-                                for (i ? te(a) ? (d = !0, e.result += r.repeat("\n", s ? 1 + f : f)) : d ? (d = !1, e.result += r.repeat("\n", f + 1)) : 0 === f ? s && (e.result += " ") : e.result += r.repeat("\n", f) : e.result += r.repeat("\n", s ? 1 + f : f), s = !0, u = !0, f = 0, n = e.position; !ee(a) && 0 !== a;) a = e.input.charCodeAt(++e.position);
-                                ge(e, n, e.position, !1)
+                                for (i ? et(a) ? (d = !0, t.result += r.repeat("\n", s ? 1 + f : f)) : d ? (d = !1, t.result += r.repeat("\n", f + 1)) : 0 === f ? s && (t.result += " ") : t.result += r.repeat("\n", f) : t.result += r.repeat("\n", s ? 1 + f : f), s = !0, u = !0, f = 0, n = t.position; !tt(a) && 0 !== a;) a = t.input.charCodeAt(++t.position);
+                                gt(t, n, t.position, !1)
                             }
                         }
                         return !0
-                    }(e, d) || function(e, t) {
+                    }(t, d) || function(t, e) {
                         var n, i, r;
-                        if (39 !== (n = e.input.charCodeAt(e.position))) return !1;
-                        for (e.kind = "scalar", e.result = "", e.position++, i = r = e.position; 0 !== (n = e.input.charCodeAt(e.position));)
+                        if (39 !== (n = t.input.charCodeAt(t.position))) return !1;
+                        for (t.kind = "scalar", t.result = "", t.position++, i = r = t.position; 0 !== (n = t.input.charCodeAt(t.position));)
                             if (39 === n) {
-                                if (ge(e, i, e.position, !0), 39 !== (n = e.input.charCodeAt(++e.position))) return !0;
-                                i = e.position, e.position++, r = e.position
-                            } else ee(n) ? (ge(e, i, r, !0), we(e, ve(e, !1, t)), i = r = e.position) : e.position === e.lineStart && Ae(e) ? fe(e, "unexpected end of the document within a single quoted scalar") : (e.position++, r = e.position);
-                        fe(e, "unexpected end of the stream within a single quoted scalar")
-                    }(e, d) || function(e, t) {
-                        var n, i, r, o, a, l, c;
-                        if (34 !== (l = e.input.charCodeAt(e.position))) return !1;
-                        for (e.kind = "scalar", e.result = "", e.position++, n = i = e.position; 0 !== (l = e.input.charCodeAt(e.position));) {
-                            if (34 === l) return ge(e, n, e.position, !0), e.position++, !0;
-                            if (92 === l) {
-                                if (ge(e, n, e.position, !0), ee(l = e.input.charCodeAt(++e.position))) ve(e, !1, t);
-                                else if (l < 256 && le[l]) e.result += ce[l], e.position++;
-                                else if ((a = 120 === (c = l) ? 2 : 117 === c ? 4 : 85 === c ? 8 : 0) > 0) {
-                                    for (r = a, o = 0; r > 0; r--)(a = re(l = e.input.charCodeAt(++e.position))) >= 0 ? o = (o << 4) + a : fe(e, "expected hexadecimal character");
-                                    e.result += ae(o), e.position++
-                                } else fe(e, "unknown escape sequence");
-                                n = i = e.position
-                            } else ee(l) ? (ge(e, n, i, !0), we(e, ve(e, !1, t)), n = i = e.position) : e.position === e.lineStart && Ae(e) ? fe(e, "unexpected end of the document within a double quoted scalar") : (e.position++, i = e.position)
-                        }
-                        fe(e, "unexpected end of the stream within a double quoted scalar")
-                    }(e, d) ? y = !0 : function(e) {
-                        var t, n, i;
-                        if (42 !== (i = e.input.charCodeAt(e.position))) return !1;
-                        for (i = e.input.charCodeAt(++e.position), t = e.position; 0 !== i && !ne(i) && !ie(i);) i = e.input.charCodeAt(++e.position);
-                        return e.position === t && fe(e, "name of an alias node must contain at least one character"), n = e.input.slice(t, e.position), R.call(e.anchorMap, n) || fe(e, 'unidentified alias "' + n + '"'), e.result = e.anchorMap[n], ve(e, !0, -1), !0
-                    }(e) ? (y = !0, null === e.tag && null === e.anchor || fe(e, "alias node should not have any properties")) : function(e, t, n) {
-                        var i, r, o, a, l, c, s, u, p = e.kind,
-                            f = e.result;
-                        if (ne(u = e.input.charCodeAt(e.position)) || ie(u) || 35 === u || 38 === u || 42 === u || 33 === u || 124 === u || 62 === u || 39 === u || 34 === u || 37 === u || 64 === u || 96 === u) return !1;
-                        if ((63 === u || 45 === u) && (ne(i = e.input.charCodeAt(e.position + 1)) || n && ie(i))) return !1;
-                        for (e.kind = "scalar", e.result = "", r = o = e.position, a = !1; 0 !== u;) {
+                                if (gt(t, i, t.position, !0), 39 !== (n = t.input.charCodeAt(++t.position))) return !0;
+                                i = t.position, t.position++, r = t.position
+                            } else tt(n) ? (gt(t, i, r, !0), kt(t, vt(t, !1, e)), i = r = t.position) : t.position === t.lineStart && At(t) ? ft(t, "unexpected end of the document within a single quoted scalar") : (t.position++, r = t.position);
+                        ft(t, "unexpected end of the stream within a single quoted scalar")
+                    }(t, d) || function(t, e) {
+                        var n, i, r, o, a, c, l;
+                        if (34 !== (c = t.input.charCodeAt(t.position))) return !1;
+                        for (t.kind = "scalar", t.result = "", t.position++, n = i = t.position; 0 !== (c = t.input.charCodeAt(t.position));) {
+                            if (34 === c) return gt(t, n, t.position, !0), t.position++, !0;
+                            if (92 === c) {
+                                if (gt(t, n, t.position, !0), tt(c = t.input.charCodeAt(++t.position))) vt(t, !1, e);
+                                else if (c < 256 && ct[c]) t.result += lt[c], t.position++;
+                                else if ((a = 120 === (l = c) ? 2 : 117 === l ? 4 : 85 === l ? 8 : 0) > 0) {
+                                    for (r = a, o = 0; r > 0; r--)(a = rt(c = t.input.charCodeAt(++t.position))) >= 0 ? o = (o << 4) + a : ft(t, "expected hexadecimal character");
+                                    t.result += at(o), t.position++
+                                } else ft(t, "unknown escape sequence");
+                                n = i = t.position
+                            } else tt(c) ? (gt(t, n, i, !0), kt(t, vt(t, !1, e)), n = i = t.position) : t.position === t.lineStart && At(t) ? ft(t, "unexpected end of the document within a double quoted scalar") : (t.position++, i = t.position)
+                        }
+                        ft(t, "unexpected end of the stream within a double quoted scalar")
+                    }(t, d) ? y = !0 : function(t) {
+                        var e, n, i;
+                        if (42 !== (i = t.input.charCodeAt(t.position))) return !1;
+                        for (i = t.input.charCodeAt(++t.position), e = t.position; 0 !== i && !nt(i) && !it(i);) i = t.input.charCodeAt(++t.position);
+                        return t.position === e && ft(t, "name of an alias node must contain at least one character"), n = t.input.slice(e, t.position), B.call(t.anchorMap, n) || ft(t, 'unidentified alias "' + n + '"'), t.result = t.anchorMap[n], vt(t, !0, -1), !0
+                    }(t) ? (y = !0, null === t.tag && null === t.anchor || ft(t, "alias node should not have any properties")) : function(t, e, n) {
+                        var i, r, o, a, c, l, s, u, p = t.kind,
+                            f = t.result;
+                        if (nt(u = t.input.charCodeAt(t.position)) || it(u) || 35 === u || 38 === u || 42 === u || 33 === u || 124 === u || 62 === u || 39 === u || 34 === u || 37 === u || 64 === u || 96 === u) return !1;
+                        if ((63 === u || 45 === u) && (nt(i = t.input.charCodeAt(t.position + 1)) || n && it(i))) return !1;
+                        for (t.kind = "scalar", t.result = "", r = o = t.position, a = !1; 0 !== u;) {
                             if (58 === u) {
-                                if (ne(i = e.input.charCodeAt(e.position + 1)) || n && ie(i)) break
+                                if (nt(i = t.input.charCodeAt(t.position + 1)) || n && it(i)) break
                             } else if (35 === u) {
-                                if (ne(e.input.charCodeAt(e.position - 1))) break
+                                if (nt(t.input.charCodeAt(t.position - 1))) break
                             } else {
-                                if (e.position === e.lineStart && Ae(e) || n && ie(u)) break;
-                                if (ee(u)) {
-                                    if (l = e.line, c = e.lineStart, s = e.lineIndent, ve(e, !1, -1), e.lineIndent >= t) {
-                                        a = !0, u = e.input.charCodeAt(e.position);
+                                if (t.position === t.lineStart && At(t) || n && it(u)) break;
+                                if (tt(u)) {
+                                    if (c = t.line, l = t.lineStart, s = t.lineIndent, vt(t, !1, -1), t.lineIndent >= e) {
+                                        a = !0, u = t.input.charCodeAt(t.position);
                                         continue
                                     }
-                                    e.position = o, e.line = l, e.lineStart = c, e.lineIndent = s;
+                                    t.position = o, t.line = c, t.lineStart = l, t.lineIndent = s;
                                     break
                                 }
                             }
-                            a && (ge(e, r, o, !1), we(e, e.line - l), r = o = e.position, a = !1), te(u) || (o = e.position + 1), u = e.input.charCodeAt(++e.position)
+                            a && (gt(t, r, o, !1), kt(t, t.line - c), r = o = t.position, a = !1), et(u) || (o = t.position + 1), u = t.input.charCodeAt(++t.position)
                         }
-                        return ge(e, r, o, !1), !!e.result || (e.kind = p, e.result = f, !1)
-                    }(e, d, B === n) && (y = !0, null === e.tag && (e.tag = "?")), null !== e.anchor && (e.anchorMap[e.anchor] = e.result)) : 0 === g && (y = c && ke(e, h))), null === e.tag) null !== e.anchor && (e.anchorMap[e.anchor] = e.result);
-                else if ("?" === e.tag) {
-                    for (null !== e.result && "scalar" !== e.kind && fe(e, 'unacceptable node kind for !<?> tag; it should be "scalar", not "' + e.kind + '"'), s = 0, u = e.implicitTypes.length; s < u; s += 1)
-                        if ((f = e.implicitTypes[s]).resolve(e.result)) {
-                            e.result = f.construct(e.result), e.tag = f.tag, null !== e.anchor && (e.anchorMap[e.anchor] = e.result);
+                        return gt(t, r, o, !1), !!t.result || (t.kind = p, t.result = f, !1)
+                    }(t, d, R === n) && (y = !0, null === t.tag && (t.tag = "?")), null !== t.anchor && (t.anchorMap[t.anchor] = t.result)) : 0 === g && (y = l && Ct(t, h))), null === t.tag) null !== t.anchor && (t.anchorMap[t.anchor] = t.result);
+                else if ("?" === t.tag) {
+                    for (null !== t.result && "scalar" !== t.kind && ft(t, 'unacceptable node kind for !<?> tag; it should be "scalar", not "' + t.kind + '"'), s = 0, u = t.implicitTypes.length; s < u; s += 1)
+                        if ((f = t.implicitTypes[s]).resolve(t.result)) {
+                            t.result = f.construct(t.result), t.tag = f.tag, null !== t.anchor && (t.anchorMap[t.anchor] = t.result);
                             break
                         }
-                } else if ("!" !== e.tag) {
-                    if (R.call(e.typeMap[e.kind || "fallback"], e.tag)) f = e.typeMap[e.kind || "fallback"][e.tag];
+                } else if ("!" !== t.tag) {
+                    if (B.call(t.typeMap[t.kind || "fallback"], t.tag)) f = t.typeMap[t.kind || "fallback"][t.tag];
                     else
-                        for (f = null, s = 0, u = (p = e.typeMap.multi[e.kind || "fallback"]).length; s < u; s += 1)
-                            if (e.tag.slice(0, p[s].tag.length) === p[s].tag) {
+                        for (f = null, s = 0, u = (p = t.typeMap.multi[t.kind || "fallback"]).length; s < u; s += 1)
+                            if (t.tag.slice(0, p[s].tag.length) === p[s].tag) {
                                 f = p[s];
                                 break
-                            } f || fe(e, "unknown tag !<" + e.tag + ">"), null !== e.result && f.kind !== e.kind && fe(e, "unacceptable node kind for !<" + e.tag + '> tag; it should be "' + f.kind + '", not "' + e.kind + '"'), f.resolve(e.result, e.tag) ? (e.result = f.construct(e.result, e.tag), null !== e.anchor && (e.anchorMap[e.anchor] = e.result)) : fe(e, "cannot resolve a node with !<" + e.tag + "> explicit tag")
+                            } f || ft(t, "unknown tag !<" + t.tag + ">"), null !== t.result && f.kind !== t.kind && ft(t, "unacceptable node kind for !<" + t.tag + '> tag; it should be "' + f.kind + '", not "' + t.kind + '"'), f.resolve(t.result, t.tag) ? (t.result = f.construct(t.result, t.tag), null !== t.anchor && (t.anchorMap[t.anchor] = t.result)) : ft(t, "cannot resolve a node with !<" + t.tag + "> explicit tag")
                 }
-                return null !== e.listener && e.listener("close", e), null !== e.tag || null !== e.anchor || y
+                return null !== t.listener && t.listener("close", t), null !== t.tag || null !== t.anchor || y
             }
 
-            function je(e) {
-                var t, n, i, r, o = e.position,
+            function St(t) {
+                var e, n, i, r, o = t.position,
                     a = !1;
-                for (e.version = null, e.checkLineBreaks = e.legacy, e.tagMap = Object.create(null), e.anchorMap = Object.create(null); 0 !== (r = e.input.charCodeAt(e.position)) && (ve(e, !0, -1), r = e.input.charCodeAt(e.position), !(e.lineIndent > 0 || 37 !== r));) {
-                    for (a = !0, r = e.input.charCodeAt(++e.position), t = e.position; 0 !== r && !ne(r);) r = e.input.charCodeAt(++e.position);
-                    for (i = [], (n = e.input.slice(t, e.position)).length < 1 && fe(e, "directive name must not be less than one character in length"); 0 !== r;) {
-                        for (; te(r);) r = e.input.charCodeAt(++e.position);
+                for (t.version = null, t.checkLineBreaks = t.legacy, t.tagMap = Object.create(null), t.anchorMap = Object.create(null); 0 !== (r = t.input.charCodeAt(t.position)) && (vt(t, !0, -1), r = t.input.charCodeAt(t.position), !(t.lineIndent > 0 || 37 !== r));) {
+                    for (a = !0, r = t.input.charCodeAt(++t.position), e = t.position; 0 !== r && !nt(r);) r = t.input.charCodeAt(++t.position);
+                    for (i = [], (n = t.input.slice(e, t.position)).length < 1 && ft(t, "directive name must not be less than one character in length"); 0 !== r;) {
+                        for (; et(r);) r = t.input.charCodeAt(++t.position);
                         if (35 === r) {
                             do {
-                                r = e.input.charCodeAt(++e.position)
-                            } while (0 !== r && !ee(r));
+                                r = t.input.charCodeAt(++t.position)
+                            } while (0 !== r && !tt(r));
                             break
                         }
-                        if (ee(r)) break;
-                        for (t = e.position; 0 !== r && !ne(r);) r = e.input.charCodeAt(++e.position);
-                        i.push(e.input.slice(t, e.position))
+                        if (tt(r)) break;
+                        for (e = t.position; 0 !== r && !nt(r);) r = t.input.charCodeAt(++t.position);
+                        i.push(t.input.slice(e, t.position))
                     }
-                    0 !== r && be(e), R.call(he, n) ? he[n](e, n, i) : de(e, 'unknown document directive "' + n + '"')
+                    0 !== r && bt(t), B.call(ht, n) ? ht[n](t, n, i) : dt(t, 'unknown document directive "' + n + '"')
                 }
-                ve(e, !0, -1), 0 === e.lineIndent && 45 === e.input.charCodeAt(e.position) && 45 === e.input.charCodeAt(e.position + 1) && 45 === e.input.charCodeAt(e.position + 2) ? (e.position += 3, ve(e, !0, -1)) : a && fe(e, "directives end mark is expected"), Ie(e, e.lineIndent - 1, P, !1, !0), ve(e, !0, -1), e.checkLineBreaks && Q.test(e.input.slice(o, e.position)) && de(e, "non-ASCII line breaks are interpreted as content"), e.documents.push(e.result), e.position === e.lineStart && Ae(e) ? 46 === e.input.charCodeAt(e.position) && (e.position += 3, ve(e, !0, -1)) : e.position < e.length - 1 && fe(e, "end of the stream or a document separator is expected")
+                vt(t, !0, -1), 0 === t.lineIndent && 45 === t.input.charCodeAt(t.position) && 45 === t.input.charCodeAt(t.position + 1) && 45 === t.input.charCodeAt(t.position + 2) ? (t.position += 3, vt(t, !0, -1)) : a && ft(t, "directives end mark is expected"), It(t, t.lineIndent - 1, G, !1, !0), vt(t, !0, -1), t.checkLineBreaks && H.test(t.input.slice(o, t.position)) && dt(t, "non-ASCII line breaks are interpreted as content"), t.documents.push(t.result), t.position === t.lineStart && At(t) ? 46 === t.input.charCodeAt(t.position) && (t.position += 3, vt(t, !0, -1)) : t.position < t.length - 1 && ft(t, "end of the stream or a document separator is expected")
             }
 
-            function Oe(e, t) {
-                t = t || {}, 0 !== (e = String(e)).length && (10 !== e.charCodeAt(e.length - 1) && 13 !== e.charCodeAt(e.length - 1) && (e += "\n"), 65279 === e.charCodeAt(0) && (e = e.slice(1)));
-                var n = new ue(e, t),
-                    i = e.indexOf("\0");
-                for (-1 !== i && (n.position = i, fe(n, "null byte is not allowed in input")), n.input += "\0"; 32 === n.input.charCodeAt(n.position);) n.lineIndent += 1, n.position += 1;
-                for (; n.position < n.length - 1;) je(n);
+            function jt(t, e) {
+                e = e || {}, 0 !== (t = String(t)).length && (10 !== t.charCodeAt(t.length - 1) && 13 !== t.charCodeAt(t.length - 1) && (t += "\n"), 65279 === t.charCodeAt(0) && (t = t.slice(1)));
+                var n = new ut(t, e),
+                    i = t.indexOf("\0");
+                for (-1 !== i && (n.position = i, ft(n, "null byte is not allowed in input")), n.input += "\0"; 32 === n.input.charCodeAt(n.position);) n.lineIndent += 1, n.position += 1;
+                for (; n.position < n.length - 1;) St(n);
                 return n.documents
             }
-            var Se = function(e, t) {
-                    var n = Oe(e, t);
-                    if (0 !== n.length) {
-                        if (1 === n.length) return n[0];
-                        throw new l("expected a single document in the stream, but found more")
-                    }
-                },
-                Te = Object.prototype.toString,
-                Ne = Object.prototype.hasOwnProperty,
-                Fe = 65279,
-                Me = 9,
-                Le = 10,
-                Ee = 13,
-                _e = 32,
-                qe = 33,
-                De = 34,
-                Ue = 35,
-                Ye = 37,
-                Re = 38,
-                Be = 39,
-                $e = 42,
-                Ke = 44,
-                Pe = 45,
-                We = 58,
-                Ge = 61,
-                Ve = 62,
-                Ze = 63,
-                Qe = 64,
-                ze = 91,
-                He = 93,
-                Je = 96,
-                Xe = 123,
-                et = 124,
-                tt = 125,
-                nt = {
-                    0: "\\0",
-                    7: "\\a",
-                    8: "\\b",
-                    9: "\\t",
-                    10: "\\n",
-                    11: "\\v",
-                    12: "\\f",
-                    13: "\\r",
-                    27: "\\e",
-                    34: '\\"',
-                    92: "\\\\",
-                    133: "\\N",
-                    160: "\\_",
-                    8232: "\\L",
-                    8233: "\\P"
-                },
-                it = ["y", "Y", "yes", "Yes", "YES", "on", "On", "ON", "n", "N", "no", "No", "NO", "off", "Off", "OFF"],
-                rt = /^[-+]?[0-9_]+(?::[0-9_]+)+(?:\.[0-9_]*)?$/;
-
-            function ot(e) {
-                var t, n, i;
-                if (t = e.toString(16).toUpperCase(), e <= 255) n = "x", i = 2;
-                else if (e <= 65535) n = "u", i = 4;
-                else {
-                    if (!(e <= 4294967295)) throw new l("code point within a string may not be greater than 0xFFFFFFFF");
-                    n = "U", i = 8
+            var Tt = function(t, e) {
+                var n = jt(t, e);
+                if (0 !== n.length) {
+                    if (1 === n.length) return n[0];
+                    throw new c("expected a single document in the stream, but found more")
                 }
-                return "\\" + n + r.repeat("0", i - t.length) + t
-            }
-            var at = 2;
-
-            function lt(e) {
-                this.schema = e.schema || Y, this.indent = Math.max(1, e.indent || 2), this.noArrayIndent = e.noArrayIndent || !1, this.skipInvalid = e.skipInvalid || !1, this.flowLevel = r.isNothing(e.flowLevel) ? -1 : e.flowLevel, this.styleMap = function(e, t) {
-                    var n, i, r, o, a, l, c;
-                    if (null === t) return {};
-                    for (n = {}, r = 0, o = (i = Object.keys(t)).length; r < o; r += 1) a = i[r], l = String(t[a]), "!!" === a.slice(0, 2) && (a = "tag:yaml.org,2002:" + a.slice(2)), (c = e.compiledTypeMap.fallback[a]) && Ne.call(c.styleAliases, l) && (l = c.styleAliases[l]), n[a] = l;
-                    return n
-                }(this.schema, e.styles || null), this.sortKeys = e.sortKeys || !1, this.lineWidth = e.lineWidth || 80, this.noRefs = e.noRefs || !1, this.noCompatMode = e.noCompatMode || !1, this.condenseFlow = e.condenseFlow || !1, this.quotingType = '"' === e.quotingType ? at : 1, this.forceQuotes = e.forceQuotes || !1, this.replacer = "function" == typeof e.replacer ? e.replacer : null, this.implicitTypes = this.schema.compiledImplicit, this.explicitTypes = this.schema.compiledExplicit, this.tag = null, this.result = "", this.duplicates = [], this.usedDuplicates = null
-            }
-
-            function ct(e, t) {
-                for (var n, i = r.repeat(" ", t), o = 0, a = -1, l = "", c = e.length; o < c;) - 1 === (a = e.indexOf("\n", o)) ? (n = e.slice(o), o = c) : (n = e.slice(o, a + 1), o = a + 1), n.length && "\n" !== n && (l += i), l += n;
-                return l
-            }
-
-            function st(e, t) {
-                return "\n" + r.repeat(" ", e.indent * t)
-            }
-
-            function ut(e) {
-                return e === _e || e === Me
-            }
-
-            function pt(e) {
-                return 32 <= e && e <= 126 || 161 <= e && e <= 55295 && 8232 !== e && 8233 !== e || 57344 <= e && e <= 65533 && e !== Fe || 65536 <= e && e <= 1114111
-            }
-
-            function ft(e) {
-                return pt(e) && e !== Fe && e !== Ee && e !== Le
-            }
-
-            function dt(e, t, n) {
-                var i = ft(e),
-                    r = i && !ut(e);
-                return (n ? i : i && e !== Ke && e !== ze && e !== He && e !== Xe && e !== tt) && e !== Ue && !(t === We && !r) || ft(t) && !ut(t) && e === Ue || t === We && r
-            }
-
-            function ht(e, t) {
-                var n, i = e.charCodeAt(t);
-                return i >= 55296 && i <= 56319 && t + 1 < e.length && (n = e.charCodeAt(t + 1)) >= 56320 && n <= 57343 ? 1024 * (i - 55296) + n - 56320 + 65536 : i
-            }
-
-            function gt(e) {
-                return /^\n* /.test(e)
-            }
-            var mt = 1,
-                yt = 2,
-                bt = 3,
-                vt = 4,
-                At = 5;
-
-            function wt(e, t, n, i, r) {
-                e.dump = function() {
-                    if (0 === t.length) return e.quotingType === at ? '""' : "''";
-                    if (!e.noCompatMode && (-1 !== it.indexOf(t) || rt.test(t))) return e.quotingType === at ? '"' + t + '"' : "'" + t + "'";
-                    var o = e.indent * Math.max(1, n),
-                        a = -1 === e.lineWidth ? -1 : Math.max(Math.min(e.lineWidth, 40), e.lineWidth - o),
-                        c = i || e.flowLevel > -1 && n >= e.flowLevel;
-                    switch (function(e, t, n, i, r, o, a, l) {
-                            var c, s, u = 0,
-                                p = null,
-                                f = !1,
-                                d = !1,
-                                h = -1 !== i,
-                                g = -1,
-                                m = pt(s = ht(e, 0)) && s !== Fe && !ut(s) && s !== Pe && s !== Ze && s !== We && s !== Ke && s !== ze && s !== He && s !== Xe && s !== tt && s !== Ue && s !== Re && s !== $e && s !== qe && s !== et && s !== Ge && s !== Ve && s !== Be && s !== De && s !== Ye && s !== Qe && s !== Je && function(e) {
-                                    return !ut(e) && e !== We
-                                }(ht(e, e.length - 1));
-                            if (t || a)
-                                for (c = 0; c < e.length; u >= 65536 ? c += 2 : c++) {
-                                    if (!pt(u = ht(e, c))) return At;
-                                    m = m && dt(u, p, l), p = u
-                                } else {
-                                    for (c = 0; c < e.length; u >= 65536 ? c += 2 : c++) {
-                                        if ((u = ht(e, c)) === Le) f = !0, h && (d = d || c - g - 1 > i && " " !== e[g + 1], g = c);
-                                        else if (!pt(u)) return At;
-                                        m = m && dt(u, p, l), p = u
-                                    }
-                                    d = d || h && c - g - 1 > i && " " !== e[g + 1]
-                                }
-                            return f || d ? n > 9 && gt(e) ? At : a ? o === at ? At : yt : d ? vt : bt : !m || a || r(e) ? o === at ? At : yt : mt
-                        }(t, c, e.indent, a, (function(t) {
-                            return function(e, t) {
-                                var n, i;
-                                for (n = 0, i = e.implicitTypes.length; n < i; n += 1)
-                                    if (e.implicitTypes[n].resolve(t)) return !0;
-                                return !1
-                            }(e, t)
-                        }), e.quotingType, e.forceQuotes && !i, r)) {
-                        case mt:
-                            return t;
-                        case yt:
-                            return "'" + t.replace(/'/g, "''") + "'";
-                        case bt:
-                            return "|" + kt(t, e.indent) + xt(ct(t, o));
-                        case vt:
-                            return ">" + kt(t, e.indent) + xt(ct(function(e, t) {
-                                for (var n, i, r, o = /(\n+)([^\n]*)/g, a = (r = -1 !== (r = e.indexOf("\n")) ? r : e.length, o.lastIndex = r, Ct(e.slice(0, r), t)), l = "\n" === e[0] || " " === e[0]; i = o.exec(e);) {
-                                    var c = i[1],
-                                        s = i[2];
-                                    n = " " === s[0], a += c + (l || n || "" === s ? "" : "\n") + Ct(s, t), l = n
-                                }
-                                return a
-                            }(t, a), o));
-                        case At:
-                            return '"' + function(e) {
-                                for (var t, n = "", i = 0, r = 0; r < e.length; i >= 65536 ? r += 2 : r++) i = ht(e, r), !(t = nt[i]) && pt(i) ? (n += e[r], i >= 65536 && (n += e[r + 1])) : n += t || ot(i);
-                                return n
-                            }(t) + '"';
-                        default:
-                            throw new l("impossible error: invalid scalar style")
-                    }
-                }()
-            }
-
-            function kt(e, t) {
-                var n = gt(e) ? String(t) : "",
-                    i = "\n" === e[e.length - 1];
-                return n + (!i || "\n" !== e[e.length - 2] && "\n" !== e ? i ? "" : "-" : "+") + "\n"
-            }
-
-            function xt(e) {
-                return "\n" === e[e.length - 1] ? e.slice(0, -1) : e
-            }
-
-            function Ct(e, t) {
-                if ("" === e || " " === e[0]) return e;
-                for (var n, i, r = / [^ ]/g, o = 0, a = 0, l = 0, c = ""; n = r.exec(e);)(l = n.index) - o > t && (i = a > o ? a : l, c += "\n" + e.slice(o, i), o = i + 1), a = l;
-                return c += "\n", e.length - o > t && a > o ? c += e.slice(o, a) + "\n" + e.slice(a + 1) : c += e.slice(o), c.slice(1)
-            }
-
-            function It(e, t, n, i) {
-                var r, o, a, l = "",
-                    c = e.tag;
-                for (r = 0, o = n.length; r < o; r += 1) a = n[r], e.replacer && (a = e.replacer.call(n, String(r), a)), (Ot(e, t + 1, a, !0, !0, !1, !0) || void 0 === a && Ot(e, t + 1, null, !0, !0, !1, !0)) && (i && "" === l || (l += st(e, t)), e.dump && Le === e.dump.charCodeAt(0) ? l += "-" : l += "- ", l += e.dump);
-                e.tag = c, e.dump = l || "[]"
-            }
-
-            function jt(e, t, n) {
-                var i, r, o, a, c, s;
-                for (o = 0, a = (r = n ? e.explicitTypes : e.implicitTypes).length; o < a; o += 1)
-                    if (((c = r[o]).instanceOf || c.predicate) && (!c.instanceOf || "object" == typeof t && t instanceof c.instanceOf) && (!c.predicate || c.predicate(t))) {
-                        if (n ? c.multi && c.representName ? e.tag = c.representName(t) : e.tag = c.tag : e.tag = "?", c.represent) {
-                            if (s = e.styleMap[c.tag] || c.defaultStyle, "[object Function]" === Te.call(c.represent)) i = c.represent(t, s);
-                            else {
-                                if (!Ne.call(c.represent, s)) throw new l("!<" + c.tag + '> tag resolver accepts not "' + s + '" style');
-                                i = c.represent[s](t, s)
-                            }
-                            e.dump = i
-                        }
-                        return !0
-                    } return !1
-            }
-
-            function Ot(e, t, n, i, r, o, a) {
-                e.tag = null, e.dump = n, jt(e, n, !1) || jt(e, n, !0);
-                var c, s = Te.call(e.dump),
-                    u = i;
-                i && (i = e.flowLevel < 0 || e.flowLevel > t);
-                var p, f, d = "[object Object]" === s || "[object Array]" === s;
-                if (d && (f = -1 !== (p = e.duplicates.indexOf(n))), (null !== e.tag && "?" !== e.tag || f || 2 !== e.indent && t > 0) && (r = !1), f && e.usedDuplicates[p]) e.dump = "*ref_" + p;
-                else {
-                    if (d && f && !e.usedDuplicates[p] && (e.usedDuplicates[p] = !0), "[object Object]" === s) i && 0 !== Object.keys(e.dump).length ? (function(e, t, n, i) {
-                        var r, o, a, c, s, u, p = "",
-                            f = e.tag,
-                            d = Object.keys(n);
-                        if (!0 === e.sortKeys) d.sort();
-                        else if ("function" == typeof e.sortKeys) d.sort(e.sortKeys);
-                        else if (e.sortKeys) throw new l("sortKeys must be a boolean or a function");
-                        for (r = 0, o = d.length; r < o; r += 1) u = "", i && "" === p || (u += st(e, t)), c = n[a = d[r]], e.replacer && (c = e.replacer.call(n, a, c)), Ot(e, t + 1, a, !0, !0, !0) && ((s = null !== e.tag && "?" !== e.tag || e.dump && e.dump.length > 1024) && (e.dump && Le === e.dump.charCodeAt(0) ? u += "?" : u += "? "), u += e.dump, s && (u += st(e, t)), Ot(e, t + 1, c, !0, s) && (e.dump && Le === e.dump.charCodeAt(0) ? u += ":" : u += ": ", p += u += e.dump));
-                        e.tag = f, e.dump = p || "{}"
-                    }(e, t, e.dump, r), f && (e.dump = "&ref_" + p + e.dump)) : (function(e, t, n) {
-                        var i, r, o, a, l, c = "",
-                            s = e.tag,
-                            u = Object.keys(n);
-                        for (i = 0, r = u.length; i < r; i += 1) l = "", "" !== c && (l += ", "), e.condenseFlow && (l += '"'), a = n[o = u[i]], e.replacer && (a = e.replacer.call(n, o, a)), Ot(e, t, o, !1, !1) && (e.dump.length > 1024 && (l += "? "), l += e.dump + (e.condenseFlow ? '"' : "") + ":" + (e.condenseFlow ? "" : " "), Ot(e, t, a, !1, !1) && (c += l += e.dump));
-                        e.tag = s, e.dump = "{" + c + "}"
-                    }(e, t, e.dump), f && (e.dump = "&ref_" + p + " " + e.dump));
-                    else if ("[object Array]" === s) i && 0 !== e.dump.length ? (e.noArrayIndent && !a && t > 0 ? It(e, t - 1, e.dump, r) : It(e, t, e.dump, r), f && (e.dump = "&ref_" + p + e.dump)) : (function(e, t, n) {
-                        var i, r, o, a = "",
-                            l = e.tag;
-                        for (i = 0, r = n.length; i < r; i += 1) o = n[i], e.replacer && (o = e.replacer.call(n, String(i), o)), (Ot(e, t, o, !1, !1) || void 0 === o && Ot(e, t, null, !1, !1)) && ("" !== a && (a += "," + (e.condenseFlow ? "" : " ")), a += e.dump);
-                        e.tag = l, e.dump = "[" + a + "]"
-                    }(e, t, e.dump), f && (e.dump = "&ref_" + p + " " + e.dump));
-                    else {
-                        if ("[object String]" !== s) {
-                            if ("[object Undefined]" === s) return !1;
-                            if (e.skipInvalid) return !1;
-                            throw new l("unacceptable kind of an object to dump " + s)
-                        }
-                        "?" !== e.tag && wt(e, e.dump, t, o, u)
-                    }
-                    null !== e.tag && "?" !== e.tag && (c = encodeURI("!" === e.tag[0] ? e.tag.slice(1) : e.tag).replace(/!/g, "%21"), c = "!" === e.tag[0] ? "!" + c : "tag:yaml.org,2002:" === c.slice(0, 18) ? "!!" + c.slice(18) : "!<" + c + ">", e.dump = c + " " + e.dump)
-                }
-                return !0
-            }
-
-            function St(e, t) {
-                var n, i, r = [],
-                    o = [];
-                for (Tt(e, r, o), n = 0, i = o.length; n < i; n += 1) t.duplicates.push(r[o[n]]);
-                t.usedDuplicates = new Array(i)
-            }
-
-            function Tt(e, t, n) {
-                var i, r, o;
-                if (null !== e && "object" == typeof e)
-                    if (-1 !== (r = t.indexOf(e))) - 1 === n.indexOf(r) && n.push(r);
-                    else if (t.push(e), Array.isArray(e))
-                    for (r = 0, o = e.length; r < o; r += 1) Tt(e[r], t, n);
-                else
-                    for (r = 0, o = (i = Object.keys(e)).length; r < o; r += 1) Tt(e[i[r]], t, n)
-            }
+            };
 
-            function Nt(e, t) {
+            function Ot(t, e) {
                 return function() {
-                    throw new Error("Function yaml." + e + " is removed in js-yaml 4. Use yaml." + t + " instead, which is now safe by default.")
+                    throw new Error("Function yaml." + t + " is removed in js-yaml 4. Use yaml." + e + " instead, which is now safe by default.")
                 }
             }
-            var Ft = m,
-                Mt = Se,
-                Lt = function(e, t) {
-                    var n = new lt(t = t || {});
-                    n.noRefs || St(e, n);
-                    var i = e;
-                    return n.replacer && (i = n.replacer.call({
-                        "": i
-                    }, "", i)), Ot(n, 0, i, !0, !0) ? n.dump + "\n" : ""
-                };
-            Nt("safeLoad", "load"), Nt("safeLoadAll", "loadAll"), Nt("safeDump", "dump")
+            Object.prototype.toString, Object.prototype.hasOwnProperty;
+            var Nt = m,
+                Et = Tt;
+            Ot("safeLoad", "load"), Ot("safeLoadAll", "loadAll"), Ot("safeDump", "dump")
         },
-        3379: e => {
-            var t = [];
+        3379: t => {
+            var e = [];
 
-            function n(e) {
-                for (var n = -1, i = 0; i < t.length; i++)
-                    if (t[i].identifier === e) {
+            function n(t) {
+                for (var n = -1, i = 0; i < e.length; i++)
+                    if (e[i].identifier === t) {
                         n = i;
                         break
                     } return n
             }
 
-            function i(e, i) {
-                for (var o = {}, a = [], l = 0; l < e.length; l++) {
-                    var c = e[l],
-                        s = i.base ? c[0] + i.base : c[0],
+            function i(t, i) {
+                for (var o = {}, a = [], c = 0; c < t.length; c++) {
+                    var l = t[c],
+                        s = i.base ? l[0] + i.base : l[0],
                         u = o[s] || 0,
                         p = "".concat(s, " ").concat(u);
                     o[s] = u + 1;
                     var f = n(p),
                         d = {
-                            css: c[1],
-                            media: c[2],
-                            sourceMap: c[3],
-                            supports: c[4],
-                            layer: c[5]
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3],
+                            supports: l[4],
+                            layer: l[5]
                         };
-                    if (-1 !== f) t[f].references++, t[f].updater(d);
+                    if (-1 !== f) e[f].references++, e[f].updater(d);
                     else {
                         var h = r(d, i);
-                        i.byIndex = l, t.splice(l, 0, {
+                        i.byIndex = c, e.splice(c, 0, {
                             identifier: p,
                             updater: h,
                             references: 1
                         })
                     }
                     a.push(p)
                 }
                 return a
             }
 
-            function r(e, t) {
-                var n = t.domAPI(t);
-                return n.update(e),
-                    function(t) {
-                        if (t) {
-                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
-                            n.update(e = t)
+            function r(t, e) {
+                var n = e.domAPI(e);
+                return n.update(t),
+                    function(e) {
+                        if (e) {
+                            if (e.css === t.css && e.media === t.media && e.sourceMap === t.sourceMap && e.supports === t.supports && e.layer === t.layer) return;
+                            n.update(t = e)
                         } else n.remove()
                     }
             }
-            e.exports = function(e, r) {
-                var o = i(e = e || [], r = r || {});
-                return function(e) {
-                    e = e || [];
+            t.exports = function(t, r) {
+                var o = i(t = t || [], r = r || {});
+                return function(t) {
+                    t = t || [];
                     for (var a = 0; a < o.length; a++) {
-                        var l = n(o[a]);
-                        t[l].references--
+                        var c = n(o[a]);
+                        e[c].references--
                     }
-                    for (var c = i(e, r), s = 0; s < o.length; s++) {
+                    for (var l = i(t, r), s = 0; s < o.length; s++) {
                         var u = n(o[s]);
-                        0 === t[u].references && (t[u].updater(), t.splice(u, 1))
+                        0 === e[u].references && (e[u].updater(), e.splice(u, 1))
                     }
-                    o = c
+                    o = l
                 }
             }
         },
-        569: e => {
-            var t = {};
-            e.exports = function(e, n) {
-                var i = function(e) {
-                    if (void 0 === t[e]) {
-                        var n = document.querySelector(e);
+        569: t => {
+            var e = {};
+            t.exports = function(t, n) {
+                var i = function(t) {
+                    if (void 0 === e[t]) {
+                        var n = document.querySelector(t);
                         if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                             n = n.contentDocument.head
-                        } catch (e) {
+                        } catch (t) {
                             n = null
                         }
-                        t[e] = n
+                        e[t] = n
                     }
-                    return t[e]
-                }(e);
+                    return e[t]
+                }(t);
                 if (!i) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                 i.appendChild(n)
             }
         },
-        9216: e => {
-            e.exports = function(e) {
-                var t = document.createElement("style");
-                return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
+        9216: t => {
+            t.exports = function(t) {
+                var e = document.createElement("style");
+                return t.setAttributes(e, t.attributes), t.insert(e, t.options), e
             }
         },
-        3565: (e, t, n) => {
-            e.exports = function(e) {
-                var t = n.nc;
-                t && e.setAttribute("nonce", t)
+        3565: (t, e, n) => {
+            t.exports = function(t) {
+                var e = n.nc;
+                e && t.setAttribute("nonce", e)
             }
         },
-        7795: e => {
-            e.exports = function(e) {
+        7795: t => {
+            t.exports = function(t) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
-                var t = e.insertStyleElement(e);
+                var e = t.insertStyleElement(t);
                 return {
                     update: function(n) {
-                        ! function(e, t, n) {
+                        ! function(t, e, n) {
                             var i = "";
                             n.supports && (i += "@supports (".concat(n.supports, ") {")), n.media && (i += "@media ".concat(n.media, " {"));
                             var r = void 0 !== n.layer;
                             r && (i += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), i += n.css, r && (i += "}"), n.media && (i += "}"), n.supports && (i += "}");
                             var o = n.sourceMap;
-                            o && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), t.styleTagTransform(i, e, t.options)
-                        }(t, e, n)
+                            o && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), e.styleTagTransform(i, t, e.options)
+                        }(e, t, n)
                     },
                     remove: function() {
-                        ! function(e) {
-                            if (null === e.parentNode) return !1;
-                            e.parentNode.removeChild(e)
-                        }(t)
+                        ! function(t) {
+                            if (null === t.parentNode) return !1;
+                            t.parentNode.removeChild(t)
+                        }(e)
                     }
                 }
             }
         },
-        4589: e => {
-            e.exports = function(e, t) {
-                if (t.styleSheet) t.styleSheet.cssText = e;
+        4589: t => {
+            t.exports = function(t, e) {
+                if (e.styleSheet) e.styleSheet.cssText = t;
                 else {
-                    for (; t.firstChild;) t.removeChild(t.firstChild);
-                    t.appendChild(document.createTextNode(e))
+                    for (; e.firstChild;) e.removeChild(e.firstChild);
+                    e.appendChild(document.createTextNode(t))
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/923.1e1a92e9bcd196793c79.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -64,27 +64,27 @@
                 h = u({
                     id: "@quarto/footnotes",
                     title: "Footnotes",
                     plugin: async () => [(await n.e(473).then(n.t.bind(n, 7473, 23))).default]
                 });
             var p = n(3379),
                 f = n.n(p),
-                g = n(7795),
-                m = n.n(g),
+                m = n(7795),
+                g = n.n(m),
                 v = n(569),
                 y = n.n(v),
                 b = n(3565),
                 k = n.n(b),
                 q = n(9216),
                 $ = n.n(q),
-                w = n(4589),
-                C = n.n(w),
-                _ = n(2760),
+                C = n(4589),
+                _ = n.n(C),
+                w = n(2760),
                 M = {};
-            M.styleTagTransform = C(), M.setAttributes = k(), M.insert = y().bind(null, "head"), M.domAPI = m(), M.insertStyleElement = $(), f()(_.Z, M), _.Z && _.Z.locals && _.Z.locals;
+            M.styleTagTransform = _(), M.setAttributes = k(), M.insert = y().bind(null, "head"), M.domAPI = g(), M.insertStyleElement = $(), f()(w.Z, M), w.Z && w.Z.locals && w.Z.locals;
             var x = n(4470),
                 L = n(9391),
                 A = n.n(L);
             class O extends x.RenderedHTMLCommon {
                 constructor(t, e) {
                     super(t), this.renderer = null, this.addClass("quarto-rendered-md"), this.markdownItManager = e
                 }
@@ -127,24 +127,24 @@
                         console.warn(`Failed to highlight ${n} code`, t)
                     }
                 } catch (t) {
                     console.warn(`No CodeMirror mode: ${n}`), console.warn(`Require CodeMirror mode error: ${t}`)
                 }
                 return ""
             };
-            const T = (t, e) => {
+            const j = (t, e) => {
                     var n, r;
                     return (null !== (n = t.rank) && void 0 !== n ? n : 100) - (null !== (r = e.rank) && void 0 !== r ? r : 100)
                 },
-                j = (t, e) => {
+                S = (t, e) => {
                     if (null === e) return;
                     const n = e.find((e => e[0] === t));
                     return n ? n[1] : void 0
                 },
-                S = (t, e) => {
+                T = (t, e) => {
                     if (null === e) return (e = []).push(["class", t]), e; {
                         const n = e.findIndex((t => "class" === t[0]));
                         if (n >= 0) {
                             const r = e[n];
                             return e[n] = ["class", `${r[1]} ${t}`.trim()], e
                         }
                         return e.push(["class", t]), e
@@ -196,15 +196,15 @@
                             return t.line = e + 1, !0
                         }
                         return !1
                     }), {
                         alt: []
                     }), t.renderer.rules[R] = function(t, e, n, r, s) {
                         const o = t[e];
-                        return o.attrs = S("quarto-div", o.attrs), `<div ${s.renderAttrs(o)}>`
+                        return o.attrs = T("quarto-div", o.attrs), `<div ${s.renderAttrs(o)}>`
                     }, t.renderer.rules[D] = function() {
                         return "</div>"
                     }
                 },
                 P = u({
                     id: "@quarto/divs",
                     title: "Pandoc fenced divs",
@@ -508,91 +508,91 @@
                                         e(t, l), c = "add-title";
                                         const n = new(ct())(ut, "", 1);
                                         n.attrs = n.attrs || [], n.meta = t, i.push(n)
                                     } else i.push(u)
                                 } else u.type === D ? (a === l ? (i.push(o()), i.push(new(ct())(dt, "", -1)), a = -1, t.env["quarto-active-callout"] = void 0) : i.push(u), l--) : i.push(u)
                         }
                         return t.tokens = i, !1
-                    })), t.renderer.rules[ut] = gt, t.renderer.rules[dt] = mt, t.renderer.rules[ht] = vt, t.renderer.rules[pt] = yt
+                    })), t.renderer.rules[ut] = mt, t.renderer.rules[dt] = gt, t.renderer.rules[ht] = vt, t.renderer.rules[pt] = yt
                 };
 
-            function gt(t, e, n, r, s) {
+            function mt(t, e, n, r, s) {
                 const o = t[e],
                     i = o.meta;
-                return o.attrs = S(`callout ${i.clz}`, o.attrs), o.attrs = S(kt(i.appearance), o.attrs), `<div ${s.renderAttrs(o)}>`
+                return o.attrs = T(`callout ${i.clz}`, o.attrs), o.attrs = T(kt(i.appearance), o.attrs), `<div ${s.renderAttrs(o)}>`
             }
 
-            function mt() {
+            function gt() {
                 return "</div>"
             }
 
             function vt(t, e) {
                 const n = t[e];
-                return `\n<div class="callout-header">\n<div class="callout-icon-container">\n  <i class="callout-icon"></i>\n</div>\n<div class="callout-title-container">${j("title",n.attrs)||""}\n`
+                return `\n<div class="callout-header">\n<div class="callout-icon-container">\n  <i class="callout-icon"></i>\n</div>\n<div class="callout-title-container">${S("title",n.attrs)||""}\n`
             }
 
             function yt() {
                 return "</div>\n</div>"
             }
             const bt = t => {
                     if (null === t) return;
                     const e = t.find((t => "class" === t[0]));
                     if (!e) return;
                     const n = e[1].split(" ").find((t => t.startsWith("callout-")));
                     if (n) {
                         const e = n.replace("callout-", ""),
-                            r = j("title", t) || e.slice(0, 1).toUpperCase() + e.slice(1);
+                            r = S("title", t) || e.slice(0, 1).toUpperCase() + e.slice(1);
                         return {
                             type: e || "note",
                             clz: n,
                             title: r,
                             appearance: (t => {
                                 if (!t) return "default";
                                 switch (t) {
                                     case "minimal":
                                         return "minimal";
                                     case "simple":
                                         return "simple";
                                     default:
                                         return "default"
                                 }
-                            })(j("appearance", t))
+                            })(S("appearance", t))
                         }
                     }
                 },
                 kt = t => `callout-style-${t||"default"}`,
                 qt = u({
                     id: "@quarto/callouts",
                     title: "Quarto callouts",
                     plugin: async () => [ft]
                 }),
-                $t = (t, e) => t.length > 0 ? `<div class="quarto-attribute-decorator${e?" "+e:""}">${t.map(wt).join("")}</div>` : "",
-                wt = t => `<span class="quarto-attribute-decorator-content">${t}</span>`,
-                Ct = "paragraph_open",
-                _t = "paragraph_close",
+                $t = (t, e) => t.length > 0 ? `<div class="quarto-attribute-decorator${e?" "+e:""}">${t.map(Ct).join("")}</div>` : "",
+                Ct = t => `<span class="quarto-attribute-decorator-content">${t}</span>`,
+                _t = "paragraph_open",
+                wt = "paragraph_close",
                 Mt = "inline",
                 xt = "table_open",
                 Lt = "figure_open",
                 At = "figcaption_open",
                 Ot = "figcaption_close",
                 Et = (t, e) => {
                     t.type = "open" === e ? Lt : "figure_close", t.tag = "figure"
                 };
 
-            function Tt(t, e) {
+            function jt(t, e) {
                 e = e || {}, t.core.ruler.before("linkify", "implicit_figures", (t => {
                     let n = 1;
                     for (let r = 1, s = t.tokens.length; r < s - 1; ++r) {
                         const o = t.tokens[r];
                         if ("inline" !== o.type) continue;
                         if (!o.children || 1 !== o.children.length && 3 !== o.children.length) continue;
                         if (1 === o.children.length && "image" !== o.children[0].type) continue;
                         if (3 === o.children.length && ("link_open" !== o.children[0].type || "image" !== o.children[1].type || "link_close" !== o.children[2].type)) continue;
-                        if (0 !== r && t.tokens[r - 1].type !== Ct) continue;
-                        if (r !== s - 1 && t.tokens[r + 1].type !== _t) continue;
+                        if (0 !== r && t.tokens[r - 1].type !== _t) continue;
+                        if (r !== s - 1 && t.tokens[r + 1].type !== wt) continue;
                         const i = 1 === o.children.length ? o.children[0] : o.children[1];
                         if (!i.children || 0 === i.children.length) continue;
                         const a = t.tokens[r - 1];
                         if (Et(a, "open"), Et(t.tokens[r + 1], "close"), !0 === e.dataType && t.tokens[r - 1].attrPush(["data-type", "image"]), !0 === e.link && 1 === o.children.length) {
                             o.children.unshift(new t.Token("link_open", "a", 1));
                             const e = i.attrGet("src");
                             null !== e && o.children[0].attrPush(["href", e]), o.children.push(new t.Token("link_close", "a", -1))
@@ -600,17 +600,17 @@
                         if (!0 === e.figcaption && i.children && i.children.length && (o.children.push(new t.Token(At, "figcaption", 1)), o.children.splice(o.children.length, 0, ...i.children), o.children.push(new t.Token(Ot, "figcaption", -1)), i.children.length = 0), e.copyAttrs && i.attrs) {
                             const t = !0 === e.copyAttrs ? "" : e.copyAttrs;
                             a.attrs = i.attrs.filter((([e]) => e.match(t)))
                         }!0 === e.tabindex && (t.tokens[r - 1].attrPush(["tabindex", String(n)]), n++), !0 === e.lazyLoading && i.attrPush(["loading", "lazy"])
                     }
                 }))
             }
-            const jt = "math_block";
+            const St = "math_block";
 
-            function St(t, e) {
+            function Tt(t, e) {
                 return e.display ? `<div class='quarto-display-math'>\\[${t}\\]</div>` : `<span class='quarto-inline-math'>\\(${t}\\)</span>`
             }
 
             function Rt(t, e) {
                 const n = t.posMax;
                 let r = !0,
                     s = !0;
@@ -656,41 +656,41 @@
                 let u, d = t.src.slice(a, l);
                 if (r) return !0;
                 for ("$$" === d.trim().slice(-2) && (d = d.trim().slice(0, -2), i = !0), s = e; !(i || (s++, s >= n) || (a = t.bMarks[s] + t.tShift[s], l = t.eMarks[s], a < l && t.tShift[s] < t.blkIndent));) {
                     const e = t.src.slice(a, l).trim().match(/^\$\$\s*(\{.*\})?\s*$/);
                     e && (o = t.src.slice(0, l).lastIndexOf("$$"), c = t.src.slice(a, o), u = e[1], i = !0)
                 }
                 t.line = s + 1;
-                const h = t.push(jt, "math", 0);
+                const h = t.push(St, "math", 0);
                 return h.block = !0, u && (h.info = u), h.content = (d && d.trim() ? d + "\n" : "") + t.getLines(e + 1, s, t.tShift[e], !0) + (c && c.trim() ? c : ""), h.map = [e, t.line], h.markup = "$$", !0
             }
 
             function Pt(t, e) {
                 const n = void 0 === (e = e || {}).enableInlines || e.enableInlines,
                     r = {
                         display: !1
                     };
-                t.inline.ruler.after("escape", "math_inline", Dt), t.block.ruler.after("blockquote", jt, It, {
+                t.inline.ruler.after("escape", "math_inline", Dt), t.block.ruler.after("blockquote", St, It, {
                     alt: ["paragraph", "reference", "blockquote", "list"]
                 }), n && (t.renderer.rules.math_inline = function(t, e) {
-                    return r.display = !1, St(t[e].content, r)
+                    return r.display = !1, Tt(t[e].content, r)
                 }), t.renderer.rules.math_block = function(t, e) {
-                    return r.display = !0, St(t[e].content, r)
+                    return r.display = !0, Tt(t[e].content, r)
                 }
             }
             const Ht = "quarto_decorator",
                 Wt = "quarto-decorator-options",
                 zt = t => {
                     t.core.ruler.push("quarto-decorator", (t => {
                         const e = [];
                         for (const n of t.tokens) "fence" === n.type && !n.attrs && n.info || "heading_open" === n.type && n.attrs || n.type === R && n.attrs ? e.push(Nt(n)) : n.type === Lt && n.attrs ? e.push(Nt(n, {
                             hide: {
                                 attributes: !0
                             }
-                        })) : (n.type === xt && n.attrs || n.type === jt && n.attrs) && e.push(Nt(n)), e.push(n);
+                        })) : (n.type === xt && n.attrs || n.type === St && n.attrs) && e.push(Nt(n)), e.push(n);
                         t.tokens = e
                     })), t.renderer.rules[Ht] = Ft
                 };
 
             function Nt(t, e) {
                 const n = new(ct())(Ht, "div", 1);
                 return n.attrs = t.attrs, n.info = t.info, e && (n.meta = n.meta || {}, n.meta[Wt] = e), n
@@ -698,16 +698,16 @@
 
             function Ft(t, e) {
                 var n;
                 const r = t[e],
                     s = null === (n = r.meta) || void 0 === n ? void 0 : n[Wt];
                 return r.info ? $t([r.info]) : ((t, e) => {
                     var n;
-                    const r = j("id", t.attrs),
-                        s = j("class", t.attrs),
+                    const r = S("id", t.attrs),
+                        s = S("class", t.attrs),
                         o = null === (n = t.attrs) || void 0 === n ? void 0 : n.filter((t => "id" !== t[0] && "class" !== t[0])),
                         i = [];
                     if (r && !(null == e ? void 0 : e.hide.id) && i.push(`#${r}`), s && !(null == e ? void 0 : e.hide.classes)) {
                         const t = s.split(" ").map((t => `.${t}`)).join(" ");
                         i.push(t)
                     }
                     if (o && o.length > 0 && !(null == e ? void 0 : e.hide.attributes)) {
@@ -757,25 +757,27 @@
                     return t.line = a + 1, !1
                 }), {
                     alt: ["paragraph", "reference", "blockquote", "list"]
                 }), t.renderer.rules[Zt] = Gt
             }
 
             function Gt(t, e) {
-                const n = Ut(t[e].markup);
-                if ("object" == typeof n) {
+                const n = t[e],
+                    r = Ut(n.markup);
+                if ("object" == typeof r) {
                     const t = {},
-                        e = n,
-                        r = t => {
+                        e = r,
+                        s = t => {
                             if (void 0 !== e[t] && "string" == typeof e[t]) {
                                 const n = e[t];
                                 return delete e[t], n
                             }
-                        };
-                    t.title = r("title"), t.subtitle = r("subtitle"), t.abstract = r("abstract"), t.date = r("date"), t.modified = r("date-modified"), t.doi = r("doi"), t.authors = function(t) {
+                        },
+                        o = ["title", "subtitle", "abstract", "date", "date-modified", "doi", "author", "authors"];
+                    t.title = s("title"), t.subtitle = s("subtitle"), t.abstract = s("abstract"), t.date = s("date"), t.modified = s("date-modified"), t.doi = s("doi"), t.authors = function(t) {
                         var e;
                         const n = Array.isArray(t) ? t : [t],
                             r = [];
                         for (const t of n)
                             if ("string" == typeof t) r.push({
                                 name: t
                             });
@@ -793,16 +795,16 @@
                                 name: null !== (e = n("name", "")) && void 0 !== e ? e : "",
                                 orcid: n("orcid"),
                                 affil: s
                             })
                         }
                         return r
                     }(e.author || e.authors), delete e.author, delete e.authors;
-                    const s = [],
-                        o = function(t) {
+                    const i = [],
+                        a = function(t) {
                             var e;
                             const n = [];
                             t.title && n.push(`<h1>${t.title}</h1>`), t.subtitle && n.push(`<p class="quarto-subtitle">${t.subtitle}</p>`);
                             const r = [];
                             if (t.authors && (null === (e = t.authors) || void 0 === e ? void 0 : e.length) > 0) {
                                 const e = [],
                                     n = [];
@@ -843,21 +845,25 @@
                             }])), r.length > 0 && n.push(function(t) {
                                 const e = [];
                                 return e.push('<div class="quarto-meta-block">'), t.forEach((t => {
                                     e.push(t)
                                 })), e.push("</div>"), e.join("\n")
                             }(r)), t.abstract && n.push(`<p class="quarto-abstract">${t.abstract}</p>`), n.join("\n")
                         }(t);
-                    if (s.push(o), Object.keys(e).length > 0) {
+                    if (i.push(a), Object.keys(e).length > 0) {
                         const t = $t(["Options"]);
-                        s.push(t);
-                        const n = `<pre class="quarto-frontmatter-container"><code class="cm-s-jupyter language-yaml quarto-frontmatter">${Qt.$w(e)}</code></pre>`;
-                        s.push(n)
+                        i.push(t);
+                        let e = !1;
+                        const r = [],
+                            s = n.markup.replace(/---\s*$/, "").replace(/^---\s*/, "");
+                        for (const t of s.split("\n")) o.some((e => null !== t.match(RegExp(`^${e}\\s*:`)))) ? e = !0 : e && !t.match(/^\S/) || (e = !1, r.push(t));
+                        const a = `<pre class="quarto-frontmatter-container"><code class="cm-s-jupyter language-yaml quarto-frontmatter">${r.join("\n")}</code></pre>`;
+                        i.push(a)
                     }
-                    return s.join("\n")
+                    return i.join("\n")
                 }
                 return ""
             }
 
             function Ut(t) {
                 t = t.replace(/---\s*$/, "");
                 try {
@@ -901,33 +907,33 @@
                             }
                         }
                     }
                 }),
                 Xt = u({
                     id: "@quarto/figures",
                     title: "Quarto figures",
-                    plugin: async () => [Tt, {
+                    plugin: async () => [jt, {
                         figcaption: !0,
                         copyAttrs: !0
                     }]
                 }),
                 te = t => {
                     t.core.ruler.push("quarto-figure-divs", (t => {
                         const e = [];
                         for (let n = 0; n < t.tokens.length; n++) {
                             const r = t.tokens[n];
                             if (r.type === R) {
-                                const t = j("id", r.attrs);
+                                const t = S("id", r.attrs);
                                 (null == t ? void 0 : t.startsWith("fig-")) ? (e.push(!0), Et(r, "open")) : e.push(!1)
                             } else if (r.type === D && e.pop()) {
                                 if (n - 3 >= 0) {
                                     const e = t.tokens[n - 3],
                                         r = t.tokens[n - 2],
                                         s = t.tokens[n - 1];
-                                    e.type === Ct && s.type === _t && r.type === Mt && (ee(t.tokens[n - 3], "open"), ee(t.tokens[n - 1], "close"))
+                                    e.type === _t && s.type === wt && r.type === Mt && (ee(t.tokens[n - 3], "open"), ee(t.tokens[n - 1], "close"))
                                 }
                                 Et(r, "close")
                             }
                         }
                     }))
                 },
                 ee = (t, e) => {
@@ -954,15 +960,15 @@
                             }
                         }
                         for (const e of n) se(t.tokens, e.start, e.end)
                     }))
                 };
 
             function se(t, e, n) {
-                if (t.length > n + 3 && t[n + 1].type === Ct && t[n + 2].type === Mt && t[n + 3].type === _t) {
+                if (t.length > n + 3 && t[n + 1].type === _t && t[n + 2].type === Mt && t[n + 3].type === wt) {
                     const r = t[n + 2],
                         s = (null !== r.children && r.children.length > 0 && "text" === r.children[0].type && r.children ? r.children[0].content : "").match(/^:\s([^{}]*)(?:\{.*\}){0,1}$/);
                     if (s && s[1]) {
                         const r = t.splice(n + 1, 3);
                         r[0].type = "table_caption", r[0].tag = "caption", t[e].attrs = r[0].attrs, r[0].attrs = [], r[1].children && r[1].children.length > 0 && (r[1].children[0].content = s[1]), r[2].type = "table_caption", r[2].tag = "caption", t.splice(e + 1, 0, ...r)
                     }
                 }
@@ -1022,15 +1028,15 @@
                             r = {
                                 registerPlugin(t) {
                                     n.set(t.id, t)
                                 },
                                 async getRenderer(r, s = {}) {
                                     var o, i, a, l;
                                     const c = [...n.values()];
-                                    c.sort(T);
+                                    c.sort(j);
                                     const u = ((t, e, n, r, s) => {
                                         let o = {
                                             html: !0,
                                             linkify: !0,
                                             typographer: !0,
                                             langPrefix: `cm-s-${r.defaultTheme} language-`,
                                             highlight: E(s)
@@ -1065,15 +1071,15 @@
                                     }(e));
                                     for (const t of c) try {
                                         const [e, ...n] = await t.plugin();
                                         d = d.use(e, ...n), void 0 !== (null === (o = t.hooks) || void 0 === o ? void 0 : o.preParse) && h.push(null === (i = t.hooks) || void 0 === i ? void 0 : i.preParse), void 0 !== (null === (a = t.hooks) || void 0 === a ? void 0 : a.postRender) && p.push(null === (l = t.hooks) || void 0 === l ? void 0 : l.postRender)
                                     } catch (e) {
                                         console.warn(`Failed to load/use markdown-it plugin ${t.id}`, e)
                                     }
-                                    return h.sort(T), p.sort(T), {
+                                    return h.sort(j), p.sort(j), {
                                         render: t => d.render(t),
                                         preParse: async t => {
                                             for (const e of h) t = await e.run(t);
                                             return t
                                         },
                                         postRender: async t => {
                                             for (const e of p) await e.run(t)
```

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/remoteEntry.110f607f4dd53733e5a3.js` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/remoteEntry.7156007e7b025a17b2e3.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -70,22 +70,22 @@
         269: "6f08c3812b138d1ca789",
         316: "f7e4dd762f98107da4a5",
         336: "1731c2a718bbc1b9cc4a",
         384: "6c76694e25edf7010d50",
         473: "481d81f5703a7a82c3b1",
         487: "dee02fd512e9bb15dee6",
         543: "40a7a1799fcad108039e",
-        573: "79885c9e9fcb552239cd",
+        573: "c159bf4028ff12850190",
         596: "ef22233afe464ab9134a",
         645: "406375856388e9d7e4e9",
         651: "7673e27b3217024cb32d",
         675: "d6106f5e979f073a7272",
         700: "30097f2c1808e10c985f",
         724: "265325864c2c7d67e29e",
-        923: "b51eb181f4c017b19c97",
+        923: "1e1a92e9bcd196793c79",
         965: "f95cad8ec0ea39351f31",
         980: "57fcdfda225b581383c0"
     } [e] + ".js?v=" + {
         3: "b7aa6beb2ddb69469e1e",
         11: "bbf21e9c517bec162b9c",
         136: "43b409c7c7e6885bc7ee",
         150: "9b2f6283ffc934651e1c",
@@ -94,22 +94,22 @@
         269: "6f08c3812b138d1ca789",
         316: "f7e4dd762f98107da4a5",
         336: "1731c2a718bbc1b9cc4a",
         384: "6c76694e25edf7010d50",
         473: "481d81f5703a7a82c3b1",
         487: "dee02fd512e9bb15dee6",
         543: "40a7a1799fcad108039e",
-        573: "79885c9e9fcb552239cd",
+        573: "c159bf4028ff12850190",
         596: "ef22233afe464ab9134a",
         645: "406375856388e9d7e4e9",
         651: "7673e27b3217024cb32d",
         675: "d6106f5e979f073a7272",
         700: "30097f2c1808e10c985f",
         724: "265325864c2c7d67e29e",
-        923: "b51eb181f4c017b19c97",
+        923: "1e1a92e9bcd196793c79",
         965: "f95cad8ec0ea39351f31",
         980: "57fcdfda225b581383c0"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -168,15 +168,15 @@
                         (!f || !f.loaded && (!a != !f.eager ? a : d > f.from)) && (n[t] = {
                             get: r,
                             from: d,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === r && (f("jupyterlab-quarto", "0.2.7", (() => Promise.all([P.e(185), P.e(573), P.e(150), P.e(923)]).then((() => () => P(5923))))), f("markdown-it-attrs", "4.1.6", (() => P.e(543).then((() => () => P(9543))))), f("markdown-it-deflist", "2.1.0", (() => P.e(645).then((() => () => P(645))))), f("markdown-it-footnote", "3.0.3", (() => P.e(384).then((() => () => P(2384))))), f("markdown-it-sub", "1.0.0", (() => P.e(700).then((() => () => P(700))))), f("markdown-it-sup", "1.0.0", (() => P.e(3).then((() => () => P(7003))))), f("markdown-it-task-lists", "1.4.1", (() => P.e(651).then((() => () => P(4651))))), f("markdown-it", "12.3.2", (() => Promise.all([P.e(980), P.e(185)]).then((() => () => P(9980))))), f("mermaid", "9.4.3", (() => P.e(136).then((() => () => P(4136))))), f("wcwidth", "1.0.1", (() => P.e(11).then((() => () => P(1011)))))), e[r] = i.length ? Promise.all(i).then((() => e[r] = 1)) : 1
+                return "default" === r && (f("jupyterlab-quarto", "0.2.8", (() => Promise.all([P.e(185), P.e(573), P.e(150), P.e(923)]).then((() => () => P(5923))))), f("markdown-it-attrs", "4.1.6", (() => P.e(543).then((() => () => P(9543))))), f("markdown-it-deflist", "2.1.0", (() => P.e(645).then((() => () => P(645))))), f("markdown-it-footnote", "3.0.3", (() => P.e(384).then((() => () => P(2384))))), f("markdown-it-sub", "1.0.0", (() => P.e(700).then((() => () => P(700))))), f("markdown-it-sup", "1.0.0", (() => P.e(3).then((() => () => P(7003))))), f("markdown-it-task-lists", "1.4.1", (() => P.e(651).then((() => () => P(4651))))), f("markdown-it", "12.3.2", (() => Promise.all([P.e(980), P.e(185)]).then((() => () => P(9980))))), f("mermaid", "9.4.3", (() => P.e(136).then((() => () => P(4136))))), f("wcwidth", "1.0.1", (() => P.e(11).then((() => () => P(1011)))))), e[r] = i.length ? Promise.all(i).then((() => e[r] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var t = P.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
```

### Comparing `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/third-party-licenses.json` & `jupyterlab_quarto-0.2.8/jupyterlab-quarto/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/index.ts` & `jupyterlab_quarto-0.2.8/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/manager.ts` & `jupyterlab_quarto-0.2.8/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/types.ts` & `jupyterlab_quarto-0.2.8/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/widgets.ts` & `jupyterlab_quarto-0.2.8/src/widgets.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/ast/ast.ts` & `jupyterlab_quarto-0.2.8/src/ast/ast.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/hooks/codemirror.ts` & `jupyterlab_quarto-0.2.8/src/hooks/codemirror.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/callouts.ts` & `jupyterlab_quarto-0.2.8/src/plugins/callouts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/cites.ts` & `jupyterlab_quarto-0.2.8/src/plugins/cites.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/decorator.ts` & `jupyterlab_quarto-0.2.8/src/plugins/decorator.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/divs.ts` & `jupyterlab_quarto-0.2.8/src/plugins/divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/figure-divs.ts` & `jupyterlab_quarto-0.2.8/src/plugins/figure-divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/figures.ts` & `jupyterlab_quarto-0.2.8/src/plugins/figures.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/index.ts` & `jupyterlab_quarto-0.2.8/src/plugins/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/math.ts` & `jupyterlab_quarto-0.2.8/src/plugins/math.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/shortcodes.ts` & `jupyterlab_quarto-0.2.8/src/plugins/shortcodes.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/spans.ts` & `jupyterlab_quarto-0.2.8/src/plugins/spans.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/table-captions.ts` & `jupyterlab_quarto-0.2.8/src/plugins/table-captions.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/yaml.ts` & `jupyterlab_quarto-0.2.8/src/plugins/yaml.ts`

 * *Files 5% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         return val;
       } else {
         return undefined;
       }
     };
 
     // Read simple values
+    const eatKeys = ['title', 'subtitle', 'abstract', 'date', 'date-modified', 'doi', 'author', 'authors'];
     titleBlock.title = readStr('title');
     titleBlock.subtitle = readStr('subtitle');
     titleBlock.abstract = readStr('abstract');
     titleBlock.date = readStr('date');
     titleBlock.modified = readStr('date-modified');
     titleBlock.doi = readStr('doi');
 
@@ -211,17 +212,36 @@
     titleLines.push(titleRendered);
 
     if (Object.keys(frontMatter).length > 0) {
       // decorator
       const decor = decorator(['Options']);
       titleLines.push(decor);
 
-      // yaml
-      const yamlDump = yaml.dump(frontMatter);
-      const otherYamlRendered = `<pre class="quarto-frontmatter-container"><code class="cm-s-jupyter language-yaml quarto-frontmatter">${yamlDump}</code></pre>`;
+      // Left over YAML
+      // Use the raw YAML string so we don't end up mutating / round tripping the YAML
+      let eating = false;
+      const outputYaml: string[] = [];
+      const yamlNoDelimiters = token.markup.replace(/---\s*$/, '').replace(/^---\s*/, '');
+
+      for (const line of yamlNoDelimiters.split("\n")) {
+        const eatKey = eatKeys.some((k) => {
+          const match = line.match(RegExp(`^${k}\\s*:`));
+          return match !== null;
+        })
+        if (eatKey) {
+          eating = true;
+        } else {
+          if (!eating || line.match(/^\S/)) {
+            eating = false;
+            outputYaml.push(line);  
+          }
+        }
+      }
+
+      const otherYamlRendered = `<pre class="quarto-frontmatter-container"><code class="cm-s-jupyter language-yaml quarto-frontmatter">${outputYaml.join("\n")}</code></pre>`;
 
       titleLines.push(otherYamlRendered);
     }
     return titleLines.join('\n');
   } else {
     return '';
   }
```

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/index.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetCells.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/gridtables/GetCells.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/EmitTable.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/EmitTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetLine.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/GetLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTable.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/ParseTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/IState.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/interfaces/markdown-it/IState.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/gridtables/rules/gridtable.ts` & `jupyterlab_quarto-0.2.8/src/plugins/gridtables/rules/gridtable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/mermaid/index.ts` & `jupyterlab_quarto-0.2.8/src/plugins/mermaid/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/utils/html.ts` & `jupyterlab_quarto-0.2.8/src/plugins/utils/html.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/plugins/utils/markdownit.ts` & `jupyterlab_quarto-0.2.8/src/plugins/utils/markdownit.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/providers/divs.ts` & `jupyterlab_quarto-0.2.8/src/providers/divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/providers/math.ts` & `jupyterlab_quarto-0.2.8/src/providers/math.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/src/providers/provider.ts` & `jupyterlab_quarto-0.2.8/src/providers/provider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/style/base.css` & `jupyterlab_quarto-0.2.8/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/ui-tests/README.md` & `jupyterlab_quarto-0.2.8/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/ui-tests/tests/jupyterlab-quarto.spec.ts` & `jupyterlab_quarto-0.2.8/ui-tests/tests/jupyterlab-quarto.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/.gitignore` & `jupyterlab_quarto-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/LICENSE` & `jupyterlab_quarto-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/README.md` & `jupyterlab_quarto-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/pyproject.toml` & `jupyterlab_quarto-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.7/PKG-INFO` & `jupyterlab_quarto-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-quarto
-Version: 0.2.7
+Version: 0.2.8
 Summary: Jupyter extension to enable authoring of Quarto documents within Jupyterlab Notebooks.
 Project-URL: Homepage, https://github.com/quarto-dev/jupyterlab-quarto
 Project-URL: Bug Tracker, https://github.com/quarto-dev/jupyterlab-quarto/issues
 Project-URL: Repository, https://github.com/quarto-dev/jupyterlab-quarto.git
 Author-email: Charles Teague <charles@posit.co>
 License: BSD 3-Clause License
```

