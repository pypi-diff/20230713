# Comparing `tmp/sp_repo_review-2023.7.13.tar.gz` & `tmp/sp_repo_review-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Jul 13 17:47:34 2023, max compression
+gzip compressed data, last modified: Thu Jul  6 19:13:47 2023, max compression
```

## Comparing `sp_repo_review-2023.7.13.tar` & `sp_repo_review-2023.7.6.tar`

### file list

```diff
@@ -1,132 +1,130 @@
--rw-r--r--   0        0        0      125 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.git_archival.txt
--rw-r--r--   0        0        0       45 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.gitattributes
--rw-r--r--   0        0        0     2559 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.pre-commit-config.yaml
--rw-r--r--   0        0        0      179 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      702 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.readthedocs.yaml
--rw-r--r--   0        0        0        6 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.ruby-version
--rw-r--r--   0        0        0     1182 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/Gemfile
--rw-r--r--   0        0        0     3683 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/Gemfile.lock
--rw-r--r--   0        0        0    18757 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/README.md
--rw-r--r--   0        0        0     1020 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/_config.yml
--rw-r--r--   0        0        0      763 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/action.yml
--rw-r--r--   0        0        0     1208 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/cookiecutter.json
--rw-r--r--   0        0        0     2691 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/copier.yml
--rw-r--r--   0        0        0    11663 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/noxfile.py
--rw-r--r--   0        0        0      527 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      162 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.github/dependabot.yml
--rw-r--r--   0        0        0      825 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.github/workflows/bump.yml
--rw-r--r--   0        0        0      726 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1219 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2109 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.github/workflows/reusable-change-detection.yml
--rw-r--r--   0        0        0     5295 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.github/workflows/reusable-cookie.yml
--rw-r--r--   0        0        0     1262 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.github/workflows/reusable-rr-tests.yml
--rw-r--r--   0        0        0      251 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/LICENSE
--rw-r--r--   0        0        0      829 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/README.md
--rw-r--r--   0        0        0     2180 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_includes/head.html
--rw-r--r--   0        0        0     1019 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_includes/head_custom.html
--rw-r--r--   0        0        0      547 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_includes/interactive_repo_review.html
--rw-r--r--   0        0        0     2753 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_includes/pyproject.md
--rw-r--r--   0        0        0      145 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_includes/toc.html
--rw-r--r--   0        0        0      435 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_plugins/details.rb
--rw-r--r--   0        0        0      512 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_plugins/repo_review.rb
--rw-r--r--   0        0        0     1541 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_plugins/tabs.rb
--rw-r--r--   0        0        0       22 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_sass/color_schemes/skhep.scss
--rw-r--r--   0        0        0     2627 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/_sass/custom/custom.scss
--rw-r--r--   0        0        0    15086 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/assets/favicon.ico
--rw-r--r--   0        0        0     8070 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      652 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/assets/js/tabs.js
--rw-r--r--   0        0        0    10215 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/assets/js/webapp.js
--rw-r--r--   0        0        0     4104 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/index.md
--rw-r--r--   0        0        0     5085 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/coverage.md
--rw-r--r--   0        0        0     9872 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/docs.md
--rw-r--r--   0        0        0    22978 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/gha_basic.md
--rw-r--r--   0        0        0     7836 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/gha_pure.md
--rw-r--r--   0        0        0     8067 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/gha_wheels.md
--rw-r--r--   0        0        0     2956 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/index.md
--rw-r--r--   0        0        0    10386 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/mypy.md
--rw-r--r--   0        0        0    18232 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/packaging_classic.md
--rw-r--r--   0        0        0     9364 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/packaging_compiled.md
--rw-r--r--   0        0        0     6187 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/packaging_simple.md
--rw-r--r--   0        0        0    14312 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/pytest.md
--rw-r--r--   0        0        0      947 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/repo_review.md
--rw-r--r--   0        0        0    28348 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/style.md
--rw-r--r--   0        0        0     9121 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/guides/tasks.md
--rw-r--r--   0        0        0     4260 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/patterns/backports.md
--rw-r--r--   0        0        0     7171 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/patterns/data_files.md
--rw-r--r--   0        0        0     3119 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/patterns/exports.md
--rw-r--r--   0        0        0      738 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/patterns/index.md
--rw-r--r--   0        0        0    11212 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/principles/design.md
--rw-r--r--   0        0        0      561 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/principles/index.md
--rw-r--r--   0        0        0     2209 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/principles/process.md
--rw-r--r--   0        0        0     4526 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/tutorials/dev-environment.md
--rw-r--r--   0        0        0     4795 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/tutorials/docs.md
--rw-r--r--   0        0        0      998 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/tutorials/index.md
--rw-r--r--   0        0        0     2578 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/tutorials/module.md
--rw-r--r--   0        0        0     3300 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/tutorials/packaging.md
--rw-r--r--   0        0        0     4645 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/docs/pages/tutorials/test.md
--rw-r--r--   0        0        0      908 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/helpers/cog_cc.py
--rw-r--r--   0        0        0      615 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/helpers/cog_helpers.py
--rw-r--r--   0        0        0      699 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/helpers/extensions.py
--rw-r--r--   0        0        0      246 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/__init__.py
--rw-r--r--   0        0        0      168 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/_version.pyi
--rw-r--r--   0        0        0      822 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/families.py
--rw-r--r--   0        0        0        0 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0      152 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     2849 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/general.py
--rw-r--r--   0        0        0     5018 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/github.py
--rw-r--r--   0        0        0     4133 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     3154 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     5339 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2565 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/readthedocs.py
--rw-r--r--   0        0        0     3006 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/src/sp_repo_review/checks/ruff.py
--rw-r--r--   0        0        0      412 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/tests/test_cmd.py
--rw-r--r--   0        0        0      597 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/tests/test_package.py
--rw-r--r--   0        0        0      125 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.gitattributes
--rw-r--r--   0        0        0     2218 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2901 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.readthedocs.yml
--rw-r--r--   0        0        0     1689 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0     2928 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/noxfile.py
--rw-r--r--   0        0        0     8661 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0     3987 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}
--rw-r--r--   0        0        0      169 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
--rw-r--r--   0        0        0     2197 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
--rw-r--r--   0        0        0      691 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
--rw-r--r--   0        0        0      915 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
--rw-r--r--   0        0        0      727 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
--rw-r--r--   0        0        0      376 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
--rw-r--r--   0        0        0      266 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
--rw-r--r--   0        0        0    11380 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1559 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}
--rw-r--r--   0        0        0     1089 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}
--rw-r--r--   0        0        0      102 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
--rw-r--r--   0        0        0     2528 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/dependabot.yml
--rwxr-xr-x   0        0        0      978 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}
--rw-r--r--   0        0        0      668 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1912 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1597 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type!='compiled' %}cd.yml{% endif %}
--rw-r--r--   0        0        0     1573 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}
--rw-r--r--   0        0        0      934 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      218 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/docs/index.md
--rw-r--r--   0        0        0      632 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
--rw-r--r--   0        0        0      562 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
--rw-r--r--   0        0        0      422 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
--rw-r--r--   0        0        0      117 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
--rw-r--r--   0        0        0      118 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.backend in ['setuptools', 'pybind11'] %}_version.pyi{% endif %}
--rw-r--r--   0        0        0      215 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/__init__.py
--rw-r--r--   0        0        0      573 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py
--rw-r--r--   0        0        0      378 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/tests/test_package.py
--rw-r--r--   0        0        0      190 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
--rw-r--r--   0        0        0     2289 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/.gitignore
--rw-r--r--   0        0        0     1525 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/LICENSE
--rw-r--r--   0        0        0     5530 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/pyproject.toml
--rw-r--r--   0        0        0    10038 2023-07-13 17:47:34.000000 sp_repo_review-2023.7.13/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.git_archival.txt
+-rw-r--r--   0        0        0       45 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.gitattributes
+-rw-r--r--   0        0        0     2547 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      179 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      702 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.readthedocs.yaml
+-rw-r--r--   0        0        0        6 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.ruby-version
+-rw-r--r--   0        0        0     1042 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/Gemfile
+-rw-r--r--   0        0        0     2737 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/Gemfile.lock
+-rw-r--r--   0        0        0    18677 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/README.md
+-rw-r--r--   0        0        0     1057 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/_config.yml
+-rw-r--r--   0        0        0      763 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/action.yml
+-rw-r--r--   0        0        0      877 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/cookiecutter.json
+-rw-r--r--   0        0        0     2120 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/copier.yml
+-rw-r--r--   0        0        0    11663 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/noxfile.py
+-rw-r--r--   0        0        0      640 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      162 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      825 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      726 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1219 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2109 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-change-detection.yml
+-rw-r--r--   0        0        0     5295 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-cookie.yml
+-rw-r--r--   0        0        0     1262 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.github/workflows/reusable-rr-tests.yml
+-rw-r--r--   0        0        0      251 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/LICENSE
+-rw-r--r--   0        0        0      829 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/README.md
+-rw-r--r--   0        0        0     2180 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/head.html
+-rw-r--r--   0        0        0     1019 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/head_custom.html
+-rw-r--r--   0        0        0      545 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/interactive_repo_review.html
+-rw-r--r--   0        0        0     2753 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/pyproject.md
+-rw-r--r--   0        0        0      145 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_includes/toc.html
+-rw-r--r--   0        0        0      435 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/details.rb
+-rw-r--r--   0        0        0      512 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/repo_review.rb
+-rw-r--r--   0        0        0     1541 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_plugins/tabs.rb
+-rw-r--r--   0        0        0       22 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_sass/color_schemes/skhep.scss
+-rw-r--r--   0        0        0     2611 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/_sass/custom/custom.scss
+-rw-r--r--   0        0        0    15086 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     8070 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      652 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/js/tabs.js
+-rw-r--r--   0        0        0    10211 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/assets/js/webapp.js
+-rw-r--r--   0        0        0     3322 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/index.md
+-rw-r--r--   0        0        0     5085 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/coverage.md
+-rw-r--r--   0        0        0     9872 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/docs.md
+-rw-r--r--   0        0        0    22870 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_basic.md
+-rw-r--r--   0        0        0     7836 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_pure.md
+-rw-r--r--   0        0        0     8067 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/gha_wheels.md
+-rw-r--r--   0        0        0     2956 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/index.md
+-rw-r--r--   0        0        0    10386 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/mypy.md
+-rw-r--r--   0        0        0    18232 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_classic.md
+-rw-r--r--   0        0        0     9364 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_compiled.md
+-rw-r--r--   0        0        0     6194 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/packaging_simple.md
+-rw-r--r--   0        0        0    14312 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/pytest.md
+-rw-r--r--   0        0        0      947 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/repo_review.md
+-rw-r--r--   0        0        0    28349 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/style.md
+-rw-r--r--   0        0        0     9121 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/guides/tasks.md
+-rw-r--r--   0        0        0     4260 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/backports.md
+-rw-r--r--   0        0        0     7171 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/data_files.md
+-rw-r--r--   0        0        0     3119 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/exports.md
+-rw-r--r--   0        0        0      738 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/patterns/index.md
+-rw-r--r--   0        0        0    11217 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/design.md
+-rw-r--r--   0        0        0      561 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/index.md
+-rw-r--r--   0        0        0     2209 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/principles/process.md
+-rw-r--r--   0        0        0     4526 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/dev-environment.md
+-rw-r--r--   0        0        0     4795 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/docs.md
+-rw-r--r--   0        0        0      998 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/index.md
+-rw-r--r--   0        0        0     2578 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/module.md
+-rw-r--r--   0        0        0     3300 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/packaging.md
+-rw-r--r--   0        0        0     4645 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/docs/pages/tutorials/test.md
+-rw-r--r--   0        0        0      615 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/helpers/cog_helpers.py
+-rw-r--r--   0        0        0      699 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/helpers/extensions.py
+-rw-r--r--   0        0        0      246 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/__init__.py
+-rw-r--r--   0        0        0      166 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_version.pyi
+-rw-r--r--   0        0        0      822 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/families.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      152 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2849 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/general.py
+-rw-r--r--   0        0        0     5018 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/github.py
+-rw-r--r--   0        0        0     4133 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3154 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5339 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2565 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/readthedocs.py
+-rw-r--r--   0        0        0     3002 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/src/sp_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0      412 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/tests/test_cmd.py
+-rw-r--r--   0        0        0      597 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/tests/test_package.py
+-rw-r--r--   0        0        0      125 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitattributes
+-rw-r--r--   0        0        0     2218 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2901 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.readthedocs.yml
+-rw-r--r--   0        0        0     1689 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0     2928 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/noxfile.py
+-rw-r--r--   0        0        0     8661 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0     3987 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.__ci == 'gitlab' %}.gitlab-ci.yml{% endif %}
+-rw-r--r--   0        0        0      169 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
+-rw-r--r--   0        0        0     2197 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
+-rw-r--r--   0        0        0      691 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
+-rw-r--r--   0        0        0      915 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
+-rw-r--r--   0        0        0      727 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      376 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
+-rw-r--r--   0        0        0      266 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
+-rw-r--r--   0        0        0    11380 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1559 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'BSD' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0     1089 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'MIT' %}LICENSE{% endif %}
+-rw-r--r--   0        0        0      102 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
+-rw-r--r--   0        0        0     2528 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/dependabot.yml
+-rwxr-xr-x   0        0        0      978 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}
+-rw-r--r--   0        0        0      668 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     3424 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1573 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}
+-rw-r--r--   0        0        0      934 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      218 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/index.md
+-rw-r--r--   0        0        0      632 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
+-rw-r--r--   0        0        0      562 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
+-rw-r--r--   0        0        0      422 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
+-rw-r--r--   0        0        0      117 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
+-rw-r--r--   0        0        0      118 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.backend in ['setuptools', 'pybind11'] %}_version.pyi{% endif %}
+-rw-r--r--   0        0        0      215 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py
+-rw-r--r--   0        0        0      378 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/tests/test_package.py
+-rw-r--r--   0        0        0      190 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
+-rw-r--r--   0        0        0     2249 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/.gitignore
+-rw-r--r--   0        0        0     1525 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/LICENSE
+-rw-r--r--   0        0        0     5530 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/pyproject.toml
+-rw-r--r--   0        0        0    10037 2023-07-06 19:13:47.000000 sp_repo_review-2023.7.6/PKG-INFO
```

### Comparing `sp_repo_review-2023.7.13/.pre-commit-config.yaml` & `sp_repo_review-2023.7.6/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,26 @@
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 exclude: "^({{cookiecutter\\.project_name}}|hooks/pre_gen_project.py$)"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: "23.7.0"
+    rev: "23.3.0"
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: "1.15.0"
+    rev: "1.14.0"
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.7.0]
+        additional_dependencies: [black==23.3.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.277"
+    rev: "v0.0.276"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.4.0"
     hooks:
@@ -57,15 +57,15 @@
           - pytest
           - repo-review
           - rich
           - tomli
           - types-PyYAML
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0"
+    rev: "v2.7.1"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.5"
@@ -85,9 +85,9 @@
         name: Disallow _ in permalinks
         language: pygrep
         entry: "^permalink:.*_.*"
       - id: cog
         name: Cog the pages
         language: python
         entry: cog -P -r -I ./helpers
-        files: "^docs/pages/guides/(packaging_compiled|docs).md|^copier.yml"
+        files: "^docs/pages/guides/(packaging_compiled|docs).md"
         additional_dependencies: [cogapp, cookiecutter]
```

### Comparing `sp_repo_review-2023.7.13/.readthedocs.yaml` & `sp_repo_review-2023.7.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/Gemfile` & `sp_repo_review-2023.7.6/Gemfile`

 * *Files 14% similar despite different names*

```diff
@@ -24,19 +24,14 @@
   gem 'jekyll-feed'
   gem 'jekyll-seo-tag'
 end
 
 group :development do
   # Verify good coding practices in Ruby files
   gem 'rubocop', '~>1.52', require: false
-
-  # Check links. Use:
-  #   bundle exec jekyll build
-  #   bundle exec htmlproofer --assume_extension '.html' ./_site
-  gem 'html-proofer'
 end
 
 # Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
 # and associated library.
 platforms :mingw, :x64_mingw, :mswin, :jruby do
   gem "tzinfo", ">= 1", "< 3"
   gem "tzinfo-data"
```

### Comparing `sp_repo_review-2023.7.13/Gemfile.lock` & `sp_repo_review-2023.7.6/Gemfile.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,26 @@
 GEM
   remote: https://rubygems.org/
   specs:
-    Ascii85 (1.1.0)
     addressable (2.8.4)
       public_suffix (>= 2.0.2, < 6.0)
-    afm (0.2.2)
     ast (2.4.2)
-    async (2.6.2)
-      console (~> 1.10)
-      fiber-annotation
-      io-event (~> 1.1)
-      timers (~> 4.1)
     colorator (1.1.0)
     concurrent-ruby (1.2.2)
-    console (1.17.2)
-      fiber-annotation
-      fiber-local
     em-websocket (0.5.3)
       eventmachine (>= 0.12.9)
       http_parser.rb (~> 0)
-    ethon (0.16.0)
-      ffi (>= 1.15.0)
     eventmachine (1.2.7)
     ffi (1.15.5)
-    fiber-annotation (0.2.0)
-    fiber-local (1.0.0)
     forwardable-extended (2.6.0)
     google-protobuf (3.23.3-x86_64-darwin)
     google-protobuf (3.23.3-x86_64-linux)
-    hashery (2.1.2)
-    html-proofer (5.0.7)
-      addressable (~> 2.3)
-      async (~> 2.1)
-      nokogiri (~> 1.13)
-      pdf-reader (~> 2.11)
-      rainbow (~> 3.0)
-      typhoeus (~> 1.3)
-      yell (~> 2.0)
-      zeitwerk (~> 2.5)
     http_parser.rb (0.8.0)
     i18n (1.14.1)
       concurrent-ruby (~> 1.0)
-    io-event (1.2.2)
     jekyll (4.3.2)
       addressable (~> 2.4)
       colorator (~> 1.0)
       em-websocket (~> 0.5)
       i18n (~> 1.0)
       jekyll-sass-converter (>= 2.0, < 4.0)
       jekyll-watch (~> 2.0)
@@ -76,30 +51,20 @@
     kramdown-parser-gfm (1.1.0)
       kramdown (~> 2.0)
     liquid (4.0.4)
     listen (3.8.0)
       rb-fsevent (~> 0.10, >= 0.10.3)
       rb-inotify (~> 0.9, >= 0.9.10)
     mercenary (0.4.0)
-    nokogiri (1.15.3-x86_64-darwin)
-      racc (~> 1.4)
-    nokogiri (1.15.3-x86_64-linux)
-      racc (~> 1.4)
     parallel (1.23.0)
     parser (3.2.2.3)
       ast (~> 2.4.1)
       racc
     pathutil (0.16.2)
       forwardable-extended (~> 2.6)
-    pdf-reader (2.11.0)
-      Ascii85 (~> 1.0)
-      afm (~> 0.2.1)
-      hashery (~> 2.0)
-      ruby-rc4
-      ttfunk
     public_suffix (5.0.1)
     racc (1.7.1)
     rainbow (3.1.1)
     rake (13.0.6)
     rb-fsevent (0.11.2)
     rb-inotify (0.10.1)
       ffi (~> 1.0)
@@ -115,37 +80,29 @@
       rexml (>= 3.2.5, < 4.0)
       rubocop-ast (>= 1.28.0, < 2.0)
       ruby-progressbar (~> 1.7)
       unicode-display_width (>= 2.4.0, < 3.0)
     rubocop-ast (1.29.0)
       parser (>= 3.2.1.0)
     ruby-progressbar (1.13.0)
-    ruby-rc4 (0.1.5)
     safe_yaml (1.0.5)
     sass-embedded (1.63.6)
       google-protobuf (~> 3.23)
       rake (>= 13.0.0)
     terminal-table (3.0.2)
       unicode-display_width (>= 1.1.1, < 3)
-    timers (4.3.5)
-    ttfunk (1.7.0)
-    typhoeus (1.4.0)
-      ethon (>= 0.9.0)
     unicode-display_width (2.4.2)
     wdm (0.1.1)
     webrick (1.8.1)
-    yell (2.2.2)
-    zeitwerk (2.6.8)
 
 PLATFORMS
   x86_64-darwin-21
   x86_64-linux
 
 DEPENDENCIES
-  html-proofer
   jekyll (~> 4.3)
   jekyll-feed
   jekyll-seo-tag
   just-the-docs (~> 0.5.3)
   kramdown-parser-gfm
   rubocop (~> 1.52)
   tzinfo (>= 1, < 3)
```

### Comparing `sp_repo_review-2023.7.13/README.md` & `sp_repo_review-2023.7.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,14 @@
 otherwise with `pipx install cookiecutter` (or prepend `pipx run` to the command
 below, and skip installation). Then run:
 
 ```bash
 cookiecutter gh:scientific-python/cookie
 ```
 
-If you are using cookiecutter 2.2+, you will get descriptions for the options.
-
 #### To use (classic cruft version)
 
 You can also use [cruft][], which adds the ability update to cookiecutter
 projects. Install with `pipx install cruft` (or prepend `pipx run` to the
 command below, and skip installation). Then run:
 
 ```bash
```

### Comparing `sp_repo_review-2023.7.13/_config.yml` & `sp_repo_review-2023.7.6/_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 title: Scientific Python Development Guide
 email: guide@scientific-python.org
 description: >-
   This guide is maintained by the scientific Python community for the benefit of
   fellow scientists and research software engineers.
+url: "https://learn.scientific-python.org"
 github_username: scientific-python
 source: docs
 
 # Build settings
 markdown: kramdown
 theme: "just-the-docs"
 plugins:
@@ -18,15 +19,15 @@
 
 # Enable or disable the site search
 search_enabled: true
 
 # Aux links for the upper right navigation
 aux_links:
   "Scientific Python Cookie":
-    - "https://github.com/scientific-python/cookie"
+    - "//github.com/scientific-python/cookie"
 
 gh_edit_link: true
 gh_edit_link_text: "View source for this page on GitHub."
 gh_edit_repository: "https://github.com/scientific-python/cookie"
 gh_edit_branch: "main"
 gh_edit_source: "docs"
 gh_edit_view_mode: "tree" # "tree" or "edit"
```

### Comparing `sp_repo_review-2023.7.13/action.yml` & `sp_repo_review-2023.7.6/action.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/copier.yml` & `sp_repo_review-2023.7.6/copier.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,55 @@
-# [[[cog
-# from cog_cc import CC
-#
-# cc = CC("cookiecutter.json")
-# ]]]
-# [[[end]]]
-
-# [[[cog print(cc.project_name.yaml()) ]]]
 project_name:
   type: str
   help: The name of your project
-  # [[[end]]]
   validator: >-
     {% if not project_name %} You must provide a name for the project. {% endif
     %}
 
-# [[[cog print(cc.org.yaml()) ]]]
 org:
   type: str
   help: The name of your (GitHub?) org
-  # [[[end]]]
   validator: >-
     {% if not org %} You must provide a org for the project. It might just be
     your user name on the site (like GitHub) you are targeting. {% endif %}
 
-# [[[cog print(cc.url.yaml()) ]]]
 url:
   type: str
-  help: The url to your GitHub or GitLab repository
-  #[[[end]]]
+  help: The URL for your repository
   default: "https://github.com/{{ org }}/{{ project_name }}"
 
-# [[[cog print(cc.full_name.yaml()) ]]]
 full_name:
   type: str
   help: Your name
-  # [[[end]]]
   placeholder: My Name
   validator: >-
     {% if not full_name %} You must provide a name (possibly yours) to place in
     your config files. {% endif %}
 
-# [[[cog print(cc.email.yaml()) ]]]
 email:
   type: str
   help: Your email
-  #[[[end]]]
   placeholder: me@email.com
   validator: >-
     {% if not email %} You must provide an email (possibly yours) to place in
     your config files, as required by PyPI. {% endif %}
 
-# [[[cog print(cc.project_short_description.yaml()) ]]]
 project_short_description:
   type: str
-  help: A short description of your project
-  #[[[end]]]
   default: A great package.
 
-# [[[cog print(cc.license.yaml()) ]]]
 license:
   help: Select a license
-  #[[[end]]]
   choices:
     - BSD
     - Apache
     - MIT
 
-# [[[cog print(cc.backend.yaml()) ]]]
 backend:
   help: Choose a build backend
-  #[[[end]]]
   choices:
     "Hatchling                      - Pure Python (recommended)": hatch
     "Flit-core                      - Pure Python (minimal)": flit
     "PDM-backend                    - Pure Python": pdm
     "Trampolim                      - Pure Python": trampolim
     "Whey                           - Pure Python": whey
     "Poetry                         - Pure Python": poetry
```

### Comparing `sp_repo_review-2023.7.13/noxfile.py` & `sp_repo_review-2023.7.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/.devcontainer/devcontainer.json` & `sp_repo_review-2023.7.6/.devcontainer/devcontainer.json`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,40 @@
-00000000: 7b0a 2020 226e 616d 6522 3a20 2273 6369  {.  "name": "sci
-00000010: 656e 7469 6669 632d 7079 7468 6f6e 2d63  entific-python-c
-00000020: 6f6f 6b69 655b 6465 765d 222c 0a20 2022  ookie[dev]",.  "
-00000030: 696d 6167 6522 3a20 226d 6372 2e6d 6963  image": "mcr.mic
-00000040: 726f 736f 6674 2e63 6f6d 2f64 6576 636f  rosoft.com/devco
-00000050: 6e74 6169 6e65 7273 2f70 7974 686f 6e3a  ntainers/python:
-00000060: 302d 332e 3131 222c 0a20 2022 6665 6174  0-3.11",.  "feat
-00000070: 7572 6573 223a 207b 0a20 2020 2022 6768  ures": {.    "gh
-00000080: 6372 2e69 6f2f 6465 7663 6f6e 7461 696e  cr.io/devcontain
-00000090: 6572 732f 6665 6174 7572 6573 2f72 7573  ers/features/rus
-000000a0: 743a 3122 3a20 7b7d 2c0a 2020 2020 2267  t:1": {},.    "g
-000000b0: 6863 722e 696f 2f64 6576 636f 6e74 6169  hcr.io/devcontai
-000000c0: 6e65 7273 2f66 6561 7475 7265 732f 7275  ners/features/ru
-000000d0: 6279 3a31 223a 207b 0a20 2020 2020 2022  by:1": {.      "
-000000e0: 7665 7273 696f 6e22 3a20 2233 2e31 220a  version": "3.1".
-000000f0: 2020 2020 7d0a 2020 7d2c 0a20 2022 706f      }.  },.  "po
-00000100: 7374 4372 6561 7465 436f 6d6d 616e 6422  stCreateCommand"
-00000110: 3a20 2270 6970 7820 696e 7374 616c 6c20  : "pipx install 
-00000120: 6e6f 7820 2626 2070 6970 7820 696e 7374  nox && pipx inst
-00000130: 616c 6c20 7072 652d 636f 6d6d 6974 2026  all pre-commit &
-00000140: 2620 6275 6e64 6c65 2069 6e73 7461 6c6c  & bundle install
-00000150: 222c 0a20 2022 6375 7374 6f6d 697a 6174  ",.  "customizat
-00000160: 696f 6e73 223a 207b 0a20 2020 2022 7673  ions": {.    "vs
-00000170: 636f 6465 223a 207b 0a20 2020 2020 2022  code": {.      "
-00000180: 6578 7465 6e73 696f 6e73 223a 205b 0a20  extensions": [. 
-00000190: 2020 2020 2020 2022 6d73 2d70 7974 686f         "ms-pytho
-000001a0: 6e2e 7079 7468 6f6e 222c 0a20 2020 2020  n.python",.     
-000001b0: 2020 2022 646f 6e6a 6179 616d 616e 6e65     "donjayamanne
-000001c0: 2e70 7974 686f 6e2d 656e 7669 726f 6e6d  .python-environm
-000001d0: 656e 742d 6d61 6e61 6765 7222 2c0a 2020  ent-manager",.  
-000001e0: 2020 2020 2020 2263 6861 726c 6965 726d        "charlierm
-000001f0: 6172 7368 2e72 7566 6622 0a20 2020 2020  arsh.ruff".     
-00000200: 205d 0a20 2020 207d 0a20 207d 0a7d 0a     ].    }.  }.}.
+00000000: 2f2f 2046 6f72 2066 6f72 6d61 7420 6465  // For format de
+00000010: 7461 696c 732c 2073 6565 2068 7474 7073  tails, see https
+00000020: 3a2f 2f61 6b61 2e6d 732f 6465 7663 6f6e  ://aka.ms/devcon
+00000030: 7461 696e 6572 2e6a 736f 6e2e 2046 6f72  tainer.json. For
+00000040: 2063 6f6e 6669 6720 6f70 7469 6f6e 732c   config options,
+00000050: 2073 6565 2074 6865 0a2f 2f20 5245 4144   see the.// READ
+00000060: 4d45 2061 743a 2068 7474 7073 3a2f 2f67  ME at: https://g
+00000070: 6974 6875 622e 636f 6d2f 6465 7663 6f6e  ithub.com/devcon
+00000080: 7461 696e 6572 732f 7465 6d70 6c61 7465  tainers/template
+00000090: 732f 7472 6565 2f6d 6169 6e2f 7372 632f  s/tree/main/src/
+000000a0: 756e 6976 6572 7361 6c0a 7b0a 2020 226e  universal.{.  "n
+000000b0: 616d 6522 3a20 2273 6369 656e 7469 6669  ame": "scientifi
+000000c0: 632d 7079 7468 6f6e 2d63 6f6f 6b69 655b  c-python-cookie[
+000000d0: 6465 765d 222c 0a20 2022 696d 6167 6522  dev]",.  "image"
+000000e0: 3a20 226d 6372 2e6d 6963 726f 736f 6674  : "mcr.microsoft
+000000f0: 2e63 6f6d 2f64 6576 636f 6e74 6169 6e65  .com/devcontaine
+00000100: 7273 2f70 7974 686f 6e3a 302d 332e 3131  rs/python:0-3.11
+00000110: 222c 0a20 2022 6665 6174 7572 6573 223a  ",.  "features":
+00000120: 207b 0a20 2020 2022 6768 6372 2e69 6f2f   {.    "ghcr.io/
+00000130: 6465 7663 6f6e 7461 696e 6572 732f 6665  devcontainers/fe
+00000140: 6174 7572 6573 2f72 7573 743a 3122 3a20  atures/rust:1": 
+00000150: 7b7d 2c0a 2020 2020 2267 6863 722e 696f  {},.    "ghcr.io
+00000160: 2f64 6576 636f 6e74 6169 6e65 7273 2f66  /devcontainers/f
+00000170: 6561 7475 7265 732f 7275 6279 3a31 223a  eatures/ruby:1":
+00000180: 207b 0a20 2020 2020 2022 7665 7273 696f   {.      "versio
+00000190: 6e22 3a20 2233 2e31 220a 2020 2020 7d0a  n": "3.1".    }.
+000001a0: 2020 7d2c 0a20 2022 706f 7374 4372 6561    },.  "postCrea
+000001b0: 7465 436f 6d6d 616e 6422 3a20 2270 6970  teCommand": "pip
+000001c0: 7820 696e 7374 616c 6c20 6e6f 7820 2626  x install nox &&
+000001d0: 2062 756e 646c 6520 696e 7374 616c 6c22   bundle install"
+000001e0: 2c0a 2020 2263 7573 746f 6d69 7a61 7469  ,.  "customizati
+000001f0: 6f6e 7322 3a20 7b0a 2020 2020 2276 7363  ons": {.    "vsc
+00000200: 6f64 6522 3a20 7b0a 2020 2020 2020 2265  ode": {.      "e
+00000210: 7874 656e 7369 6f6e 7322 3a20 5b0a 2020  xtensions": [.  
+00000220: 2020 2020 2020 226d 732d 7079 7468 6f6e        "ms-python
+00000230: 2e70 7974 686f 6e22 2c0a 2020 2020 2020  .python",.      
+00000240: 2020 2264 6f6e 6a61 7961 6d61 6e6e 652e    "donjayamanne.
+00000250: 7079 7468 6f6e 2d65 6e76 6972 6f6e 6d65  python-environme
+00000260: 6e74 2d6d 616e 6167 6572 220a 2020 2020  nt-manager".    
+00000270: 2020 5d0a 2020 2020 7d0a 2020 7d0a 7d0a    ].    }.  }.}.
```

### Comparing `sp_repo_review-2023.7.13/.github/workflows/bump.yml` & `sp_repo_review-2023.7.6/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/.github/workflows/cd.yml` & `sp_repo_review-2023.7.6/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/.github/workflows/ci.yml` & `sp_repo_review-2023.7.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/.github/workflows/reusable-change-detection.yml` & `sp_repo_review-2023.7.6/.github/workflows/reusable-change-detection.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/.github/workflows/reusable-cookie.yml` & `sp_repo_review-2023.7.6/.github/workflows/reusable-cookie.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/.github/workflows/reusable-rr-tests.yml` & `sp_repo_review-2023.7.6/.github/workflows/reusable-rr-tests.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/README.md` & `sp_repo_review-2023.7.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/_includes/head.html` & `sp_repo_review-2023.7.6/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/_includes/head_custom.html` & `sp_repo_review-2023.7.6/docs/_includes/head_custom.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/_includes/pyproject.md` & `sp_repo_review-2023.7.6/docs/_includes/pyproject.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/_plugins/repo_review.rb` & `sp_repo_review-2023.7.6/docs/_plugins/repo_review.rb`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/_plugins/tabs.rb` & `sp_repo_review-2023.7.6/docs/_plugins/tabs.rb`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/_sass/custom/custom.scss` & `sp_repo_review-2023.7.6/docs/_sass/custom/custom.scss`

 * *Files 5% similar despite different names*

```diff
@@ -80,17 +80,15 @@
   line-height: 1.2;
 }
 
 details {
   padding: 4px;
   margin-bottom: 1.5rem;
   border-radius: 4px;
-  box-shadow:
-    0 2px 3px rgba(0, 0, 0, 0.12),
-    0 3px 10px rgba(0, 0, 0, 0.08);
+  box-shadow: 0 2px 3px rgba(0, 0, 0, 0.12), 0 3px 10px rgba(0, 0, 0, 0.08);
   @media (prefers-color-scheme: dark) {
     box-shadow: 0 0 4px rgba(255, 255, 255, 0.4);
     background-color: black;
   }
 }
 
 details:not([open]) > summary::after {
@@ -115,17 +113,15 @@
   margin-block-end: 0;
   margin-inline-start: 0;
   margin-inline-end: 0;
 
   padding: 4px 1em;
   margin-bottom: 1.5rem;
   border-radius: 4px;
-  box-shadow:
-    0 2px 3px rgba(0, 0, 0, 0.12),
-    0 3px 10px rgba(0, 0, 0, 0.08);
+  box-shadow: 0 2px 3px rgba(0, 0, 0, 0.12), 0 3px 10px rgba(0, 0, 0, 0.08);
   @media (prefers-color-scheme: dark) {
     box-shadow: 0 0 4px rgba(255, 255, 255, 0.4);
     background-color: black;
   }
 }
 
 blockquote > h2 {
```

### Comparing `sp_repo_review-2023.7.13/docs/assets/favicon.ico` & `sp_repo_review-2023.7.6/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/assets/images/logo.svg` & `sp_repo_review-2023.7.6/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/assets/js/tabs.js` & `sp_repo_review-2023.7.6/docs/assets/js/tabs.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/assets/js/webapp.js` & `sp_repo_review-2023.7.6/docs/assets/js/webapp.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -210,15 +210,15 @@
             MaterialUI.ListSubheader > {
                 props.families[key]
             } <
             /MaterialUI.ListSubheader> {
                 results_components
             } <
             /ul> <
-            /li>,
+            /li>
         );
     }
 
     return ( <
         MaterialUI.Box sx = {
             {
                 bgcolor: "background.paper"
@@ -246,25 +246,25 @@
         await micropip.install([${deps_str}])
     `);
     return pyodide;
 }
 
 function MyThemeProvider(props) {
     const prefersDarkMode = MaterialUI.useMediaQuery(
-        "(prefers-color-scheme: dark)",
+        "(prefers-color-scheme: dark)"
     );
 
     const theme = React.useMemo(
         () =>
         MaterialUI.createTheme({
             palette: {
                 mode: prefersDarkMode ? "dark" : "light",
             },
         }),
-        [prefersDarkMode],
+        [prefersDarkMode]
     );
 
     return ( <
         MaterialUI.ThemeProvider theme = {
             theme
         } > {
             props.children
@@ -293,15 +293,15 @@
         if (!this.state.repo || !this.state.branch) {
             this.setState({
                 results: [],
                 msg: DEFAULT_MSG
             });
             window.history.replaceState(null, "", baseurl);
             alert(
-                `Please enter a repo (${this.state.repo}) and branch (${this.state.branch})`,
+                `Please enter a repo (${this.state.repo}) and branch (${this.state.branch})`
             );
             return;
         }
         const local_params = new URLSearchParams({
             repo: this.state.repo,
             branch: this.state.branch,
         });
```

### Comparing `sp_repo_review-2023.7.13/docs/pages/index.md` & `sp_repo_review-2023.7.6/docs/pages/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 code accidentally breaking other parts of your code? Do you want to more
 maintainable, reusable, and shareable form? Start at the
 [tutorial]({% link pages/tutorials/index.md %}).
 
 **Learn recommended tools and best practices.** [Topical guides]({% link
 pages/guides/index.md %}) provide task-based instruction on topics that scientists
 and research software engineers may encounter as their projects evolve and grow.
-This covers modern packaging([simple][] or [compiled][]), [style checking][], [testing][],
-[documentation][], [static typing][], [CI][], and much more!
+This covers [modern packaging][], [style checking][], [testing][], [documentation][],
+[static typing][], [CI][], and much more!
 
 {: .highlight-title }
 
 > New project template
 >
 > This guide comes with a [copier][]/[cookiecutter][]/[cruft][] template for
 > making new repos, [scientific-python/cookie][]. Twelve build backends
@@ -55,36 +55,21 @@
 libraries; it focuses on making or maintaining a package. We recommend the
 [SciPy Lecture Notes](https://scipy-lectures.org/) if you want info.
 
 This guide also does not cover version control, but it is essential to have a
 basic facility with git to use these tools successfully. We recommend the
 [Software Carpentry lesson on git](https://swcarpentry.github.io/git-novice/).
 
-{: .note-title }
-
-> History
->
-> This guide (along with cookie & repo-review) started in [Scikit-HEP][]
-> in 2020. It was merged with the [NSLS-II][] guidelines and moved to Scientific
-> Python at the [2023 Scientific Python Developer Summit][2023 spdev], along
-> with many updates. Improved support for compiled components supported in part
-> by NSF cooperative agreement [OAC-2209877][].
-
 <!-- prettier-ignore-start -->
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
-[simple]:                   {% link pages/guides/packaging_simple.md %}
-[compiled]:                 {% link pages/guides/packaging_compiled.md %}
+[modern packaging]:         {% link pages/guides/packaging_simple.md %}
 [style checking]:           {% link pages/guides/style.md %}
 [testing]:                  {% link pages/guides/pytest.md %}
 [documentation]:            {% link pages/guides/docs.md %}
 [static typing]:            {% link pages/guides/mypy.md %}
 [ci]:                       {% link pages/guides/gha_pure.md %}
 [sp-repo-review]:           {% link pages/guides/repo_review.md %}
 [repo-review]:              https://repo-review.readthedocs.io
 [copier]:                   https://copier.readthedocs.io
 [cookiecutter]:             https://cookiecutter.readthedocs.io
 [cruft]:                    https://cruft.github.io/cruft
-[2023 spdev]:               https://scientific-python.org/summits/developer/2023
-[scikit-hep]:               https://scikit-hep.org
-[OAC-2209877]:              https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209877&HistoricalAwards=false
-[nsls-ii]:                  https://nsls-ii.github.io
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/coverage.md` & `sp_repo_review-2023.7.6/docs/pages/guides/coverage.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/docs.md` & `sp_repo_review-2023.7.6/docs/pages/guides/docs.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/gha_basic.md` & `sp_repo_review-2023.7.6/docs/pages/guides/gha_basic.md`

 * *Files 2% similar despite different names*

```diff
@@ -201,17 +201,16 @@
 
 You can write GitHub flavored markdown to `$GITHUB_STEP_SUMMARY`, and it will be
 shown on the summary page.
 
 You can output annotations, as well; these show up inline on the code in the PR.
 This can be done by
 [setting special double-colon outputs](https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#setting-an-error-message),
-like `echo "::error file=app.js,line=1::Missing semicolon"`. See
-[pytest-github-actions-annotate-failures](https://github.com/pytest-dev/pytest-github-actions-annotate-failures)
-for a plugin to do this with pytest.
+like `echo "::error file=app.js,line=1::Missing semicolon"`. See []() for a
+plugin to do this with pytest.
 
 You can also do this
 [by supplying matchers](https://github.com/actions/toolkit/blob/main/docs/problem-matchers.md),
 which tell GitHub to look for certain patterns, such as
 `echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"`. Do keep
 in mind you can only see up to 10 matches per type per step, and a total of 50
 matchers.
@@ -271,15 +270,15 @@
 - [re-actors/alls-green](https://github.com/re-actors/alls-green): Tooling to
   check to see if all jobs passed (supports allowed failures, too).
 
 There are also a few useful tools installed which can really simplify your
 workflow or adding custom actions. This includes system package managers (like
 brew, chocolaty, NuGet, Vcpkg, etc), as well as a fantastic cross platform one:
 
-- [pipx](https://github.com/pypa/pipx): This is pre-installed on all runners
+- [pipx](https://github.com/pypy/pipx): This is pre-installed on all runners
   (GitHub uses to set up other things), and is kept up to date. It enables you
   to use any PyPI application in a single line with `pipx run <app>`.
 
 You can also run GitHub Actions locally:
 
 - [act](https://github.com/nektos/act): Run GitHub Actions in a docker image
   locally.
@@ -650,15 +649,15 @@
 `base_url`, or `host` - see the action
 [config](https://github.com/actions/configure-pages/blob/main/action.yml)).
 
 {% endraw %}
 
 ```yaml
 - name: Upload artifact
-  uses: actions/upload-pages-artifact@v2
+  uses: actions/upload-pages-artifact@v1
 ```
 
 This actions defaults to uploading `_site`, but you can give any `with: path:`
 if you want, including `"."` which is the whole repository.
 
 Finally, you'll need to deploy the artifact (named `github-pages`) to Pages. You
 can make this a custom job with `needs:` pointing at your previous job (in this
```

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/gha_pure.md` & `sp_repo_review-2023.7.6/docs/pages/guides/gha_pure.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/gha_wheels.md` & `sp_repo_review-2023.7.6/docs/pages/guides/gha_wheels.md`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
   steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.14.0
+    - uses: pypa/cibuildwheel@v2.13.1
 
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
 ```
```

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/index.md` & `sp_repo_review-2023.7.6/docs/pages/guides/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/mypy.md` & `sp_repo_review-2023.7.6/docs/pages/guides/mypy.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/packaging_classic.md` & `sp_repo_review-2023.7.6/docs/pages/guides/packaging_classic.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/packaging_compiled.md` & `sp_repo_review-2023.7.6/docs/pages/guides/packaging_compiled.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/packaging_simple.md` & `sp_repo_review-2023.7.6/docs/pages/guides/packaging_simple.md`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
 - [Hatchling info here](https://hatch.pypa.io/latest/config/build/#file-selection).
   Hatchling uses your VCS ignore file by default, so make sure it is accurate
   (which is a good idea anyway).
 - [Flit info here](https://flit.readthedocs.io/en/latest/pyproject_toml.html#sdist-section).
   Flit requires manual inclusion/exclusion in many cases, like using a dirty
   working directory.
-- [PDM info here](https://pdm-backend.fming.dev/build_config/#include-or-exclude-files).
+- [PDM info here](https://pdm.fming.dev/pyproject/tool-pdm/#include-and-exclude-package-files).
 - Setuptools still uses `MANIFEST.in`.
 
 {: .warning }
 
 > Flit will not use VCS (like git) to populate the SDist if you use standard
 > tooling, even if it can do that using its own tooling. So make sure you list
 > explicit include/exclude rules, and test the contents:
```

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/pytest.md` & `sp_repo_review-2023.7.6/docs/pages/guides/pytest.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/repo_review.md` & `sp_repo_review-2023.7.6/docs/pages/guides/repo_review.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/style.md` & `sp_repo_review-2023.7.6/docs/pages/guides/style.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 normalization, and to change the line length, and those go in your
 `pyproject.toml` file.
 
 Here is the snippet to add Black to your `.pre-commit-config.yml`:
 
 ```yaml
 - repo: https://github.com/psf/black
-  rev: "23.7.0"
+  rev: "23.3.0"
   hooks:
     - id: black
 ```
 
 {% details You can add a Black badge to your repo as well %}
 
 ```md
@@ -137,18 +137,18 @@
 {% rr PC111 %} If you want Black used in your documentation, you can use
 blacken-docs. This can even catch syntax errors in code snippets! It supports
 markdown and restructured text. Note that because black is in
 `additional_dependencies`, you'll have to keep it up to date manually.
 
 ```yaml
 - repo: https://github.com/asottile/blacken-docs
-  rev: "1.15.0"
+  rev: "1.14.0"
   hooks:
     - id: blacken-docs
-      additional_dependencies: [black==23.7.0]
+      additional_dependencies: [black==23.3.0]
 ```
 
 {% enddetails %}
 
 ## Ruff
 
 {% rr PC190 %} [Ruff][] [(docs)][ruff docs] is a Python code linter and
@@ -158,15 +158,15 @@
 pre-commit hook.
 
 [ruff docs]: https://beta.ruff.rs
 [ruff]: https://github.com/astral-sh/ruff
 
 ```yaml
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: "v0.0.277"
+  rev: "v0.0.276"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 ```
 
 {% rr PC191 %} The `--fix` argument is optional, but recommended, since you can
 inspect and undo changes in git.
@@ -431,21 +431,21 @@
 style syntax. Most useful to keep Python 2 outdated constructs out, it can even
 do some code updates for different versions of Python 3, like adding f-strings
 when clearly better (please always use them, they are faster) if you set
 `--py36-plus` (for example). This is a recommended addition for any project.
 
 ```yaml
 - repo: https://github.com/asottile/pyupgrade
-  rev: "v3.9.0"
+  rev: "v3.8.0"
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 ```
 
-[pyupgrade]: https://github.com/asottile/pyupgrade
+[pyupgrade]: https://github.com/asottile/pyupgrade:
 
 {: .note }
 
 > If you set this to at least `--py37-plus`, you can add the annotations import
 > by adding the following line to your isort pre-commit hook configuration:
 >
 > ```yaml
@@ -710,15 +710,15 @@
 ## Prettier
 
 {% rr PC180 %} The [prettier](https://prettier.io) tool can format a large
 number of different file types. An example of usage:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-prettier
-  rev: "v3.0.0"
+  rev: "v2.7.1"
   hooks:
     - id: prettier
       types_or: [yaml, markdown, html, css, scss, javascript, json]
 ```
 
 Since this formats a variety of very common file types (like `.html`, `.md`,
 `.yaml`, `.js`, and `.json`), you will usually want to provide a `types_or`
```

### Comparing `sp_repo_review-2023.7.13/docs/pages/guides/tasks.md` & `sp_repo_review-2023.7.6/docs/pages/guides/tasks.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/patterns/backports.md` & `sp_repo_review-2023.7.6/docs/pages/patterns/backports.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/patterns/data_files.md` & `sp_repo_review-2023.7.6/docs/pages/patterns/data_files.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/patterns/exports.md` & `sp_repo_review-2023.7.6/docs/pages/patterns/exports.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/patterns/index.md` & `sp_repo_review-2023.7.6/docs/pages/patterns/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/principles/design.md` & `sp_repo_review-2023.7.6/docs/pages/principles/design.md`

 * *Files 1% similar despite different names*

```diff
@@ -265,10 +265,10 @@
 exercising some restraint and consistency with the scientific Python ecosystem,
 Python can be used to build scientific tools that last and grow well over time.
 
 <!-- prettier-ignore-start -->
 
 [the UNIX philosophy]: https://en.wikipedia.org/wiki/Unix_philosophy
 [Duck typing]: https://en.wikipedia.org/wiki/Duck_typing
-["Stop Writing Classes"]: https://youtube.com/watch?v=o9pEzgHorH0&t=193s
+["Stop Writing Classes"]: https:k//www.youtube.com/watch?v=o9pEzgHorH0&t=193s
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.7.13/docs/pages/principles/index.md` & `sp_repo_review-2023.7.6/docs/pages/principles/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/principles/process.md` & `sp_repo_review-2023.7.6/docs/pages/principles/process.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/tutorials/dev-environment.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/dev-environment.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/tutorials/docs.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/docs.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/tutorials/index.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/tutorials/module.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/module.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/tutorials/packaging.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/packaging.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/docs/pages/tutorials/test.md` & `sp_repo_review-2023.7.6/docs/pages/tutorials/test.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/helpers/cog_helpers.py` & `sp_repo_review-2023.7.6/helpers/cog_helpers.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/helpers/extensions.py` & `sp_repo_review-2023.7.6/helpers/extensions.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/families.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/families.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/checks/general.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/general.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/checks/github.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/github.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/checks/mypy.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/checks/precommit.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/precommit.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/checks/pyproject.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/pyproject.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/checks/readthedocs.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/readthedocs.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/src/sp_repo_review/checks/ruff.py` & `sp_repo_review-2023.7.6/src/sp_repo_review/checks/ruff.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,17 +83,17 @@
 class RF1xx(Ruff):
     family = "ruff"
     requires = {"RF001"}
 
     @classmethod
     def check(cls: type[RuffMixin], pyproject: dict[str, Any]) -> bool:
         """
-        Must select the {self.name} `{self.code}` checks. Recommended:
+        Must select the {cls.name} `{cls.code}` checks. Recommended:
         ```toml
-        select = ["{self.code}"]  # {self.name}
+        select = ["{cls.code}"]  # {cls.name}
         ```
         """
 
         match pyproject:
             case {"tool": {"ruff": {"select": list(x)}}} | {
                 "tool": {"ruff": {"extend-select": list(x)}}
             }:
```

### Comparing `sp_repo_review-2023.7.13/tests/test_package.py` & `sp_repo_review-2023.7.6/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.gitignore` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: "23.7.0"
+    rev: "23.3.0"
     hooks:
       - id: black-jupyter
 
-  - repo: https://github.com/asottile/blacken-docs
-    rev: "1.15.0"
-    hooks:
-      - id: blacken-docs
-        additional_dependencies: [black==23.7.0]
-
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
@@ -34,22 +28,28 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0"
+    rev: "v2.7.1"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
+  - repo: https://github.com/asottile/blacken-docs
+    rev: "1.14.0"
+    hooks:
+      - id: blacken-docs
+        additional_dependencies: [black==23.3.0]
+
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.277"
+    rev: "v0.0.276"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
 {%- if cookiecutter.backend == "setuptools" or cookiecutter.backend == "pybind11" %}
 
   - repo: https://github.com/asottile/setup-cfg-fmt
```

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/README.md` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/noxfile.py` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/noxfile.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/pyproject.toml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.__ci=='gitlab' %}.gitlab-ci.yml{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.__ci == 'gitlab' %}.gitlab-ci.yml{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.license=='Apache' %}LICENSE{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'Apache' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.license=='BSD' %}LICENSE{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'BSD' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/{% if cookiecutter.license=='MIT' %}LICENSE{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/{% if cookiecutter.license == 'MIT' %}LICENSE{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/{% if cookiecutter.__ci == 'gitlab' %}pre-commit-update.sh{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/matchers/pylint.json` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/workflows/ci.yml` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,70 @@
-name: CI
+name: wheels
 
 on:
   workflow_dispatch:
-  pull_request:
-  push:
-    branches:
-      - master
-      - main
-      - develop
+  release:
+    types:
+      - published
 
 concurrency:
   group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: 3
 
 jobs:
-  pre-commit:
-    name: Format
+  make_sdist:
+    name: Make SDist
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-      - uses: pre-commit/action@v3.0.0
+
+      - name: Build SDist
+        run: pipx run build --sdist
+
+      - uses: actions/upload-artifact@v3
         with:
-          extra_args: --hook-stage manual --all-files
-      - name: Run PyLint
-        run: |
-          echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
-          pipx run nox -s pylint
-
-  checks:
-    name: {% raw %}Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}{% endraw %}
-    runs-on: {% raw %}${{ matrix.runs-on }}{% endraw %}
-    needs: [pre-commit]
+          path: dist/*.tar.gz
+
+  build_wheels:
+    name: {% raw %}Wheel on ${{ matrix.os }}{% endraw %}
+    runs-on: {% raw %}${{ matrix.os }}{% endraw %}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.11", "3.12"]
-        runs-on: [ubuntu-latest, macos-latest, windows-latest]
-
-        include:
-          - python-version: pypy-3.9
-            runs-on: ubuntu-latest
+        os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - uses: actions/setup-python@v4
-        with:
-          python-version: {% raw %}${{ matrix.python-version }}{% endraw %}
-          allow-prereleases: true
-
-      {%- if cookiecutter.backend == "mesonpy" %}
+      - uses: pypa/cibuildwheel@v2.13.1
 
-      - name: Activate MSVC for Meson
-        if: runner.os == 'Windows'
-        uses: ilammy/msvc-dev-cmd@v1
-
-      {%- endif %}
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          path: wheelhouse/*.whl
 
-      - name: Install package
-        run: python -m pip install .[test]
+  upload_all:
+    needs: [build_wheels, make_sdist]
+    environment: pypi
+    permissions:
+      id-token: write
+    runs-on: ubuntu-latest
+    if: github.event_name == 'release' && github.event.action == 'published'
 
-      - name: Test package
-        run: >-
-          python -m pytest -ra --cov --cov-report=xml --cov-report=term
-          --durations=20
+    steps:
+      - uses: actions/download-artifact@v3
+        with:
+          name: artifact
+          path: dist
 
-      - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.4
+      - uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          # Remember to tell (test-)pypi about this repo before publishing
+          # Remove this line to publish to PyPI
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type=='compiled' %}cd.yml{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,137 @@
-name: wheels
+{%- set compiled = cookiecutter.backend in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
+name: CI
 
 on:
   workflow_dispatch:
+  pull_request:
+  push:
+    branches:
+      - master
+      - main
+      - develop
+  {%- if not compiled %}
   release:
     types:
       - published
+  {%- endif %}
 
 concurrency:
   group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: 3
 
 jobs:
-  make_sdist:
-    name: Make SDist
+  pre-commit:
+    name: Format
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-
-      - name: Build SDist
-        run: pipx run build --sdist
-
-      - uses: actions/upload-artifact@v3
+      - uses: actions/setup-python@v4
         with:
-          path: dist/*.tar.gz
-
-  build_wheels:
-    name: {% raw %}Wheel on ${{ matrix.os }}{% endraw %}
-    runs-on: {% raw %}${{ matrix.os }}{% endraw %}
+          python-version: "3.x"
+      - uses: pre-commit/action@v3.0.0
+        with:
+          extra_args: --hook-stage manual --all-files
+      - name: Run PyLint
+        run: |
+          echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
+          pipx run nox -s pylint
+
+  checks:
+    name: {% raw %}Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}{% endraw %}
+    runs-on: {% raw %}${{ matrix.runs-on }}{% endraw %}
+    needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ["3.8", "3.11", "3.12"]
+        runs-on: [ubuntu-latest, macos-latest, windows-latest]
+
+        include:
+          - python-version: pypy-3.9
+            runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: {% raw %}${{ matrix.python-version }}{% endraw %}
+          allow-prereleases: true
+
+      {%- if cookiecutter.backend == "mesonpy" %}
+      - name: Activate MSVC for Meson
+        if: runner.os == 'Windows'
+        uses: ilammy/msvc-dev-cmd@v1
+      {%- endif %}
+
+      - name: Install package
+        run: python -m pip install .[test]
+
+      - name: Test package
+        run: >-
+          python -m pytest -ra --cov --cov-report=xml --cov-report=term
+          --durations=20
+
+      - name: Upload coverage report
+        uses: codecov/codecov-action@v3.1.4
+
+  {%- if not compiled %}
+
+  dist:
+    needs: [pre-commit]
+    name: Distribution build
+    runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - uses: pypa/cibuildwheel@v2.14.0
+      - name: Build sdist and wheel
+        run: pipx run build
 
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v3
         with:
-          path: wheelhouse/*.whl
+          path: dist
+
+      {%- if cookiecutter.backend != "trampolim" %}
 
-  upload_all:
-    needs: [build_wheels, make_sdist]
+      - name: Check products
+        run: pipx run twine check dist/*
+
+      {%- endif %}
+
+  publish:
+    needs: [dist]
+    name: Publish to PyPI
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
+        if: github.event_name == 'release' && github.event.action == 'published'
         with:
           # Remember to tell (test-)pypi about this repo before publishing
           # Remove this line to publish to PyPI
           repository-url: https://test.pypi.org/legacy/
+          {%- if cookiecutter.backend == "trampolim" %}
+          # Check not supported currently by twine + trampolim
+          verify-metadata: false
+          {%- endif %}
+
+  {%- endif %}
```

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/docs/conf.py` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py` & `sp_repo_review-2023.7.6/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/.gitignore` & `sp_repo_review-2023.7.6/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -148,10 +148,7 @@
 # NodeJS stuff, just in case (developer tooling)
 node_modules/
 package-lock.json
 package.json
 
 # readthedocs
 _readthedocs
-
-# Default cookiecutter output
-/package
```

### Comparing `sp_repo_review-2023.7.13/LICENSE` & `sp_repo_review-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/pyproject.toml` & `sp_repo_review-2023.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.7.13/PKG-INFO` & `sp_repo_review-2023.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sp_repo_review
-Version: 2023.7.13
+Version: 2023.7.6
 Summary: Review repos for compliance to the Scientific-Python development guidelines
 Project-URL: Guide, https://learn.scientific-python.org/development
 Project-URL: Homepage, https://scientific-python.github.io/cookie
 Project-URL: Preview, https://scientific-python-cookie.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/cookie
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
```

