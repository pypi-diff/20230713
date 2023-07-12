# Comparing `tmp/quartodoc-0.3.5.tar.gz` & `tmp/quartodoc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.3.5.tar", last modified: Thu Jul  6 21:08:34 2023, max compression
+gzip compressed data, was "quartodoc-0.4.0.tar", last modified: Wed Jul 12 22:53:10 2023, max compression
```

## Comparing `quartodoc-0.3.5.tar` & `quartodoc-0.4.0.tar`

### file list

```diff
@@ -1,137 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-06 21:08:22.000000 quartodoc-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 21:08:22.000000 quartodoc-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 21:08:22.000000 quartodoc-0.3.5/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-06 21:08:22.000000 quartodoc-0.3.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-06 21:08:34.463706 quartodoc-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-06 21:08:22.000000 quartodoc-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-06 21:08:22.000000 quartodoc-0.3.5/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.443705 quartodoc-0.3.5/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:08:22.000000 quartodoc-0.3.5/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 21:08:22.000000 quartodoc-0.3.5/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-06 21:08:22.000000 quartodoc-0.3.5/_extensions/interlinks/interlinks.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 21:08:22.000000 quartodoc-0.3.5/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.447705 quartodoc-0.3.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/advanced-layouts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/basic-building.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/basic-content.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-big-picture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-dataclasses.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-prepare.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/dev-renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/docstring-examples.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/docstring-style.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/extra-build-sequence.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 21:08:22.000000 quartodoc-0.3.5/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.451706 quartodoc-0.3.5/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/single-page/reference/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/examples/weird-install/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/weird-install/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/examples/weird-install/src/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 21:08:22.000000 quartodoc-0.3.5/examples/weird-install/src/some_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 21:08:22.000000 quartodoc-0.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.455706 quartodoc-0.3.5/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/autosummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/builder/write.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_alias_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/quartodoc/tests/example_interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/quartodoc/tests/example_interlinks/_inv/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/_inv/other_objects.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.md
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/example_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_builder_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 21:08:22.000000 quartodoc-0.3.5/quartodoc/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.459706 quartodoc-0.3.5/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 21:08:34.000000 quartodoc-0.3.5/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-06 21:08:22.000000 quartodoc-0.3.5/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.443705 quartodoc-0.3.5/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:08:34.463706 quartodoc-0.3.5/scripts/filter-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-06 21:08:22.000000 quartodoc-0.3.5/scripts/filter-spec/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 21:08:22.000000 quartodoc-0.3.5/scripts/filter-spec/generate_test_qmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-06 21:08:34.463706 quartodoc-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.818970 quartodoc-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-12 22:52:56.000000 quartodoc-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-12 22:52:56.000000 quartodoc-0.4.0/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-12 22:52:56.000000 quartodoc-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-12 22:53:10.818970 quartodoc-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-12 22:52:56.000000 quartodoc-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-12 22:52:56.000000 quartodoc-0.4.0/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.794968 quartodoc-0.4.0/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 22:52:56.000000 quartodoc-0.4.0/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 22:52:56.000000 quartodoc-0.4.0/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-12 22:52:56.000000 quartodoc-0.4.0/_extensions/interlinks/interlinks.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.802969 quartodoc-0.4.0/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.802969 quartodoc-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.802969 quartodoc-0.4.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/auto-package/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/auto-package/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/reference/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/weird-install/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/weird-install/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/weird-install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/weird-install/src/some_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 22:52:56.000000 quartodoc-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20767 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/__snapshots__/test_renderers.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/example_interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/example_interlinks/_inv/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/_inv/other_objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-12 22:52:56.000000 quartodoc-0.4.0/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.818970 quartodoc-0.4.0/scripts/filter-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-12 22:52:56.000000 quartodoc-0.4.0/scripts/filter-spec/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-12 22:52:56.000000 quartodoc-0.4.0/scripts/filter-spec/generate_test_qmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-12 22:53:10.818970 quartodoc-0.4.0/setup.cfg
```

### Comparing `quartodoc-0.3.5/.github/CODE_OF_CONDUCT.md` & `quartodoc-0.4.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/.github/workflows/ci.yml` & `quartodoc-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/.gitignore` & `quartodoc-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/LICENSE` & `quartodoc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/Makefile` & `quartodoc-0.4.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 	cd $(EXAMPLE_INTERLINKS) && quarto render test.qmd --to gfm
 
 
 examples/%/_site: examples/%/_quarto.yml
 	cd examples/$* \
 		&& quarto add --no-prompt ../.. \
 		&& quarto add --no-prompt quarto-ext/shinylive
-	cd examples/$* && quartodoc build _quarto.yml --verbose
+	cd examples/$* && quartodoc build --config _quarto.yml --verbose
 	cd examples/$* && quartodoc interlinks
 	quarto render $(dir $<)
 
 
 docs/examples/%: examples/%/_site
 	rm -rf docs/examples/$*
 	cp -rv $< $@
 
-docs-build-examples: docs/examples/single-page docs/examples/pkgdown
+docs-build-examples: docs/examples/single-page docs/examples/pkgdown docs/examples/auto-package
 
 docs-build: docs-build-examples
 	cd docs && quarto add --no-prompt ..
 	cd docs && quartodoc build
 	cd docs && quartodoc interlinks
 	quarto render docs
```

### Comparing `quartodoc-0.3.5/PKG-INFO` & `quartodoc-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.5
+Version: 0.4.0
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.3.5/README.md` & `quartodoc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/README.qmd` & `quartodoc-0.4.0/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/_extensions/interlinks/interlinks.lua` & `quartodoc-0.4.0/_extensions/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/case_studies/objects_sqla.inv` & `quartodoc-0.4.0/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/case_studies/parsing.qmd` & `quartodoc-0.4.0/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/case_studies/some_package.py` & `quartodoc-0.4.0/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/case_studies/sphinx-inventory.md` & `quartodoc-0.4.0/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/case_studies/sphinx-inventory.qmd` & `quartodoc-0.4.0/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/_quarto.yml` & `quartodoc-0.4.0/docs/_quarto.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 project:
   type: website
   output-dir: _build
   resources:
     - examples/single-page
     - examples/pkgdown
+    - examples/auto-package
 
 metadata-files:
   - api/_sidebar.yml
 
 filters:
   - "interlinks"
```

### Comparing `quartodoc-0.3.5/docs/examples/index.qmd` & `quartodoc-0.4.0/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/architecture.qmd` & `quartodoc-0.4.0/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/basic-building.qmd` & `quartodoc-0.4.0/docs/get-started/basic-building.qmd`

 * *Files 12% similar despite different names*

```diff
@@ -5,35 +5,54 @@
     display_name: Python 3 (ipykernel)
     language: python
     name: python3
 ---
 
 **tl;dr**: Once you've configured quartodoc in your `_quarto.yml` file, use the following commands to build and preview a documentation site.
 
+## `quartodoc build`: Create doc files
+
+Automatically generate `.qmd` files with reference api documentation.  This is written by default to the reference/ folder in your quarto project.
+
 ```bash
-# Create the documentation files. These are written 
-# by default to the reference/ folder in your docs.
-quartodoc build --verbose
-
-# Create optional inventory files, which allow you to
-# link to API doc pages within and across documentation
-# sites. These are put in the _inv folder in your docs.
-quartodoc interlinks
+quartodoc build
+```
 
-# Preview the documentation site.
-# Use quarto render to generate the final site.
-quarto preview
+If you are iterating on your docstrings while previewing your site with `quarto preview`, you will likely want to rebuild the doc pages automatically when docstrings change.  The `--watch` flag does exactly this.
+
+```bash
+quartodoc build --watch
+```
+
+For more information on the `quartodoc build` command, use `--help` in the terminal like so:
+
+```bash
+quartodoc build --help
+```
+
+```{python}
+#|echo: false
+!quartodoc build --help
+```
+
+
+## `quartodoc interlinks`: Create inventory files
+
+Inventory files facilitate linking to API doc pages within and across `quartodoc` sites.  This is optional.
+  
+```bash
+quartodoc interlinks
 ```
 
-## Rebuilding doc pages
+## `quarto preview`: Preview the site
 
-While using `quarto preview`, you can preview updates to your docstrings by regenerating their documentation pages:
+Use `quarto` to preview the site:
 
 ```bash
-quartodoc build --verbose
+quarto preview
 ```
 
 ## Speeding up preview
 
 ### Rewriting doc files
 
 By default, the `quartodoc build` only re-writes doc pages when it detects
```

### Comparing `quartodoc-0.3.5/docs/get-started/basic-content.qmd` & `quartodoc-0.4.0/docs/get-started/basic-content.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/basic-docs.qmd` & `quartodoc-0.4.0/docs/get-started/basic-docs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/crossrefs.qmd` & `quartodoc-0.4.0/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/dev-big-picture.qmd` & `quartodoc-0.4.0/docs/get-started/dev-big-picture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/dev-docstrings.qmd` & `quartodoc-0.4.0/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/dev-prepare.qmd` & `quartodoc-0.4.0/docs/get-started/dev-prepare.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/dev-renderers.qmd` & `quartodoc-0.4.0/docs/get-started/dev-renderers.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/docstring-examples.qmd` & `quartodoc-0.4.0/docs/get-started/docstring-examples.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/extending.qmd` & `quartodoc-0.4.0/docs/get-started/extending.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/extra-build-sequence.qmd` & `quartodoc-0.4.0/docs/get-started/extra-build-sequence.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/interlinks.qmd` & `quartodoc-0.4.0/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/get-started/overview.qmd` & `quartodoc-0.4.0/docs/get-started/overview.qmd`

 * *Files 4% similar despite different names*

```diff
@@ -81,28 +81,26 @@
 
 ```bash
 quarto preview
 ```
 
 ## Rebuilding site
 
-As mentioned in the previous section, you can preview your quartodoc site using these commands:
+You can preview your `quartodoc` site using the following commands:
+
+First, watch for changes to the library you are documenting so that your docs will automatically re-generate:
 
 ```bash
-quartodoc build
-quarto preview
+quartodoc build --watch
 ```
 
-In order to rebuild your API documentation pages during a quarto preview, re-run
-the quartodoc build command:
+Second, preview your site:
 
 ```bash
-# with quarto preview running, you only need to re-run quartodoc build,
-# which will re-create the pages of your API documentation.
-quartodoc build
+quarto preview
 ```
 
 ## Looking up objects
 
 Finding python objects to document involves two pieces of configuration:
 
 * the package name.
```

### Comparing `quartodoc-0.3.5/docs/get-started/sidebar.qmd` & `quartodoc-0.4.0/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/docs/styles.css` & `quartodoc-0.4.0/docs/styles.css`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/dascore/_quarto.yml` & `quartodoc-0.4.0/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/dascore/generate_api.py` & `quartodoc-0.4.0/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/pkgdown/_quarto.yml` & `quartodoc-0.4.0/examples/pkgdown/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/pkgdown/objects.json` & `quartodoc-0.4.0/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.4.0/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.4.0/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/single-page/_quarto.yml` & `quartodoc-0.4.0/examples/single-page/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/single-page/objects.json` & `quartodoc-0.4.0/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/examples/single-page/reference/index.qmd` & `quartodoc-0.4.0/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/ast.py` & `quartodoc-0.4.0/quartodoc/ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/autosummary.py` & `quartodoc-0.4.0/quartodoc/autosummary.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,32 +412,35 @@
             raise KeyError(f"A builder for style {cls.style} already exists")
 
         cls._registry[cls.style] = cls
 
     def __init__(
         self,
         package: str,
-        sections: "list[Any]",
+        # TODO: correct typing
+        sections: "list[Any]" = tuple(),
         version: "str | None" = None,
         dir: str = "reference",
         title: str = "Function reference",
         renderer: "dict | Renderer | str" = "markdown",
         out_index: str = None,
         sidebar: "str | None" = None,
         rewrite_all_pages=False,
         source_dir: "str | None" = None,
         dynamic: bool | None = None,
+        parser="numpy",
     ):
         self.layout = self.load_layout(sections=sections, package=package)
 
         self.package = package
         self.version = None
         self.dir = dir
         self.title = title
         self.sidebar = sidebar
+        self.parser = parser
 
         self.renderer = Renderer.from_config(renderer)
 
         if out_index is not None:
             self.out_index = out_index
 
         self.rewrite_all_pages = rewrite_all_pages
@@ -447,18 +450,20 @@
     def load_layout(self, sections: dict, package: str):
         # TODO: currently returning the list of sections, to make work with
         # previous code. We should make Layout a first-class citizen of the
         # process.
         try:
             return layout.Layout(sections=sections, package=package)
         except ValidationError as e:
-            msg = 'Configuration error for YAML:\n - '
+            msg = "Configuration error for YAML:\n - "
             errors = [fmt(err) for err in e.errors() if fmt(err)]
-            first_error = errors[0] # we only want to show one error at a time b/c it is confusing otherwise
-            msg += first_error           
+            first_error = errors[
+                0
+            ]  # we only want to show one error at a time b/c it is confusing otherwise
+            msg += first_error
             raise ValueError(msg) from None
 
     # building ----------------------------------------------------------------
 
     def build(self, filter: str = "*"):
         """Build index page, sphinx inventory, and individual doc pages.
 
@@ -476,15 +481,15 @@
             import sys
 
             sys.path.append(self.source_dir)
 
         # shaping and collection ----
 
         _log.info("Generating blueprint.")
-        blueprint = blueprint(self.layout, dynamic=self.dynamic)
+        blueprint = blueprint(self.layout, dynamic=self.dynamic, parser=self.parser)
 
         _log.info("Collecting pages and inventory items.")
         pages, items = collect(blueprint, base_dir=self.dir)
 
         # writing pages ----
 
         _log.info("Writing index")
```

### Comparing `quartodoc-0.3.5/quartodoc/builder/blueprint.py` & `quartodoc-0.4.0/quartodoc/builder/blueprint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 import logging
+import json
+import yaml
 
 from griffe import dataclasses as dc
 from griffe.loader import GriffeLoader
 from griffe.collections import ModulesCollection, LinesCollection
 from griffe.docstrings.parsers import Parser
 from functools import partial
+from textwrap import indent
 
 from plum import dispatch
 
 from quartodoc.layout import (
     MISSING,
     _Base,
     Auto,
@@ -27,14 +30,73 @@
 from .utils import PydanticTransformer, ctx_node, WorkaroundKeyError
 
 from typing import overload
 
 _log = logging.getLogger(__name__)
 
 
+def _auto_package(mod: dc.Module) -> list[Section]:
+    """Create default sections for the given package."""
+
+    import griffe.docstrings.dataclasses as ds
+
+    # get module members for content ----
+    contents = []
+    for name, member in mod.members.items():
+        external_alias = _is_external_alias(member, mod)
+        if external_alias or member.is_module or name.startswith("__"):
+            continue
+
+        contents.append(Auto(name=name))
+
+    # try to fetch a description of the module ----
+    mod_summary = mod.docstring.parsed[0]
+    if isinstance(mod_summary, ds.DocstringSectionText):
+        desc = mod_summary.value
+    else:
+        desc = ""
+
+    return [Section(title=mod.path, desc=desc, contents=contents)]
+
+
+def _is_external_alias(obj: dc.Alias | dc.Object, mod: dc.Module):
+    package_name = mod.path.split(".")[0]
+
+    if not isinstance(obj, dc.Alias):
+        return False
+
+    crnt_target = obj
+
+    while crnt_target.is_alias:
+        if not crnt_target.target_path.startswith(package_name):
+            return True
+
+        try:
+            new_target = crnt_target.modules_collection[crnt_target.target_path]
+
+            if new_target is crnt_target:
+                raise Exception(f"Cyclic Alias: {new_target}")
+
+            crnt_target = new_target
+
+        except KeyError:
+            # assumes everything from module was loaded, so target must
+            # be outside module
+            return True
+
+    return False
+
+
+def _to_simple_dict(el):
+    # round-trip to json, so we can take advantage of pydantic
+    # dumping Enums, etc.. There may be a simple way to do
+    # this in pydantic v2.
+    return json.loads(el.json(exclude_unset=True))
+
+
 class BlueprintTransformer(PydanticTransformer):
     def __init__(self, get_object=None, parser="numpy"):
 
         if get_object is None:
             loader = GriffeLoader(
                 docstring_parser=Parser(parser),
                 modules_collection=ModulesCollection(),
@@ -60,14 +122,21 @@
         except KeyError as e:
             key_name = e.args[0]
             raise WorkaroundKeyError(
                 f"Cannot find an object named: {key_name}."
                 f" Does an object with the path {path} exist?"
             )
 
+    @staticmethod
+    def _clean_member_path(path, new):
+        if ":" in new:
+            return new.replace(":", ".")
+
+        return new
+
     @dispatch
     def visit(self, el):
         # TODO: use a context handler
         self._log("VISITING", el)
 
         package = getattr(el, "package", MISSING())
         old = self.crnt_package
@@ -77,14 +146,48 @@
 
         try:
             return super().visit(el)
         finally:
             self.crnt_package = old
 
     @dispatch
+    def enter(self, el: Layout):
+        if not el.sections:
+            # TODO: should be shown all the time, not just logged,
+            # but also want to be able to disable (similar to pins)
+            print("Autogenerating contents (since no contents specified in config)")
+
+            package = el.package
+
+            mod = self.get_object_fixed(package)
+            sections = _auto_package(mod)
+
+            if not sections:
+                # TODO: informative message. When would this occur?
+                raise ValueError()
+
+            new_el = el.copy()
+            new_el.sections = sections
+
+            print(
+                "Use the following configuration to recreate the automatically",
+                " generated site:\n\n\n",
+                "quartodoc:\n",
+                indent(
+                    yaml.safe_dump(_to_simple_dict(new_el), sort_keys=False), " " * 2
+                ),
+                "\n",
+                sep="",
+            )
+
+            return super().enter(new_el)
+
+        return super().enter(el)
+
+    @dispatch
     def exit(self, el: Section):
         """Transform top-level sections, so their contents are all Pages."""
 
         node = ctx_node.get()
 
         # if we're not in a top-level section, then quit
         if not isinstance(node.parent.parent.value, Layout):
@@ -105,16 +208,18 @@
     def enter(self, el: Auto):
         self._log("Entering", el)
 
         # TODO: make this less brittle
         pkg = self.crnt_package
         if pkg is None:
             path = el.name
+        elif ":" in pkg or ":" in el.name:
+            path = f"{pkg}.{el.name}"
         else:
-            path = f"{pkg}.{el.name}" if ":" in el.name else f"{pkg}:{el.name}"
+            path = f"{pkg}:{el.name}"
 
         _log.info(f"Getting object for {path}")
 
         dynamic = el.dynamic if el.dynamic is not None else self.dynamic
 
         obj = self.get_object_fixed(path, dynamic=dynamic)
         raw_members = self._fetch_members(el, obj)
@@ -124,37 +229,46 @@
         children = []
         for entry in raw_members:
             # Note that we could have iterated over obj.members, but currently
             # if obj is an Alias to a class, then its members are not Aliases,
             # but the actual objects on the target.
             # On the other hand, we've wired get_object up to make sure getting
             # the member of an Alias also returns an Alias.
-            member_path = self._append_member_path(path, entry)
-            obj_member = self.get_object_fixed(member_path, dynamic=dynamic)
+            # member_path = self._append_member_path(path, entry)
+            relative_path = self._clean_member_path(path, entry)
+
+            # create Doc element for member ----
+            # TODO: when a member is a Class, it is currently created using
+            # defaults, and there is no way to override those.
+            doc = self.visit(Auto(name=relative_path, dynamic=dynamic, package=path))
 
             # do no document submodules
-            if obj_member.kind.value == "module":
+            if (
+                _is_external_alias(doc.obj, obj.package)
+                or doc.obj.kind.value == "module"
+            ):
                 continue
 
-            # create element for child ----
-            doc = Doc.from_griffe(obj_member.name, obj_member)
+            # obj_member = self.get_object_fixed(member_path, dynamic=dynamic)
+            # doc = Doc.from_griffe(obj_member.name, obj_member)
 
             # Case 1: make each member entry its own page
             if el.children == ChoicesChildren.separate:
-                res = MemberPage(path=obj_member.path, contents=[doc])
+                res = MemberPage(path=doc.obj.path, contents=[doc])
             # Case2: use just the Doc element, so it gets embedded directly
             # into the class being documented
             elif el.children in {ChoicesChildren.embedded, ChoicesChildren.flat}:
                 res = doc
             # Case 3: make each member just a link in a summary table.
             # if the page for the member is not created somewhere else, then it
             # won't exist in the documentation (but its summary will still be in
             # the table).
+            # TODO: we shouldn't even bother blueprinting these members.
             elif el.children == ChoicesChildren.linked:
-                res = Link(name=obj_member.path, obj=obj_member)
+                res = Link(name=doc.obj.path, obj=doc.obj)
             else:
                 raise ValueError(f"Unsupported value of children: {el.children}")
 
             children.append(res)
 
         is_flat = el.children == ChoicesChildren.flat
         return Doc.from_griffe(el.name, obj, members=children, flat=is_flat)
@@ -171,19 +285,22 @@
 
         if el.exclude:
             raise NotImplementedError("exclude argument currently unsupported.")
 
         if not el.include_private:
             options = {k: v for k, v in options.items() if not k.startswith("_")}
 
+        if not el.include_imports:
+            options = {k: v for k, v in options.items() if not v.is_alias}
+
         # for modules, remove any Alias objects, since they were imported from
         # other places. Sphinx has a flag for this behavior, so may be good
         # to do something similar.
-        if obj.is_module:
-            options = {k: v for k, v in options.items() if not v.is_alias}
+        # if obj.is_module:
+        #    options = {k: v for k, v in options.items() if not v.is_alias}
 
         return sorted(options)
 
 
 class _PagePackageStripper(PydanticTransformer):
     def __init__(self, package: str):
         self.package = package
@@ -201,15 +318,17 @@
 
 
 @overload
 def blueprint(el: Auto, package: str) -> Doc:
     ...
 
 
-def blueprint(el: _Base, package: str = None, dynamic: None | bool = None) -> _Base:
+def blueprint(
+    el: _Base, package: str = None, dynamic: None | bool = None, parser="numpy"
+) -> _Base:
     """Convert a configuration element to something that is ready to render.
 
     Parameters
     ----------
     el:
         An element, like layout.Auto, to transform.
     package:
@@ -226,15 +345,15 @@
     DocFunction(name='quartodoc.get_object', ...)
 
     >>> blueprint(Auto(name = "get_object"), package = "quartodoc")
     DocFunction(name='get_object', ...)
 
     """
 
-    trans = BlueprintTransformer()
+    trans = BlueprintTransformer(parser=parser)
 
     if package is not None:
         trans.crnt_package = package
 
     if dynamic is not None:
         trans.dynamic = dynamic
```

### Comparing `quartodoc-0.3.5/quartodoc/builder/collect.py` & `quartodoc-0.4.0/quartodoc/builder/collect.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/builder/utils.py` & `quartodoc-0.4.0/quartodoc/builder/utils.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/interlinks.py` & `quartodoc-0.4.0/quartodoc/interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/inventory.py` & `quartodoc-0.4.0/quartodoc/inventory.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/layout.py` & `quartodoc-0.4.0/quartodoc/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     ----------
     sections:
         Top-level sections of the quarto layout config.
     package:
         The package being documented.
     """
 
-    sections: list[Union[SectionElement, Section]]
+    sections: list[Union[SectionElement, Section]] = []
     package: Union[str, None, MISSING] = MISSING()
 
 
 # SubElements -----------------------------------------------------------------
 
 
 class Section(_Structural):
@@ -192,14 +192,16 @@
     kind:
     name:
         Name of the object. This should be the path needed to import it.
     members:
         A list of members, such as attributes or methods on a class, to document.
     include_private:
         Whether to include members starting with "_"
+    include_imports:
+        Whether to include members that were imported from somewhere else.
     include:
         (Not implemented). A list of members to include.
     exclude:
         (Not implemented). A list of members to exclude.
     dynamic:
         Whether to dynamically load docstring. By default docstrings are loaded
         using static analysis. dynamic may be a string pointing to another object,
@@ -212,14 +214,15 @@
 
     """
 
     kind: Literal["auto"] = "auto"
     name: str
     members: Optional[list[str]] = None
     include_private: bool = False
+    include_imports: bool = False
     include: Optional[str] = None
     exclude: Optional[str] = None
     dynamic: Union[None, bool, str] = None
     children: ChoicesChildren = ChoicesChildren.embedded
     package: Union[str, None, MISSING] = MISSING()
```

### Comparing `quartodoc-0.3.5/quartodoc/renderers/base.py` & `quartodoc-0.4.0/quartodoc/renderers/base.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/renderers/md_renderer.py` & `quartodoc-0.4.0/quartodoc/renderers/md_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,56 +245,71 @@
     def render(self, el: layout.Doc):
         raise NotImplementedError(f"Unsupported Doc type: {type(el)}")
 
     @dispatch
     def render(self, el: Union[layout.DocClass, layout.DocModule]):
         title = self.render_header(el)
 
-        extra_parts = []
+        attr_docs = []
         meth_docs = []
+        class_docs = []
+
         if el.members:
             sub_header = "#" * (self.crnt_header_level + 1)
             raw_attrs = [x for x in el.members if x.obj.is_attribute]
             raw_meths = [x for x in el.members if x.obj.is_function]
+            raw_classes = [x for x in el.members if x.obj.is_class]
 
 
             header = "| Name | Description |\n| --- | --- |"
 
             # attribute summary table ----
             # docstrings can define an attributes section. If that exists on
             # then we skip summarizing each attribute into a table.
             # TODO: for now, we skip making an attribute table on classes, unless
             # they contain an attributes section in the docstring
             if (
                     raw_attrs
                     and not _has_attr_section(el.obj.docstring)
-                    and not isinstance(el, layout.DocClass)
+                    # TODO: what should backwards compat be?
+                    # and not isinstance(el, layout.DocClass)
                 ):
 
                 _attrs_table = "\n".join(map(self.summarize, raw_attrs))
                 attrs = f"{sub_header} Attributes\n\n{header}\n{_attrs_table}"
-                extra_parts.append(attrs)
+                attr_docs.append(attrs)
+            
+            # classes summary table ----
+            if raw_classes:
+                _summary_table = "\n".join(map(self.summarize, raw_classes))
+                section_name = "Classes"
+                objs = f"{sub_header} {section_name}\n\n{header}\n{_summary_table}"
+                class_docs.append(objs)
+
+                n_incr = 1 if el.flat else 2
+                with self._increment_header(n_incr):
+                    class_docs.extend([self.render(x) for x in raw_classes if isinstance(x, layout.Doc)])
 
             # method summary table ----
             if raw_meths:
-                _meths_table = "\n".join(map(self.summarize, raw_meths))
+                _summary_table = "\n".join(map(self.summarize, raw_meths))
                 section_name = (
                     "Methods" if isinstance(el, layout.DocClass)
                     else "Functions"
                 )
-                meths = f"{sub_header} {section_name}\n\n{header}\n{_meths_table}"
-                extra_parts.append(meths)
+                objs = f"{sub_header} {section_name}\n\n{header}\n{_summary_table}"
+                meth_docs.append(objs)
 
                 # TODO use context manager, or context variable?
                 n_incr = 1 if el.flat else 2
                 with self._increment_header(n_incr):
-                    meth_docs = [self.render(x) for x in raw_meths if isinstance(x, layout.Doc)]
+                    meth_docs.extend([self.render(x) for x in raw_meths if isinstance(x, layout.Doc)])
 
         body = self.render(el.obj)
-        return "\n\n".join([title, body, *extra_parts, *meth_docs])
+        return "\n\n".join([title, body, *attr_docs, *class_docs, *meth_docs])
 
     @dispatch
     def render(self, el: layout.DocFunction):
         title = self.render_header(el)
 
         return "\n\n".join([title, self.render(el.obj)])
```

### Comparing `quartodoc-0.3.5/quartodoc/tests/example_dynamic.py` & `quartodoc-0.4.0/quartodoc/tests/example_dynamic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/example_interlinks/interlinks.lua` & `quartodoc-0.4.0/quartodoc/tests/example_interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/example_interlinks/objects.json` & `quartodoc-0.4.0/quartodoc/tests/example_interlinks/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/example_interlinks/spec.yml` & `quartodoc-0.4.0/quartodoc/tests/example_interlinks/spec.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.md` & `quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/example_interlinks/test.qmd` & `quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_ast.py` & `quartodoc-0.4.0/quartodoc/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_basic.py` & `quartodoc-0.4.0/quartodoc/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_builder.py` & `quartodoc-0.4.0/quartodoc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_builder_blueprint.py` & `quartodoc-0.4.0/quartodoc/tests/test_builder_blueprint.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,7 +102,18 @@
     with pytest.raises(WorkaroundKeyError) as exc_info:
         bp.visit(auto)
 
     assert (
         "Does an object with the path quartodoc.bbb.ccc exist?"
         in exc_info.value.args[0]
     )
+
+
+def test_blueprint_auto_package(bp):
+    layout = blueprint(lo.Layout(package="quartodoc.tests.example"))
+    sections = layout.sections
+    assert len(sections) == 1
+    assert sections[0].title == "quartodoc.tests.example"
+    assert sections[0].desc == "A module"
+
+    # 4 objects documented
+    assert len(sections[0].contents) == 4
```

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_interlinks.py` & `quartodoc-0.4.0/quartodoc/tests/test_interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_layout.py` & `quartodoc-0.4.0/quartodoc/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_renderers.py` & `quartodoc-0.4.0/quartodoc/tests/test_renderers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import griffe.docstrings.dataclasses as ds
 import griffe.expressions as exp
 
 from quartodoc.renderers import MdRenderer
-from quartodoc import get_object
+from quartodoc import Auto, blueprint, get_object
 
 
 @pytest.fixture
 def renderer():
     return MdRenderer()
 
 
@@ -61,17 +61,39 @@
 
     res = renderer.render(pars)
     assert interlink in res
 
 
 def test_render_doc_attribute(renderer):
     attr = ds.DocstringAttribute(
-        name = "abc",
+        name="abc",
         description="xyz",
         annotation=exp.Expression(exp.Name("Optional", full="Optional"), "[", "]"),
-        value=1
+        value=1,
     )
 
     res = renderer.render(attr)
 
-    assert res == ["abc", "Optional\[\]", "xyz"]
+    assert res == ["abc", r"Optional\[\]", "xyz"]
 
+
+@pytest.mark.parametrize("children", ["embedded", "flat"])
+def test_render_doc_module(snapshot, renderer, children):
+    bp = blueprint(Auto(name="quartodoc.tests.example", children=children))
+    res = renderer.render(bp)
+
+    assert res == snapshot
+
+
+@pytest.mark.parametrize("children", ["embedded", "flat"])
+def test_render_doc_class(snapshot, renderer, children):
+    bp = blueprint(Auto(name="quartodoc.tests.example_class.C", children=children))
+    res = renderer.render(bp)
+
+    assert res == snapshot
+
+
+def test_render_doc_class_attributes_section(snapshot, renderer):
+    bp = blueprint(Auto(name="quartodoc.tests.example_class.AttributesTable"))
+    res = renderer.render(bp)
+
+    assert res == snapshot
```

### Comparing `quartodoc-0.3.5/quartodoc/tests/test_validation.py` & `quartodoc-0.4.0/quartodoc/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc/validation.py` & `quartodoc-0.4.0/quartodoc/validation.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.4.0/quartodoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.5
+Version: 0.4.0
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.3.5/quartodoc.egg-info/SOURCES.txt` & `quartodoc-0.4.0/quartodoc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 docs/get-started/docstring-style.qmd
 docs/get-started/extending.qmd
 docs/get-started/extra-build-sequence.qmd
 docs/get-started/interlinks.qmd
 docs/get-started/overview.qmd
 docs/get-started/sidebar.qmd
 examples/.gitignore
+examples/auto-package/_quarto.yml
 examples/dascore/.gitignore
 examples/dascore/_quarto.yml
 examples/dascore/generate_api.py
 examples/dascore/index.md
 examples/pkgdown/.gitignore
 examples/pkgdown/_quarto.yml
 examples/pkgdown/objects.json
@@ -83,24 +84,26 @@
 quartodoc/renderers/__init__.py
 quartodoc/renderers/base.py
 quartodoc/renderers/md_renderer.py
 quartodoc/tests/__init__.py
 quartodoc/tests/example.py
 quartodoc/tests/example_alias_target.py
 quartodoc/tests/example_attribute.py
+quartodoc/tests/example_class.py
 quartodoc/tests/example_dynamic.py
 quartodoc/tests/example_signature.py
 quartodoc/tests/test_ast.py
 quartodoc/tests/test_basic.py
 quartodoc/tests/test_builder.py
 quartodoc/tests/test_builder_blueprint.py
 quartodoc/tests/test_interlinks.py
 quartodoc/tests/test_layout.py
 quartodoc/tests/test_renderers.py
 quartodoc/tests/test_validation.py
+quartodoc/tests/__snapshots__/test_renderers.ambr
 quartodoc/tests/example_interlinks/.gitignore
 quartodoc/tests/example_interlinks/README.md
 quartodoc/tests/example_interlinks/_quarto.yml
 quartodoc/tests/example_interlinks/interlinks.lua
 quartodoc/tests/example_interlinks/objects.json
 quartodoc/tests/example_interlinks/spec.yml
 quartodoc/tests/example_interlinks/test.md
```

### Comparing `quartodoc-0.3.5/requirements-dev.txt` & `quartodoc-0.4.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/scripts/filter-spec/generate_files.py` & `quartodoc-0.4.0/scripts/filter-spec/generate_files.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.5/setup.cfg` & `quartodoc-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -26,28 +26,27 @@
 	sphobjinv>=2.3.1
 	tabulate>=0.9.0
 	importlib-metadata>=5.1.0
 	importlib-resources>=5.10.2
 	pydantic<2.0
 	pyyaml
 	typing-extensions>=4.4.0
+	watchdog>=3.0.0
 
 [options.extras_require]
 dev = 
 	pytest
 	jupyterlab
 	jupytext
+	syrupy
 
 [options.entry_points]
 console_scripts = 
 	quartodoc = quartodoc.__main__:cli
 
-[project.scripts]
-quartodoc = "quartodoc.cli:main"
-
 [bdist_wheel]
 universal = 1
 
 [flake8]
 exclude = docs
 max-line-length = 90
 ignore =
```

