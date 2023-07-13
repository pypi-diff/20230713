# Comparing `tmp/tskit_book_theme-0.3.2.tar.gz` & `tmp/tskit_book_theme-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tskit_book_theme-0.3.2.tar", last modified: Wed Sep  7 22:12:50 2022, max compression
+gzip compressed data, was "tskit_book_theme-1.0.1.tar", last modified: Thu Jul 13 12:21:37 2023, max compression
```

## Comparing `tskit_book_theme-0.3.2.tar` & `tskit_book_theme-1.0.1.tar`

### file list

```diff
@@ -1,226 +1,239 @@
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-09-07 22:12:50.447928 tskit_book_theme-0.3.2/
--rw-rw-r--   0 benj      (1000) benj      (1000)     5446 2022-06-23 11:32:22.235980 tskit_book_theme-0.3.2/ARCHITECTURE.md
--rw-rw-r--   0 benj      (1000) benj      (1000)    19800 2022-06-23 11:27:26.932963 tskit_book_theme-0.3.2/CHANGELOG.md
--rw-rw-r--   0 benj      (1000) benj      (1000)       68 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/CONTRIBUTING.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     1522 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/LICENSE
--rw-rw-r--   0 benj      (1000) benj      (1000)     1989 2022-06-23 11:33:19.604877 tskit_book_theme-0.3.2/README.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      178 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/codecov.yml
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:45:56.465471 tskit_book_theme-0.3.2/docs/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_static/
--rw-rw-r--   0 benj      (1000) benj      (1000)       41 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_static/custom.css
--rw-rw-r--   0 benj      (1000) benj      (1000)     2143 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_static/logo-square.svg
--rw-rw-r--   0 benj      (1000) benj      (1000)     9371 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_static/logo-wide.svg
--rw-rw-r--   0 benj      (1000) benj      (1000)      266 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_static/rtd-data.js
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_templates/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_templates/sections/
--rw-rw-r--   0 benj      (1000) benj      (1000)       78 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/_templates/sections/header.html
--rw-rw-r--   0 benj      (1000) benj      (1000)       33 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/changelog.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     6749 2022-06-23 11:32:44.108336 tskit_book_theme-0.3.2/docs/conf.py
--rw-rw-r--   0 benj      (1000) benj      (1000)     7938 2022-06-23 11:28:10.362302 tskit_book_theme-0.3.2/docs/content-blocks.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/contributing/
--rw-rw-r--   0 benj      (1000) benj      (1000)       39 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/contributing/architecture.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      589 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/contributing/index.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     4953 2022-06-23 11:32:48.564407 tskit_book_theme-0.3.2/docs/contributing/setup.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     2878 2022-06-23 11:32:52.100462 tskit_book_theme-0.3.2/docs/contributing/style.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     1657 2022-06-23 11:33:25.544963 tskit_book_theme-0.3.2/docs/contributing/subthemes.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     3493 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/contributing/tests.md
--rw-rw-r--   0 benj      (1000) benj      (1000)       74 2022-06-23 11:32:53.992492 tskit_book_theme-0.3.2/docs/contributing/translate.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/
--rw-rw-r--   0 benj      (1000) benj      (1000)      740 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/announcements.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      607 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/custom-css.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      303 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/download.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     1107 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/header.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     2449 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/index.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     3606 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/sidebar-primary.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     1092 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/sidebar-secondary.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      346 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/single-page.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     1854 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/customize/source-files.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/images/
--rw-rw-r--   0 benj      (1000) benj      (1000)     9269 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/images/cool.jpg
--rw-rw-r--   0 benj      (1000) benj      (1000)     2304 2022-06-23 11:28:54.399537 tskit_book_theme-0.3.2/docs/index.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     4037 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/launch.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     8116 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/notebooks.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/
--rw-rw-r--   0 benj      (1000) benj      (1000)      245 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/api-numpy.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/blog/
--rw-rw-r--   0 benj      (1000) benj      (1000)       70 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/blog/post1.md
--rw-rw-r--   0 benj      (1000) benj      (1000)       79 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/blog/post2.md
--rw-rw-r--   0 benj      (1000) benj      (1000)       99 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/blog.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      962 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/comments.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     2285 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/extensions.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/kitchen-sink/
--rw-rw-r--   0 benj      (1000) benj      (1000)      208 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/kitchen-sink/api.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)      239 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/kitchen-sink/index.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)    10125 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/kitchen-sink/lists-and-tables.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)    14178 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/kitchen-sink/paragraph-markup.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)     4685 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/notebooks.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     7257 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/special-theme-elements.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     1668 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/reference/thebe.md
--rw-rw-r--   0 benj      (1000) benj      (1000)     1597 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/references.bib
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/docs/tutorials/
--rw-rw-r--   0 benj      (1000) benj      (1000)     3944 2022-06-23 11:33:26.920983 tskit_book_theme-0.3.2/docs/tutorials/get-started.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      632 2022-06-23 11:33:18.452860 tskit_book_theme-0.3.2/package.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     1747 2022-06-23 11:32:30.896123 tskit_book_theme-0.3.2/pyproject.toml
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:34:42.989979 tskit_book_theme-0.3.2/src/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-07-12 13:45:49.868528 tskit_book_theme-0.3.2/src/tskit_book_theme/
--rw-rw-r--   0 benj      (1000) benj      (1000)     7492 2022-09-04 23:46:48.186208 tskit_book_theme-0.3.2/src/tskit_book_theme/__init__.py
--rw-rw-r--   0 benj      (1000) benj      (1000)     2523 2022-06-23 11:32:59.940583 tskit_book_theme-0.3.2/src/tskit_book_theme/_compile_translations.py
--rw-rw-r--   0 benj      (1000) benj      (1000)     3890 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/_transforms.py
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/scripts/
--rw-rw-r--   0 benj      (1000) benj      (1000)     6985 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/scripts/index.js
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 13:25:03.856263 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/abstracts/
--rw-rw-r--   0 benj      (1000) benj      (1000)     1233 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/abstracts/_mixins.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     2210 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/abstracts/_variables.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/base/
--rw-rw-r--   0 benj      (1000) benj      (1000)      984 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/base/_base.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      177 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/base/_bootstrap.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     1047 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/base/_print.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     1030 2022-06-23 12:32:23.385702 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/base/_typography.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/components/
--rw-rw-r--   0 benj      (1000) benj      (1000)     2218 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/components/_buttons.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      281 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/components/_search.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/
--rw-rw-r--   0 benj      (1000) benj      (1000)      428 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_admonitions.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      955 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_code.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      415 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_field-lists.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      292 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_footnotes.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)       51 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_glossary.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      824 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_images.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     2879 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_margin.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      846 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_math.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      372 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_quotes.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      375 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_sidebar.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     1275 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_tableofcontents.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/extensions/
--rw-rw-r--   0 benj      (1000) benj      (1000)      565 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/extensions/_ablog.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      825 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/extensions/_myst-nb.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     1419 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/extensions/_readthedocs.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      307 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/extensions/_sphinx-tabs.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      431 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/extensions/_thebe.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      308 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/extensions/comments.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     1529 2022-06-23 13:25:03.856263 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/index.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/pages/
--rw-rw-r--   0 benj      (1000) benj      (1000)      810 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/pages/_search.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/
--rw-rw-r--   0 benj      (1000) benj      (1000)      418 2022-06-23 12:23:27.027602 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_article.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      515 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_footer-article.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      169 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_footer-content.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      765 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_header-article.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)      407 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_headers.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     2616 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_sidebar-primary.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     2430 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_sidebar-secondary.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     1914 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_sidebars-toggle.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 12:32:10.497522 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/tskit/
--rw-rw-r--   0 benj      (1000) benj      (1000)      917 2022-06-23 13:31:44.227112 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/tskit/_palette.scss
--rw-rw-r--   0 benj      (1000) benj      (1000)     5364 2022-08-30 13:28:10.165391 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/tskit/_tskit.scss
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/
--rw-rw-r--   0 benj      (1000) benj      (1000)     3280 2022-06-23 11:33:27.968998 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/README.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/
--rw-rw-r--   0 benj      (1000) benj      (1000)     3018 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/By the.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     2986 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/By.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     2494 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Contents.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3443 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Copyright.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     4814 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Download notebook file.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     4389 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Download source file.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     4205 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Download this page.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     4096 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Edit this page.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3008 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Fullscreen mode.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     4133 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Last updated on.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3199 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Launch.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3717 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Open an issue.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3625 2022-06-23 11:26:17.382541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Print to PDF.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3320 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Search the docs.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     4402 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Search this book.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3638 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Source repository.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3954 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Sphinx Book Theme.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3282 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Theme by the.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     4111 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Toggle navigation.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3548 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/next page.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3561 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/open issue.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3595 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/previous page.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     2529 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/repository.json
--rw-rw-r--   0 benj      (1000) benj      (1000)     3697 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/suggest edit.json
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:45:56.553471 tskit_book_theme-0.3.2/src/tskit_book_theme/header_buttons/
--rw-rw-r--   0 benj      (1000) benj      (1000)     6147 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/header_buttons/__init__.py
--rw-rw-r--   0 benj      (1000) benj      (1000)     7573 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/header_buttons/launch.py
--rw-rw-r--   0 benj      (1000) benj      (1000)     1254 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/nodes.py
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:35:44.034654 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/components/
--rw-rw-r--   0 benj      (1000) benj      (1000)     1002 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/components/sbt-sidebar-nav.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      534 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/components/sidebar-logo.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      199 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/components/toc-button.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     3787 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/layout.html
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/macros/
--rw-rw-r--   0 benj      (1000) benj      (1000)     2399 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/macros/buttons.html
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/sections/
--rw-rw-r--   0 benj      (1000) benj      (1000)       27 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/sections/announcement.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      164 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/sections/footer-article.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      788 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/sections/footer-content.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     1163 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/sections/header-article.html
--rw-rw-r--   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/sections/header.html
--rw-rw-r--   0 benj      (1000) benj      (1000)       84 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/sections/sidebar.html
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:45:34.329451 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/
--rw-rw-r--   0 benj      (1000) benj      (1000)       23 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/.gitignore
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/
--rw-rw-r--   0 benj      (1000) benj      (1000)     1186 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_binder.svg
--rw-rw-r--   0 benj      (1000) benj      (1000)     7601 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_colab.png
--rw-rw-r--   0 benj      (1000) benj      (1000)      681 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_deepnote.svg
--rw-rw-r--   0 benj      (1000) benj      (1000)     1758 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_jupyterhub.svg
--rw-rw-r--   0 benj      (1000) benj      (1000)      417 2022-06-23 11:31:29.547043 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/sbt-webpack-macros.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      827 2022-07-15 12:51:28.572132 tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/theme.conf
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/
--rw-rw-r--   0 benj      (1000) benj      (1000)       43 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/conftest.py
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/
--rw-rw-r--   0 benj      (1000) benj      (1000)      634 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/Makefile
--rw-rw-r--   0 benj      (1000) benj      (1000)     1170 2022-06-23 11:33:14.096796 tskit_book_theme-0.3.2/tests/sites/base/conf.py
--rw-rw-r--   0 benj      (1000) benj      (1000)      138 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/index.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      143 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/page1.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      359 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/page2.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/section1/
--rw-rw-r--   0 benj      (1000) benj      (1000)       77 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/section1/index.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      778 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/section1/ntbk.ipynb
--rw-rw-r--   0 benj      (1000) benj      (1000)   146494 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/section1/ntbk_julia.ipynb
--rw-rw-r--   0 benj      (1000) benj      (1000)    41097 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/section1/ntbk_octave.ipynb
--rw-rw-r--   0 benj      (1000) benj      (1000)      275 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/section1/ntbkmd.md
--rw-rw-r--   0 benj      (1000) benj      (1000)       18 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/section1/page1.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/titles/
--rw-rw-r--   0 benj      (1000) benj      (1000)       59 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/titles/index.md
--rw-rw-r--   0 benj      (1000) benj      (1000)      120 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/titles/page-multipletitles.md
--rw-rw-r--   0 benj      (1000) benj      (1000)       96 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/titles/page-onetitle.md
--rw-rw-r--   0 benj      (1000) benj      (1000)       53 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/base/titles/page-onetitlenoheadings.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/notitle/
--rw-rw-r--   0 benj      (1000) benj      (1000)      329 2022-06-23 11:33:15.756821 tskit_book_theme-0.3.2/tests/sites/notitle/conf.py
--rw-rw-r--   0 benj      (1000) benj      (1000)       24 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/notitle/index.md
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/
--rw-rw-r--   0 benj      (1000) benj      (1000)      641 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/Makefile
--rw-rw-r--   0 benj      (1000) benj      (1000)       61 2022-06-23 11:33:16.796836 tskit_book_theme-0.3.2/tests/sites/parallel-build/conf.py
--rw-rw-r--   0 benj      (1000) benj      (1000)       22 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/five.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)       22 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/four.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)      302 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/index.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)       17 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/one.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)       23 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/three.rst
--rw-rw-r--   0 benj      (1000) benj      (1000)       17 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/sites/parallel-build/two.rst
-drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/
--rw-rw-r--   0 benj      (1000) benj      (1000)     4406 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/build__header-article.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     1050 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/build__pagetoc--page-multipletitles.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      581 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/build__pagetoc--page-onetitle.html
--rw-rw-r--   0 benj      (1000) benj      (1000)       50 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/build__pagetoc--page-onetitlenoheadings.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     2669 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/build__sidebar-primary__nav.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     1223 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/header__repo-buttons--all-off.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     2738 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/header__repo-buttons--all-on.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     2196 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/header__repo-buttons--custom-branch.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     1507 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/header__repo-buttons--one-on.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     2449 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/test_header_launchbtns.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      980 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/test_marginnote.html
--rw-rw-r--   0 benj      (1000) benj      (1000)       97 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/test_right_sidebar_title.html
--rw-rw-r--   0 benj      (1000) benj      (1000)      878 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/test_sidenote.html
--rw-rw-r--   0 benj      (1000) benj      (1000)     2449 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tests/test_build/test_topbar_launchbtns.html
--rw-rw-r--   0 benj      (1000) benj      (1000)    12843 2022-06-23 11:30:39.714047 tskit_book_theme-0.3.2/tests/test_build.py
--rw-rw-r--   0 benj      (1000) benj      (1000)      861 2022-06-23 11:33:12.704775 tskit_book_theme-0.3.2/tests/test_locale_convert.py
--rw-rw-r--   0 benj      (1000) benj      (1000)     1288 2022-06-23 11:26:17.386541 tskit_book_theme-0.3.2/tox.ini
--rw-rw-r--   0 benj      (1000) benj      (1000)     1650 2022-06-23 11:33:24.124943 tskit_book_theme-0.3.2/webpack.config.js
--rw-r--r--   0        0        0     5701 1970-01-01 00:00:00.000000 tskit_book_theme-0.3.2/PKG-INFO
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-13 12:21:37.364160 tskit_book_theme-1.0.1/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     5441 2023-07-11 13:11:00.380425 tskit_book_theme-1.0.1/ARCHITECTURE.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)    32144 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/CHANGELOG.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      114 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/CONTRIBUTING.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1522 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/LICENSE
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1944 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/README.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      178 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/codecov.yml
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-12 15:10:35.818435 tskit_book_theme-1.0.1/docs/
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       41 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/custom.css
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1507 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/ebp-logo.png
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2620 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/logo-square.png
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2143 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/logo-square.svg
+-rw-rw-r--   0 benj      (1000) benj      (1000)    10269 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/logo-wide-dark.svg
+-rw-rw-r--   0 benj      (1000) benj      (1000)     9371 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/logo-wide.svg
+-rw-rw-r--   0 benj      (1000) benj      (1000)      266 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_static/rtd-data.js
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_templates/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      201 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/_templates/test.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)       33 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/changelog.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/components/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      551 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/components/custom-css.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      682 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/components/download.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      297 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/components/icon-links.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      171 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/components/index.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      286 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/components/logo.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3354 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/components/source-files.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     8213 2023-07-12 15:10:35.810435 tskit_book_theme-1.0.1/docs/conf.py
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:22:10.306687 tskit_book_theme-1.0.1/docs/content/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     7951 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/content/content-blocks.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      169 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/content/index.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4047 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/content/launch.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     8117 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/content/notebooks.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/contributing/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       39 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/contributing/architecture.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      585 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/contributing/index.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4963 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/contributing/setup.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2881 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/contributing/style.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1659 2023-07-11 13:11:00.384425 tskit_book_theme-1.0.1/docs/contributing/subthemes.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3493 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/contributing/tests.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)       75 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/contributing/translate.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2400 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/contributing/versions.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/images/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     9269 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/images/cool.jpg
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2323 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/index.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      245 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/api-numpy.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/blog/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       70 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/blog/post1.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)       79 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/blog/post2.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)       99 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/blog.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      962 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/comments.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2162 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/extensions.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1608 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/admonitions.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)      980 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/api.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     8125 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/blocks.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     8597 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/generic.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3070 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/images.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)      909 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/index.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     6151 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/lists.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)    13453 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/really-long.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     6375 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/structure.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     5068 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/tables.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2668 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/kitchen-sink/typography.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4751 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/notebooks.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     7240 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/special-theme-elements.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1668 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference/thebe.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1987 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/reference.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1597 2023-07-11 13:11:00.388425 tskit_book_theme-1.0.1/docs/references.bib
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-12 15:11:02.742669 tskit_book_theme-1.0.1/docs/scripts/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1518 2023-07-12 15:11:02.734669 tskit_book_theme-1.0.1/docs/scripts/update_kitchen_sink.py
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      740 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/announcements.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      914 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/footer-content.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      912 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/footer.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1988 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/header.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      202 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/index.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2623 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/sidebar-primary.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1100 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/sections/sidebar-secondary.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/tutorials/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3946 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/docs/tutorials/get-started.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      633 2023-07-12 14:43:31.952482 tskit_book_theme-1.0.1/package.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1935 2023-07-12 14:39:35.134460 tskit_book_theme-1.0.1/pyproject.toml
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-12 16:03:01.410518 tskit_book_theme-1.0.1/src/
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-13 00:00:39.827615 tskit_book_theme-1.0.1/src/tskit_book_theme/
+-rw-rw-r--   0 benj      (1000) benj      (1000)    10398 2023-07-13 00:00:39.823615 tskit_book_theme-1.0.1/src/tskit_book_theme/__init__.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2524 2023-07-12 15:11:28.790896 tskit_book_theme-1.0.1/src/tskit_book_theme/_compile_translations.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4158 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/_transforms.py
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/scripts/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     5811 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/scripts/index.js
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:31:29.711933 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/abstracts/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      600 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/abstracts/_mixins.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1483 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/abstracts/_variables.scss
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/base/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      933 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/base/_base.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1880 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/base/_print.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      517 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/base/_typography.scss
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/components/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      455 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/components/_icon-links.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      461 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/components/_logo.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      707 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/components/_search.scss
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/content/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      128 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/content/_code.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      824 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/content/_images.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4767 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/content/_margin.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      250 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/content/_notebooks.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      364 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/content/_quotes.scss
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/extensions/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      308 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/extensions/_comments.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      431 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/extensions/_thebe.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1198 2023-07-11 13:31:16.931813 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/index.scss
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       94 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_announcement.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      580 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_article-container.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)       29 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_article.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      150 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_footer-article.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      436 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_footer-content.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4046 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_header-article.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)      233 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_header-primary.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1266 2023-07-11 13:11:00.392425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_sidebar-primary.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2568 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_sidebar-secondary.scss
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-12 23:51:24.989557 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/tskit/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      708 2023-07-11 13:37:04.135062 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/tskit/_palette.scss
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4971 2023-07-12 23:51:24.981557 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/tskit/_tskit.scss
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3288 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/README.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3033 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/By the.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2988 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/By.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2494 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Contents.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3446 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Copyright.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4808 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Download notebook file.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4389 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Download source file.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4205 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Download this page.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4090 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Edit this page.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3011 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Fullscreen mode.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4133 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Last updated on.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3198 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Launch.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3711 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Open an issue.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3627 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Print to PDF.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3659 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Source repository.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3948 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Sphinx Book Theme.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3300 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Theme by the.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4135 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Toggle navigation.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3548 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/next page.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3565 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/open issue.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3595 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/previous page.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2531 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/repository.json
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3790 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/suggest edit.json
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:22:11.210696 tskit_book_theme-1.0.1/src/tskit_book_theme/header_buttons/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     6715 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/header_buttons/__init__.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)     9008 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/header_buttons/launch.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)     5130 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/header_buttons/source.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1254 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/nodes.py
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-12 14:42:25.811936 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-12 23:42:06.396184 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      447 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/article-header-buttons.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)       97 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/author.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      103 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/extra-footer.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      640 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/page-toc.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1018 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/sbt-sidebar-nav.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      206 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/toggle-primary-sidebar.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      324 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/toggle-secondary-sidebar.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      965 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/layout.html
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/macros/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2299 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/macros/buttons.html
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/sections/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      328 2023-07-11 13:11:00.396425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/sections/footer-content.html
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-12 15:05:32.843799 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       23 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/.gitignore
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1186 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_binder.svg
+-rw-rw-r--   0 benj      (1000) benj      (1000)     7601 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_colab.png
+-rw-rw-r--   0 benj      (1000) benj      (1000)      681 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_deepnote.svg
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1758 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_jupyterhub.svg
+-rw-rw-r--   0 benj      (1000) benj      (1000)      417 2023-07-12 15:05:32.835799 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/sbt-webpack-macros.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1523 2023-07-12 23:42:06.324184 tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/theme.conf
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       43 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/conftest.py
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      634 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/Makefile
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1169 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/conf.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)      147 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/index.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      143 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/page1.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      371 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/page2.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/section1/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       77 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/section1/index.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      745 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/section1/ntbk.ipynb
+-rw-rw-r--   0 benj      (1000) benj      (1000)   146494 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/section1/ntbk_julia.ipynb
+-rw-rw-r--   0 benj      (1000) benj      (1000)    41097 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/section1/ntbk_octave.ipynb
+-rw-rw-r--   0 benj      (1000) benj      (1000)      275 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/section1/ntbkmd.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)       18 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/section1/page1.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/titles/
+-rw-rw-r--   0 benj      (1000) benj      (1000)       59 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/titles/index.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)      120 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/titles/page-multipletitles.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)       96 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/titles/page-onetitle.md
+-rw-rw-r--   0 benj      (1000) benj      (1000)       53 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/base/titles/page-onetitlenoheadings.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/notitle/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      330 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/notitle/conf.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)       24 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/notitle/index.md
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/
+-rw-rw-r--   0 benj      (1000) benj      (1000)      641 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/Makefile
+-rw-rw-r--   0 benj      (1000) benj      (1000)       62 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/conf.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)       22 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/five.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)       22 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/four.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)      302 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/index.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)       17 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/one.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)       23 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/three.rst
+-rw-rw-r--   0 benj      (1000) benj      (1000)       17 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/sites/parallel-build/two.rst
+drwxrwxr-x   0 benj      (1000) benj      (1000)        0 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/
+-rw-rw-r--   0 benj      (1000) benj      (1000)     5622 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/test_build/build__header-article.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1233 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/test_build/build__pagetoc--page-multipletitles.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      736 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/test_build/build__pagetoc--page-onetitle.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      685 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__launch-buttons--bitbucket.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1083 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__launch-buttons--github.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      515 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__launch-buttons--gitlab.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      595 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__launch-buttons--gitlab_manual.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2293 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__repo-buttons--all-off.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     4012 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__repo-buttons--all-on.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     3377 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__repo-buttons--custom-branch.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2625 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__repo-buttons--one-on.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      364 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__source-buttons--bitbucket.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      500 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__source-buttons--github.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      337 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__source-buttons--github_manual.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      455 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__source-buttons--gitlab.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      495 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/header__source-buttons--gitlab_manual.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)     2510 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/test_header_launchbtns.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      903 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/test_marginnote.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      111 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/test_right_sidebar_title.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)      931 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_build/test_sidenote.html
+-rw-rw-r--   0 benj      (1000) benj      (1000)    16746 2023-07-11 13:11:00.400425 tskit_book_theme-1.0.1/tests/test_build.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)      863 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tests/test_locale_convert.py
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1288 2023-07-11 13:11:00.404425 tskit_book_theme-1.0.1/tox.ini
+-rw-rw-r--   0 benj      (1000) benj      (1000)     1652 2023-07-12 15:11:57.763148 tskit_book_theme-1.0.1/webpack.config.js
+-rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 tskit_book_theme-1.0.1/PKG-INFO
```

### Comparing `tskit_book_theme-0.3.2/ARCHITECTURE.md` & `tskit_book_theme-1.0.1/ARCHITECTURE.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Architecture of the repository
 
 This is a short overview of the general architecture and structure of the repository, to help you orient yourself.
 
-This theme uses [sphinx-theme-builder](https://sphinx-theme-builder.readthedocs.io/en/latest/) as its build backend, and follows the [filesystem layout](https://sphinx-theme-builder.readthedocs.io/en/latest/reference/filesystem-layout/) recommended by it.
+This theme uses [sphinx-theme-builder](https://sphinx-theme-builder.readthedocs.io/en/latest/) as its build backend, and follows the [filesystem layout](https://sphinx-theme-builder.readthedocs.io/en/latest/filesystem-layout/) recommended by it.
 See below for some more specific sections
 
 ```{contents}
 ```
 
-## `src/tskit_book_theme/` - Theme source files
+## `src/sphinx_book_theme/` - Theme source files
 
 This folder contains all of the source files for this theme, and most changes to the theme are made somewhere inside this folder.
 
 `__init__.py`
 : The theme's Python module, which runs several configuration and set-up steps.
   This module does things like load in Sphinx's default HTML for the sidebar, and modify it in order to have dropdown nested lists.
   It also inserts several variables into the Jinja template context that are then used in our HTML templates.
@@ -21,15 +21,15 @@
 : Scripts to generate metadata for buttons in the header. We use [Jinja Macros](https://jinja.palletsprojects.com/en/3.0.x/templates/) (in the `macros/` folder) to generate the HTML for header buttons. The scripts in `header_buttons/` generate the data structure that is used to generate buttons with these macros (in the `header-article.html` template).
 
 `header_buttons/launch.py`
 : Logic to create the correct URLs for our launch buttons. This basically means building the URL for a given launch service in a proper fashion.
 
 The other folders in this section are described in the next few sections.
 
-### `/theme/tskit_book_theme/` - HTML templates
+### `/theme/sphinx_book_theme/` - HTML templates
 
 This is the actual theme source that is packaged and distributed via PyPI.
 It contains HTML templates that make up the theme structure.
 
 These follow the [`sphinx-basic-ng` template structure](https://sphinx-basic-ng.readthedocs.io/en/latest).
 
 - `layout.html` inherits from the [pydata sphinx theme](https://pydata-sphinx-theme.readthedocs.io/) and modifies several sections.
@@ -65,15 +65,15 @@
 - `docs/reference/`: Reference sections of the documentation, to demonstrate the look and feel of the theme.
   The "kitchen sink" is pulled directly [from the `sphinx-themes` website](https://github.com/sphinx-themes/sphinx-themes.org/tree/master/sample-docs/kitchen-sink).
   There are also other sections for theme-specific elements.
 
 
 ## `webpack.config.js` and `package.json` - Webpack and dependencies
 
-`webpack.config.js` contains the compilation code to convert source files like SCSS and JS in `src/tskit_book_theme/assets/*` into the production assets in `src/tskit_book_theme/theme/tskit_book_theme/static/` .
+`webpack.config.js` contains the compilation code to convert source files like SCSS and JS in `src/sphinx_book_theme/assets/*` into the production assets in `src/sphinx_book_theme/theme/sphinx_book_theme/static/` .
 This compilation is called by default, during development commands (see below).
 
 ## `tests/` - Testing infrastructure
 
 Testing infrastructure that uses `pytest` along with `beautifulsoup` to validate
 that the generated HTML is what we expect it to be.
 Much of these tests also use `pytest-regressions`, to check whether newly-generated HTML differs from previously-generated HTML.
```

### Comparing `tskit_book_theme-0.3.2/CHANGELOG.md` & `tskit_book_theme-1.0.1/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,95 @@
 # Changelog
 
+## v1.0.1 -- 2023-03-31
+
+This is a minor release supporting pydata>=0.13.3, with a few import changes from pydata.
+
+## v1.0.0 -- 2023-03-01
+
+This is a major release that brings in the latest PyData Sphinx Theme and a number of new features with it.
+It also overhauls and standardizes the HTML structure of the theme.
+Because of this large refactor, we are bumping the major version to `1.0`.
+Note that this doesn't imply any new long-term support or stability, we will continue to try not to make major breaking changes but will continue incrementing major versions if we must do so.
+
+### Enhancements made
+
+- PyData Sphinx Theme `v0.13`. See [the PyData Sphinx Theme `v0.13` release notes](https://github.com/pydata/pydata-sphinx-theme/releases/tag/v0.13.0) for details.
+- Icon links, more source providers, and bug fixes [#691](https://github.com/executablebooks/sphinx-book-theme/pull/691) ([@choldgraf](https://github.com/choldgraf), [@mmcky](https://github.com/mmcky))
+  - **We now support GitHub, GitLab, and BitBucket source providers**.
+  - **You can now include lists of icon links in your primary sidebar**.
+- Allowing inline elements in sidenotes and marginnotes [#641](https://github.com/executablebooks/sphinx-book-theme/pull/641) ([@AakashGfude](https://github.com/AakashGfude))
+- Improve Chinese (Taiwan) and Chinese (China) translation [#585](https://github.com/executablebooks/sphinx-book-theme/pull/585) ([@whyjz](https://github.com/whyjz))
+- sphinx >=4,<6 [#644](https://github.com/executablebooks/sphinx-book-theme/pull/644) ([@AakashGfude](https://github.com/AakashGfude))
+
+### Bugs fixed
+
+- FIX: Scroll padding on top for anchor links [#669](https://github.com/executablebooks/sphinx-book-theme/pull/669) ([@choldgraf](https://github.com/choldgraf))
+- 🐛 FIX: Correcting a broken link in CHANGELOG.md [#623](https://github.com/executablebooks/sphinx-book-theme/pull/623) ([@AakashGfude](https://github.com/AakashGfude))
+- FIX: Scroll to active navigation item [#609](https://github.com/executablebooks/sphinx-book-theme/pull/609) ([@ksuess](https://github.com/ksuess))
+- [FIX] Use logo url as is to allow for web urls. [#661](https://github.com/executablebooks/sphinx-book-theme/pull/661) ([@feanil](https://github.com/feanil))
+
+### Maintenance and upkeep improvements
+
+- MAINT: Update pre-commit versions and fix minor bugs in tests [#660](https://github.com/executablebooks/sphinx-book-theme/pull/660) ([@choldgraf](https://github.com/choldgraf))
+- MAINT: Move dependabot updates to monthly [#658](https://github.com/executablebooks/sphinx-book-theme/pull/658) ([@choldgraf](https://github.com/choldgraf))
+- MAINT: Factor publish to pypi workflow into dedicated file [#645](https://github.com/executablebooks/sphinx-book-theme/pull/645) ([@choldgraf](https://github.com/choldgraf))
+- MAINT: Remove duplication with pydata-sphinx-theme [#640](https://github.com/executablebooks/sphinx-book-theme/pull/640) ([@choldgraf](https://github.com/choldgraf))
+- MAINT: remove incorrect comment from sphinx pin. [#588](https://github.com/executablebooks/sphinx-book-theme/pull/588) ([@rossbar](https://github.com/rossbar))
+- IntersectionObserver at 1/3 screen [#567](https://github.com/executablebooks/sphinx-book-theme/pull/567) ([@choldgraf](https://github.com/choldgraf))
+
+### Documentation improvements
+
+- DOCS: Minor typo correction [#649](https://github.com/executablebooks/sphinx-book-theme/pull/649) ([@bmorris3](https://github.com/bmorris3))
+- DOC: Update kitchen sink [#610](https://github.com/executablebooks/sphinx-book-theme/pull/610) ([@choldgraf](https://github.com/choldgraf))
+
+### Breaking changes to structure and API
+
+- UPGRADE/BREAKING: PyData v0.13 and HTML refactoring [#677](https://github.com/executablebooks/sphinx-book-theme/pull/677) ([@choldgraf](https://github.com/choldgraf))
+- Remove JQuery and update versions [#668](https://github.com/executablebooks/sphinx-book-theme/pull/668) ([@choldgraf](https://github.com/choldgraf))
+
+### Tips for migration
+
+**Long sidebar entries now wrap**. If you'd like to un-do this and revert to old behavior (where they are cut off if too long), then use the following CSS rule in your custom Sphinx CSS:
+
+```css
+.bd-sidebar-primary a {
+  word-wrap: unset;
+}
+```
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/executablebooks/sphinx-book-theme/graphs/contributors?from=2022-07-17&to=2023-02-19&type=c))
+
+
+@12rambau ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3A12rambau+updated%3A2022-07-17..2023-03-01&type=Issues)) | @AakashGfude ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AAakashGfude+updated%3A2022-07-17..2023-03-01&type=Issues)) | @akhmerov ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aakhmerov+updated%3A2022-07-17..2023-03-01&type=Issues)) | @AllenDowney ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AAllenDowney+updated%3A2022-07-17..2023-03-01&type=Issues)) | @avivajpeyi ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aavivajpeyi+updated%3A2022-07-17..2023-03-01&type=Issues)) | @bmorris3 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Abmorris3+updated%3A2022-07-17..2023-03-01&type=Issues)) | @choldgraf ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Acholdgraf+updated%3A2022-07-17..2023-03-01&type=Issues)) | @chrisjsewell ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Achrisjsewell+updated%3A2022-07-17..2023-03-01&type=Issues)) | @consideRatio ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AconsideRatio+updated%3A2022-07-17..2023-03-01&type=Issues)) | @dependabot ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Adependabot+updated%3A2022-07-17..2023-03-01&type=Issues)) | @feanil ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Afeanil+updated%3A2022-07-17..2023-03-01&type=Issues)) | @fm75 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Afm75+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ghutchis ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aghutchis+updated%3A2022-07-17..2023-03-01&type=Issues)) | @guillaume-haerinck ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aguillaume-haerinck+updated%3A2022-07-17..2023-03-01&type=Issues)) | @haklc ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ahaklc+updated%3A2022-07-17..2023-03-01&type=Issues)) | @iasbusi ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aiasbusi+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ivirshup ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aivirshup+updated%3A2022-07-17..2023-03-01&type=Issues)) | @James11222 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AJames11222+updated%3A2022-07-17..2023-03-01&type=Issues)) | @kloczek ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Akloczek+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ksuess ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aksuess+updated%3A2022-07-17..2023-03-01&type=Issues)) | @martinfleis ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amartinfleis+updated%3A2022-07-17..2023-03-01&type=Issues)) | @mathbunnyru ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amathbunnyru+updated%3A2022-07-17..2023-03-01&type=Issues)) | @mcjulian1107 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amcjulian1107+updated%3A2022-07-17..2023-03-01&type=Issues)) | @melund ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amelund+updated%3A2022-07-17..2023-03-01&type=Issues)) | @mmcky ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ammcky+updated%3A2022-07-17..2023-03-01&type=Issues)) | @paugier ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apaugier+updated%3A2022-07-17..2023-03-01&type=Issues)) | @PhilipVinc ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3APhilipVinc+updated%3A2022-07-17..2023-03-01&type=Issues)) | @pradyunsg ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apradyunsg+updated%3A2022-07-17..2023-03-01&type=Issues)) | @pre-commit-ci ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apre-commit-ci+updated%3A2022-07-17..2023-03-01&type=Issues)) | @rkdarst ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Arkdarst+updated%3A2022-07-17..2023-03-01&type=Issues)) | @rossbar ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Arossbar+updated%3A2022-07-17..2023-03-01&type=Issues)) | @scmmmh ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ascmmmh+updated%3A2022-07-17..2023-03-01&type=Issues)) | @sieler ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Asieler+updated%3A2022-07-17..2023-03-01&type=Issues)) | @SilverRainZ ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3ASilverRainZ+updated%3A2022-07-17..2023-03-01&type=Issues)) | @stevepiercy ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Astevepiercy+updated%3A2022-07-17..2023-03-01&type=Issues)) | @trallard ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Atrallard+updated%3A2022-07-17..2023-03-01&type=Issues)) | @whyjz ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Awhyjz+updated%3A2022-07-17..2023-03-01&type=Issues)) | @yuvipanda ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ayuvipanda+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ZedThree ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AZedThree+updated%3A2022-07-17..2023-03-01&type=Issues))
+
+
+## v0.3.3 -- 2022-07-17
+
+### Fixes:
+
+- Style edits for last-child zero-margin on dd's [#586](https://github.com/executablebooks/sphinx-book-theme/pull/586) ([@benjaoming](https://github.com/benjaoming))
+- Escape colon in JupyterHub link to repo [#556](https://github.com/executablebooks/sphinx-book-theme/pull/556) ([@matthew-brett](https://github.com/matthew-brett))
+- Myst-nb pinning to 0.13.2 [#560](https://github.com/executablebooks/sphinx-book-theme/pull/560) ([@choldgraf](https://github.com/choldgraf))
+- Stylizing ReadTheDocs in `_readthedocs.scss` as per guidelines [#579](https://github.com/executablebooks/sphinx-book-theme/pull/579) ([@pradyunsg](https://github.com/pradyunsg))
+- `templates_path` in config was overriding any value append to `templates_path` in this package. [#566](https://github.com/executablebooks/sphinx-book-theme/pull/566) ([@AakashGfude](https://github.com/AakashGfude))
+
+### Enhancements made:
+
+- Added sidenote and marginnote using footnote syntax [#546](https://github.com/executablebooks/sphinx-book-theme/pull/546) ([@AakashGfude](https://github.com/AakashGfude))
+
+### Docs:
+
+- Added Docs for sphinx-examples [#550](https://github.com/executablebooks/sphinx-book-theme/pull/550) ([@choldgraf](https://github.com/choldgraf))
+- Lychee link fixes [#553](https://github.com/executablebooks/sphinx-book-theme/pull/553) ([@choldgraf](https://github.com/choldgraf))
+- Beta and lychee link fix [#552](https://github.com/executablebooks/sphinx-book-theme/pull/552) ([@choldgraf](https://github.com/choldgraf))
+
+
 ## v0.3.2 -- 2022-03-28
 
 Two patch releases fixed two bugs for figure content in the margin.
 
 ## v0.3.0 - 2022-03-25
 
 This is a significant change in the HTML and CSS of the site, with the goal of making it more standardized and robust. There are several design tweaks that have been made. Here is a short overview:
@@ -12,15 +98,15 @@
 - The HTML structure of the site has been re-worked to make `sticky` and other CSS behaviors more dependable.
 - The header buttons are now standardized and have an updated look and feel.
 - The in-page margin CSS is now more reliable
 - Improvements to scrollbar style throughout the site
 
 See the PRs below for where most of these changes occurred.
 
-([full changelog](https://github.com/executablebooks/tskit-book-theme/compare/v0.2.0...d9c1abc4197445faab7892291520de448f363274))
+([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.2.0...d9c1abc4197445faab7892291520de448f363274))
 
 ### Enhancements made
 
 - ‼️ REFACTOR: HTML and CSS restructuring [#472](https://github.com/executablebooks/sphinx-book-theme/pull/472) ([@choldgraf](https://github.com/choldgraf))
 - ENH: Standardize scrollbar behavior [#481](https://github.com/executablebooks/sphinx-book-theme/pull/481) ([@choldgraf](https://github.com/choldgraf))
 - ENH: Standardize header buttons [#490](https://github.com/executablebooks/sphinx-book-theme/pull/490) ([@choldgraf](https://github.com/choldgraf))
 - ENH: Updating search page style [#491](https://github.com/executablebooks/sphinx-book-theme/pull/491) ([@choldgraf](https://github.com/choldgraf))
@@ -208,19 +294,19 @@
 - Fixing linenos style [#263](https://github.com/executablebooks/sphinx-book-theme/pull/263) ([@AakashGfude](https://github.com/AakashGfude))
 
 
 ## v0.0.39 - 2020-11-08
 ([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.0.38...v0.0.39))
 
 ### New features added
-* sphinx sidebars functionality [#233](https://github.com/executablebooks/sphinx-book-theme/pull/233) ([@choldgraf](https://github.com/choldgraf)). You can now use the `html_sidebars` functionality that is native in Sphinx. [See the sidebars documentation](https://sphinx-book-theme.readthedocs.io/en/latest/customize/sidebar-primary.html).
-* Collapsible lists in sidebars [#226](https://github.com/executablebooks/sphinx-book-theme/pull/226) ([@AakashGfude](https://github.com/AakashGfude)). Sidebars that have nested sections will now have an arrow that allows you to reveal these sections without changing the current page. You can [control the depth](https://sphinx-book-theme.readthedocs.io/en/latest/customize/sidebar-primary.html#control-the-depth-of-the-left-sidebar-lists-to-expand) of expanded sections with `show_navbar_depth`.
+* sphinx sidebars functionality [#233](https://github.com/executablebooks/sphinx-book-theme/pull/233) ([@choldgraf](https://github.com/choldgraf)). You can now use the `html_sidebars` functionality that is native in Sphinx. [See the sidebars documentation](https://sphinx-book-theme.readthedocs.io/en/latest/sections/sidebar-primary.html).
+* Collapsible lists in sidebars [#226](https://github.com/executablebooks/sphinx-book-theme/pull/226) ([@AakashGfude](https://github.com/AakashGfude)). Sidebars that have nested sections will now have an arrow that allows you to reveal these sections without changing the current page. You can [control the depth](https://sphinx-book-theme.readthedocs.io/en/latest/sections/sidebar-primary.html#control-the-depth-of-the-left-sidebar-lists-to-expand) of expanded sections with `show_navbar_depth`.
 
 ### Enhancements made
-* Option for download button [#245](https://github.com/executablebooks/sphinx-book-theme/pull/245) ([@bknaepen](https://github.com/bknaepen)). The "download" button used to be automatically added, but can now be removed. See [the download button configuration](https://sphinx-book-theme.readthedocs.io/en/latest/customize/download.html).
+* Option for download button [#245](https://github.com/executablebooks/sphinx-book-theme/pull/245) ([@bknaepen](https://github.com/bknaepen)). The "download" button used to be automatically added, but can now be removed. See [the download button configuration](https://sphinx-book-theme.readthedocs.io/en/latest/components/download.html).
 
 ## v0.0.38
 
 ## Enhancements made
 👌 IMPROVE: Add missing aria-label to fullscreen button [#228](https://github.com/executablebooks/sphinx-book-theme/pull/228) ([@foster999](https://github.com/foster999))
 
 👌 IMPROVE: declare parallel read safe [#225](https://github.com/executablebooks/sphinx-book-theme/pull/225) ([@rscohn2](https://github.com/rscohn2))
@@ -243,15 +329,15 @@
 ([GitHub contributors page for this release](https://github.com/executablebooks/sphinx-book-theme/graphs/contributors?from=2020-08-25&to=2020-09-28&type=c))
 
 [@choldgraf](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Acholdgraf+updated%3A2020-08-25..2020-09-28&type=Issues) | [@chrisjsewell](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Achrisjsewell+updated%3A2020-08-25..2020-09-28&type=Issues) | [@fm75](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Afm75+updated%3A2020-08-25..2020-09-28&type=Issues) | [@hason](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ahason+updated%3A2020-08-25..2020-09-28&type=Issues) | [@najuzilu](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Anajuzilu+updated%3A2020-08-25..2020-09-28&type=Issues) | [@nathancarter](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Anathancarter+updated%3A2020-08-25..2020-09-28&type=Issues) | [@pauleveritt](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apauleveritt+updated%3A2020-08-25..2020-09-28&type=Issues) | [@pradyunsg](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apradyunsg+updated%3A2020-08-25..2020-09-28&type=Issues) |
 
 ## v0.0.36 2020-08-25
 
 👌 IMPROVED: The main theme change in this release, is the addition of CSS styling for definition lists, including those created by [sphinx.ext.autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html).
-See [Definition and Field Lists](https://sphinx-book-theme.readthedocs.io/en/latest/reference/kitchen-sink/lists-and-tables.html), and the [Python API documentation](https://sphinx-book-theme.readthedocs.io/en/latest/reference/kitchen-sink/api.html).
+See [Definition and Field Lists](https://sphinx-book-theme.readthedocs.io/en/latest/reference/kitchen-sink/lists.html), and the [Python API documentation](https://sphinx-book-theme.readthedocs.io/en/latest/reference/kitchen-sink/api.html).
 
 🔧 MAINTENANCE: Under the hood, there has also been work undertaken to improve the development environment for working with the package. Thanks to [@pradyunsg](https://github.com/pradyunsg).
 
 ### Contributors to this release
 
 [@chrisjsewell](https://github.com/chrisjsewell) | [@pradyunsg](https://github.com/pradyunsg)
```

### Comparing `tskit_book_theme-0.3.2/LICENSE` & `tskit_book_theme-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/README.md` & `tskit_book_theme-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-# tskit-book-theme
+# sphinx-book-theme
 
 [![codecov][codecov-badge]][codecov-link] [![Documentation Status][rtd-badge]][rtd-link] [![PyPI][pypi-badge]][pypi-link]
 
-**An interactive book theme for tskit ecosystem projects**.
-
-Forked from sphinx-book-theme.
+**An interactive book theme for Sphinx**.
 
 This is a lightweight Sphinx theme designed to mimic the look-and-feel of an
 interactive book. It has the following primary features:
 
-* **Bootstrap 4**
+* **Bootstrap 5**
   for visual elements and functionality.
 * **Flexible content layout** that is inspired by beautiful online books,
   such as [the Edward Tufte CSS guide](https://edwardtufte.github.io/tufte-css/)
 * **Visual classes designed for Jupyter Notebooks**. Cell inputs, outputs,
   and interactive functionality are all supported.
 * **Launch buttons for online interactivity**. For pages that are built with
   computational material, connect your site to an online BinderHub for interactive content.
 
 ## Get started
 
-To get started with `tskit-book-theme`, first install it with `pip`:
+To get started with `sphinx-book-theme`, first install it with `pip`:
 
 ```
-pip install tskit-book-theme
+pip install sphinx-book-theme
 ```
 
 then, activate the theme in your Sphinx configuration (`conf.py`):
 
 ```
 ...
-html_theme = "tskit_book_theme"
+html_theme = "sphinx_book_theme"
 ...
 ```
 
 This will activate the Sphinx Book Theme for your documentation. Note that you may
 need to change your `html_theme_options` configuration depending on your previous
 theme. See the pages to the left for information about what you can configure with
-`tskit-book-theme`.
+`sphinx-book-theme`.
 
 ## Documentation
 
 See [the Sphinx Book Theme documentation](https://sphinx-book-theme.readthedocs.io/en/latest/)
 for more information.
 
 [codecov-badge]: https://codecov.io/gh/executablebooks/sphinx-book-theme/branch/master/graph/badge.svg
```

### Comparing `tskit_book_theme-0.3.2/docs/_static/logo-square.svg` & `tskit_book_theme-1.0.1/docs/_static/logo-square.svg`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/_static/logo-wide.svg` & `tskit_book_theme-1.0.1/docs/_static/logo-wide.svg`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/conf.py` & `tskit_book_theme-1.0.1/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -- Project information -----------------------------------------------------
 import os
+from urllib.request import urlopen
 from pathlib import Path
-from urllib import request
 
 project = "Sphinx Book Theme"
-copyright = "2020"
+copyright = "2023"
 author = "the Executable Book Project"
 # language = "fr"  # For testing language translations
 
 master_doc = "index"
 
 # -- General configuration ---------------------------------------------------
 
@@ -27,27 +27,30 @@
     "sphinx_design",
     "sphinx_examples",
     "sphinx_tabs.tabs",
     "sphinx_thebe",
     "sphinx_togglebutton",
     "sphinxcontrib.bibtex",
     "sphinxext.opengraph",
+    # For the kitchen sink
+    "sphinx.ext.todo",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3.8", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master", None),
+    "pst": ("https://pydata-sphinx-theme.readthedocs.io/en/latest/", None),
 }
 nitpick_ignore = [
     ("py:class", "docutils.nodes.document"),
     ("py:class", "docutils.parsers.rst.directives.body.Sidebar"),
 ]
 
 suppress_warnings = ["myst.domains", "ref.ref"]
@@ -70,113 +73,145 @@
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "tskit_book_theme"
 html_logo = "_static/logo-wide.svg"
-html_title = "Tskit Book Theme"
+html_title = "Sphinx Book Theme"
 html_copy_source = True
-html_sourcelink_suffix = ""
 html_favicon = "_static/logo-square.svg"
 html_last_updated_fmt = ""
 
 html_sidebars = {
     "reference/blog/*": [
-        "sidebar-logo.html",
+        "navbar-logo.html",
         "search-field.html",
         "postcard.html",
         "recentposts.html",
         "tagcloud.html",
         "categories.html",
         "archives.html",
         "sbt-sidebar-nav.html",
     ]
 }
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["custom.css"]
-jupyter_execute_notebooks = "cache"
+nb_execution_mode = "cache"
 thebe_config = {
     "repository_url": "https://github.com/binder-examples/jupyter-stacks-datascience",
     "repository_branch": "master",
 }
 
 html_theme_options = {
     "path_to_docs": "docs",
-    "repository_url": "https://github.com/benjeffery/tskit-book-theme",
-    # "repository_branch": "gh-pages",  # For testing
+    "repository_url": "https://github.com/executablebooks/sphinx-book-theme",
+    "repository_branch": "master",
     "launch_buttons": {
         "binderhub_url": "https://mybinder.org",
         "colab_url": "https://colab.research.google.com/",
         "deepnote_url": "https://deepnote.com/",
         "notebook_interface": "jupyterlab",
         "thebe": True,
         # "jupyterhub_url": "https://datahub.berkeley.edu",  # For testing
     },
     "use_edit_page_button": True,
+    "use_source_button": True,
     "use_issues_button": True,
-    "use_repository_button": True,
+    # "use_repository_button": True,
     "use_download_button": True,
     "use_sidenotes": True,
-    "logo_only": True,
     "show_toc_level": 2,
     "announcement": (
         "⚠️The latest release refactored our HTML, "
         "so double-check your custom CSS rules!⚠️"
     ),
+    "logo": {
+        "image_dark": "_static/logo-wide-dark.svg",
+        # "text": html_title,  # Uncomment to try text with logo
+    },
+    "icon_links": [
+        {
+            "name": "Executable Books",
+            "url": "https://executablebooks.org/",
+            "icon": "_static/ebp-logo.png",
+            "type": "local",
+        },
+        {
+            "name": "GitHub",
+            "url": "https://github.com/executablebooks/sphinx-book-theme",
+            "icon": "fa-brands fa-github",
+        },
+        {
+            "name": "PyPI",
+            "url": "https://pypi.org/project/sphinx-book-theme/",
+            "icon": "https://img.shields.io/pypi/dw/sphinx-book-theme",
+            "type": "url",
+        },
+    ],
     # For testing
     # "use_fullscreen_button": False,
     # "home_page_in_toc": True,
-    # "single_page": True,
     # "extra_footer": "<a href='https://google.com'>Test</a>",  # DEPRECATED KEY
-    # "extra_navbar": "<a href='https://google.com'>Test</a>",
     # "show_navbar_depth": 2,
+    # Testing layout areas
+    # "navbar_start": ["test.html"],
+    # "navbar_center": ["test.html"],
+    # "navbar_end": ["test.html"],
+    # "navbar_persistent": ["test.html"],
+    # "footer_start": ["test.html"],
+    # "footer_end": ["test.html"]
+}
+
+# sphinxext.opengraph
+ogp_social_cards = {
+    "image": "_static/logo-square.png",
 }
 
 # -- ABlog config -------------------------------------------------
 blog_path = "reference/blog"
 blog_post_pattern = "reference/blog/*.md"
 blog_baseurl = "https://sphinx-book-theme.readthedocs.io"
 fontawesome_included = True
 post_auto_image = 1
 post_auto_excerpt = 2
-execution_show_tb = "READTHEDOCS" in os.environ
+nb_execution_show_tb = "READTHEDOCS" in os.environ
 bibtex_bibfiles = ["references.bib"]
 # To test that style looks good with common bibtex config
 bibtex_reference_style = "author_year"
 bibtex_default_style = "plain"
-
+numpydoc_show_class_members = False  # for automodule:: urllib.parse stub file issue
 linkcheck_ignore = [
     "http://someurl/release",  # This is a fake link
     "https://doi.org",  # These don't resolve properly and cause SSL issues
 ]
 
-# -- Download kitchen sink reference docs -------------------------------------
-# These are the kitchen sink files used by the Sphinx Themes gallery at
-# https://github.com/sphinx-themes/sphinx-themes.org
-# To re-download, delete the `references/kitchen-sink` folder and build the docs
-kitchen_sink_files = [
-    "api.rst",
-    "index.rst",
-    "lists-and-tables.rst",
-    "paragraph-markup.rst",
-]
-for ifile in kitchen_sink_files:
-    path_file = Path(f"reference/kitchen-sink/{ifile}")
-    path_file.parent.mkdir(exist_ok=True)
-    if not path_file.exists():
-        print(f"Downloading kitchen sink file {ifile}")
-        resp = request.urlopen(
-            f"https://github.com/sphinx-themes/sphinx-themes.org/raw/master/sample-docs/kitchen-sink/{ifile}"  # noqa: E501
-        )
-        header = ".. DOWNLOADED FROM sphinx-themes.org, DO NOT MANUALLY EDIT\n"
-        path_file.write_text(header + resp.read().decode())
+
+# -- Download latest theme elements page from PyData -----------------------------
+
+path_pydata_content = "https://raw.githubusercontent.com/pydata/pydata-sphinx-theme/main/docs/user_guide/theme-elements.md"  # noqa
+path_content_file = Path(__file__).parent / "content/pydata-content-blocks.md"
+if not path_content_file.exists():
+    with urlopen(path_pydata_content) as resp:
+        # Read in the content page file, then update the title and add context
+        content = resp.read().decode().split("\n")
+        ix_title = content.index("# Theme-specific elements")
+        content[ix_title] = "# PyData Theme Elements"
+        content.insert(
+            ix_title + 1,
+            "\nThis is a collection of content blocks with special support from this theme's parent theme, [the PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/latest/user_guide/theme-elements.html)\n",  # noqa
+        )  # noqa
+        content = "\n".join(content)
+        # Replace a relative link in the pydata docs w/ the respective one here
+        content = content.replace("../examples/pydata.md", "notebooks.md")
+        # Write to disk in a location that will be ignored by git
+        path_content_file.write_text(content)
 
 
 def setup(app):
     # -- To demonstrate ReadTheDocs switcher -------------------------------------
     # This links a few JS and CSS files that mimic the environment that RTD uses
     # so that we can test RTD-like behavior. We don't need to run it on RTD and we
     # don't wanted it loaded in GitHub Actions because it messes up the lighthouse
```

### Comparing `tskit_book_theme-0.3.2/docs/content-blocks.md` & `tskit_book_theme-1.0.1/docs/content/content-blocks.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Special content blocks
 
 There are a few content blocks that are unique to this theme.
 
 
 ## Quotations and epigraphs
 
-Here is what quotations and epigraphs look like in `tskit-book-theme`:
+Here is what quotations and epigraphs look like in `sphinx-book-theme`:
 
 ```{example} Default markdown quotes
 > Here's my quote, it's pretty neat.
 > I wonder how many lines I can create with
 > a single stream-of-consciousness quote.
 > I could try to add a list of ideas to talk about.
 > I suppose I could just keep going on forever,
@@ -154,15 +154,15 @@
 
 You can configure figures to use the margin for captions.
 Here is a figure with a caption to the right.
 
 ::::{example}
 :no-container:
 
-```{figure} images/cool.jpg
+```{figure} ../images/cool.jpg
 ---
 width: 60%
 figclass: margin-caption
 alt: My figure text
 name: myfig5
 ---
 And here is my figure caption, if you look to the left, you can see that COOL is in big red letters. But you probably already noticed that, really I am just taking up space to see how the margin caption looks like when it is really long :-).
@@ -195,15 +195,15 @@
 Here is a figure with a caption below. We'll add a note below to create
 some vertical space to see better.
 
 ````{example}
 :no-container:
 :reverse:
 
-```{figure} images/cool.jpg
+```{figure} ../images/cool.jpg
 ---
 figclass: margin
 alt: My figure text
 name: myfig4
 ---
 And here is my figure caption
 ```
@@ -233,15 +233,15 @@
 `````{example} Admonitions and images in the margin
 :no-container:
 :reverse:
 
 ````{margin} **Notes in margins**
 ```{note}
 Wow, a note with an image in a margin!
-![](images/cool.jpg)
+![](../images/cool.jpg)
 ```
 ````
 `````
 
 ## Sidebars
 
 Sidebars exist in-line with your text, but allow the rest of the
@@ -252,15 +252,15 @@
 `````{example}
 :no-container:
 
 ````{sidebar} **My sidebar title**
 ```{note}
 Here is my sidebar content, it is pretty cool!
 ```
-![](images/cool.jpg)
+![](../images/cool.jpg)
 ````
 `````
 
 Note how the content wraps around the sidebar to the right.
 However, the sidebar text will still be in line with your content. There are
 certain kinds of elements, such as "note" blocks and code cells, that may
 clash with your sidebar. If this happens, try using a `{margin}` instead.
```

### Comparing `tskit_book_theme-0.3.2/docs/contributing/index.md` & `tskit_book_theme-1.0.1/docs/contributing/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Contribute to this theme
+# Contributing guide
 
 Thank you for being interested in contributing to the `sphinx-book-theme`! You
 are awesome ✨.
 
-This project follows the Executable Books Project [contribution guidelines](https://executablebooks.org/en/latest/contributing.html).
+This project follows the Executable Books Project [contribution guidelines](https://executablebooks.org/en/latest/contribute).
 It contains information about our conventions around coding style, pull request workflow, commit messages and more.
 
 The rest of these sections contain information about developing the `sphinx-book-theme` specifically.
 
 ```{toctree}
 :maxdepth: 2
 :caption: Contributing Guide
 setup
 architecture
 style
 tests
+versions
 translate
 subthemes
 ```
```

### Comparing `tskit_book_theme-0.3.2/docs/contributing/setup.md` & `tskit_book_theme-1.0.1/docs/contributing/setup.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 First we'll install the necessary tools that you can use to begin making changes.
 Follow these steps:
 
 1. Get the source code of this project using git:
 
    ```bash
-   git clone https://github.com/benjeffery/tskit-book-theme
-   cd tskit-book-theme
+   git clone https://github.com/executablebooks/sphinx-book-theme
+   cd sphinx-book-theme
    ```
 
 2. Ensure you have Python 3.7 or newer!
 3. Install `tox`.
    `tox` is a tool for managing virtual environments for test suites or common jobs that are run with a repository.
    It ensures that your environment is consistent each time you build the docs or run tests.
 
@@ -66,26 +66,26 @@
 You may then preview them by opening one of the HTML files.
 
 ## Update the theme's assets (CSS/JS)
 
 Now that you've previewed the documentation, try making changes to this theme's assets and see how they affect the documentation builds.
 This is an easy way to preview the effect that your changes will make.
 
-First, **make your changes in `src/tskit_book_theme/assets/`**.
+First, **make your changes in `src/sphinx_book_theme/assets/`**.
 This folder contains all of the SCSS and Javascript that are used in this site.
 For example, edit one of the `scss` files to add or modify a rule.
 
 Next, **compile the changes**.
 Run the following command:
 
 ```console
 $ tox -e compile
 ```
 
-This uses the [Sphinx Theme Builder](https://sphinx-theme-builder.readthedocs.io/) to compile our SCSS/JS files and bundle them with our theme at `src/tskit_book_theme/theme/tskit_book_theme/static`.
+This uses the [Sphinx Theme Builder](https://sphinx-theme-builder.readthedocs.io/) to compile our SCSS/JS files and bundle them with our theme at `src/sphinx_book_theme/theme/sphinx_book_theme/static`.
 These compiled assets are **not included** in our git repository, but they **are included** in distributions of the theme.
 
 Finally, **re-build the documentation** to preview your changes:
 
 ```console
 $ rm -rf docs/_build/html
 $ tox -e docs-update
```

### Comparing `tskit_book_theme-0.3.2/docs/contributing/style.md` & `tskit_book_theme-1.0.1/docs/contributing/style.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 - The [Furo theme](https://pradyunsg.me/furo/)
 - The [Edward Tufte CSS theme](https://edwardtufte.github.io/tufte-css/)
 - [GitBook](https://docs.gitbook.com/)
 - The [Tailwind CSS docs](https://tailwindcss.com/docs/installation)
 
 ## SCSS build process
 
-Our SCSS source files at in `src/tskit_book_theme/assets/styles`.
-We use the [Sphinx Theme Builder](https://github.com/pradyunsg/sphinx-theme-builder) tp compile these assets and bundle them with the theme at `src/tskit_book_theme/theme/tskit_book_theme/static/styles`.
+Our SCSS source files at in `src/sphinx_book_theme/assets/styles`.
+We use the [Sphinx Theme Builder](https://github.com/pradyunsg/sphinx-theme-builder) tp compile these assets and bundle them with the theme at `src/sphinx_book_theme/theme/sphinx_book_theme/static/styles`.
 
 These compiled files are **not checked in to `git` history**.
 
 You can run the compilation process with `tox` like so:
 
 ```console
 $ tox -e compile
```

### Comparing `tskit_book_theme-0.3.2/docs/contributing/subthemes.md` & `tskit_book_theme-1.0.1/docs/contributing/subthemes.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 This theme defines a function called `hash_html_assets` that can be used to create hashes for your style files, and updates the Sphinx links to include them with `?digest=`.
 You can re-use this function in a sub-theme if you wish - to do so, look at the function signature of `hash_html_assets`.
 
 For example, here's a Python snippet that reuses this function:
 
 ```python
-from tskit_book_theme import hash_assets_for_files
+from sphinx_book_theme import hash_assets_for_files
 
 def hash_html_assets(app, pagename, templatename, context, doctree):
     assets = ["styles/your-css-asset.css", "scripts/your-js-asset.js"]
     STATIC_PATH = "path to your theme's static folder"
     hash_assets_for_files(assets, STATIC_PATH, context)
 
 def setup(app):
@@ -30,11 +30,11 @@
 ## Defining your own CSS
 
 If you'd like to define a new CSS stylesheet for your sub-theme, make sure to import the CSS for this theme as well.
 As a best practice, you should put your sub-theme's CSS stylesheet in the `STATIC_PATH/styles/` folder, similar to this theme.
 Then, you can import this theme's CSS with:
 
 ```scss
-@import "tskit-book-theme.css";
+@import "sphinx-book-theme.css";
 
 // And include your own CSS below
 ```
```

### Comparing `tskit_book_theme-0.3.2/docs/contributing/tests.md` & `tskit_book_theme-1.0.1/docs/contributing/tests.md`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/customize/announcements.md` & `tskit_book_theme-1.0.1/docs/sections/announcements.md`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/customize/custom-css.md` & `tskit_book_theme-1.0.1/docs/components/custom-css.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Add your own CSS rules
 
 To customize the look of your site further, you can customize your CSS stylesheets,
-as described in the [ReadTheDocs Docs](https://docs.readthedocs.io/en/stable/guides/adding-custom-css.html#adding-custom-css-or-javascript-to-sphinx-documentation).
+as described in the [ReadTheDocs Docs](https://docs.readthedocs.io/en/stable/guides/adding-custom-css.html).
 
 First, create a CSS file and place it in `_static/custom.css`.
 An example CSS file to change the color of the top-level headers might look like this.
 
 ```css
 h1 {
     color: #003B71 !important;
```

### Comparing `tskit_book_theme-0.3.2/docs/customize/index.md` & `tskit_book_theme-1.0.1/docs/reference.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# Customization
 
-These sections describe a few ways that you may customize the look and feel of your theme.
+# Reference of theme options
 
-## Theme options
+The following theme-specific options are available via `html_theme_options`.
 
-The following options are available via `html_theme_options`
+```{admonition} See the PyData Theme as well
+These are **in addition to** all of the {external:doc}`options available in the PyData Sphinx Theme <user_guide/index>`.
+```
 
 ```{list-table}
 :widths: 10 5 40
 :header-rows: 1
 * - Key
   - Type
   - Description
-* - `single_page`
-  - bool
-  - Remove the left sidebar and treat the site as a single page. See [](customize:single-page).
 * - `path_to_docs`
   - string
   - Path to the documentation, relative to the repository root (e.g. `docs/`). See [](customize:source-files).
 * - `repository_url`
   - string
   - URL of the repository for the documentation (e.g. the GitHub repository URL). See [](source-files:repository).
 * - `repository_branch`
@@ -38,38 +36,17 @@
   - Add a button in the header that links to the repository of the documentation.See [](source-files:repository).
 * - `launch_buttons`
   - bool
   - Include Binder launch buttons for pages that were built from Jupyter Notebooks. See [](customize:launch).
 * - `home_page_in_toc`
   - bool
   - Whether to put the home page in the Navigation Bar (at the top). See [](sidebar-primary:home-page).
-* - `logo_only`
-  - bool
-  - Only display the logo, not `html_title` if it exists.
 * - `show_navbar_depth`
   - int
   - Show children in the navigation bar down to the depth listed here. See [](sidebar:navbar-depth).
-* - `extra_navbar`
-  - str
-  - Extra HTML to add below the sidebar footer. See [](custom-footer).
 * - `extra_footer`
   - str
   - Extra HTML to add in the footer of each page.
 * - `toc_title`
   - str
   - The text to be displayed with the in-page TOC (`Contents` is default)
 ```
-
-## Customization Topics
-
-The following sections describe a few ways to customize the theme in more depth.
-
-```{toctree}
-sidebar-primary.md
-sidebar-secondary.md
-announcements.md
-header.md
-download.md
-source-files.md
-custom-css.md
-single-page.md
-```
```

### Comparing `tskit_book_theme-0.3.2/docs/customize/sidebar-primary.md` & `tskit_book_theme-1.0.1/docs/sections/sidebar-primary.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Customize the primary sidebar
+# Primary sidebar and navigation
 
 The primary sidebar generally contains the site navigation and logo.
 By default it is on the left side of the site.
 This page describes ways that you can control and customize the primary sidebar.
 
 (sidebar-primary:items)=
 ## Control the left sidebar items
@@ -29,62 +29,23 @@
 
 See the [Sphinx HTML sidebars documentation](https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_sidebars) for more information.
 
 ### Default sidebar elements
 
 By default, this theme comes with these three theme-specific sidebar elements enabled on all pages:
 
-- `sidebar-logo.html`: Displays the logo and site title.
+- `navbar-logo.html`: Displays the logo and site title.
 - `search-field.html`: A bootstrap-based search bar (from the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/))
 - `sbt-sidebar-nav.html`: A bootstrap-based navigation menu for your book.
-- `sbt-sidebar-footer`: A [configurable](custom-footer) snippet of HTML to add to the sidebar (by default it is placed at the bottom).
-
-(custom-footer)=
-## Customize the sidebar footer
-
-You may choose your own HTML to include in the footer of your sidebar (or set it to be empty). To do so, set the following option in `conf.py`:
-
-```python
-html_theme_options = {
-    ...
-    "extra_navbar": "<p>Your HTML</p>",
-    ...
-}
-```
-
-This text will be placed at the bottom of the sidebar by default.
-
 
 ## Add a header to your Table of Contents
 
 If you'd like to add a header above a section of TOC links, use `:caption: My header text`
 in your `toctree` directive for that section.
 
-(sidebar-primary:logo)=
-## Customize the logo, title, and favicon
-
-You can customize the logo, title, and favicon of your site with the following Sphinx configuration in `conf.py`:
-
-```python
-html_title = "Your title"
-html_logo = "path/to/logo.png"
-html_favicon = "path/to/favicon.ico"
-```
-
-These will be placed in the top-left of your page.
-
-To **remove the site title** below the logo, add this line in `conf.py`:
-
-```python
-html_theme_options = {
-  ...
-  "logo_only": True,
-  ...
-}
-```
 
 (sidebar-primary:home-page)=
 ## Add the home page to your table of contents
 
 By default, your table of contents will begin with the first file that you add to a `toctree`. You can also configure the theme to show the **landing page** of the theme in your navigation bar as well.
 
 To add the landing page of your site to the table of contents, use the following configuration:
```

### Comparing `tskit_book_theme-0.3.2/docs/customize/sidebar-secondary.md` & `tskit_book_theme-1.0.1/docs/sections/sidebar-secondary.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Customize the secondary sidebar
+# Secondary sidebar and table of contents
 
 The secondary sidebar contains information about the current page.
 It begins at the top of the page (in the header), and extends downwards (by default, from the right side of the page).
 This page describes ways to control and customize the secondary sidebar.
 
 ## Rename the in-page Table of Contents
```

### Comparing `tskit_book_theme-0.3.2/docs/images/cool.jpg` & `tskit_book_theme-1.0.1/docs/images/cool.jpg`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/index.md` & `tskit_book_theme-1.0.1/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 [Flexible content layout](reference/special-theme-elements.md)
 : Inspired by beautiful online books, such as [the Edward Tufte CSS guide](https://edwardtufte.github.io/tufte-css/)
 
 [Visual classes designed for Jupyter Notebooks](reference/notebooks)
 : Cell inputs, outputs, and interactive functionality are all supported.
 
-[Launch buttons for online interactivity](launch)
+[Launch buttons for online interactivity](content/launch)
 : For pages that are built with computational material, connect your site to an online BinderHub for interactive content.
 
-[Bootstrap 4](https://getbootstrap.com/docs/4.0/getting-started/introduction/)
+[Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
 : To style visual elements and add functionality.
 
 International
 : All text integrated in the theme is translated to the specified [Sphinx language](https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-language).
 
 :::{seealso}
 This is the default theme in [Jupyter Book](https://jupyterbook.org).
@@ -48,45 +48,45 @@
 The following topic areas will help you understand and use the theme.
 
 ```{toctree}
 :maxdepth: 1
 :caption: Topic Areas
 
 tutorials/get-started
-customize/index
-content-blocks
-notebooks
-launch
+content/index
+sections/index
+components/index
+reference
 contributing/index
+changelog
 ```
 
-# Reference pages
+# Example pages
 
-Reference pages demonstrate the visual look of this theme.
+Examples pages demonstrate the visual look of this theme.
 
 ```{toctree}
-:caption: Reference
+:caption: Example pages
 :maxdepth: 2
 
 reference/kitchen-sink/index
 reference/special-theme-elements
 reference/extensions
 reference/notebooks
 reference/thebe
 reference/blog
 reference/api-numpy
 reference/comments
-changelog
 ```
 
 # Inspiration
 
 This theme draws inspiration and borrows design elements from the following themes:
 
 - The [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/)
 - The [Furo theme](https://pradyunsg.me/furo/)
 - The [Edward Tufte CSS theme](https://edwardtufte.github.io/tufte-css/)
 - [GitBook](https://docs.gitbook.com/)
 - The [Tailwind CSS docs](https://tailwindcss.com/docs/installation)
 
-[pypi-badge]: https://img.shields.io/pypi/v/tskit-book-theme.svg
-[pypi-link]: https://pypi.org/project/tskit-book-theme
+[pypi-badge]: https://img.shields.io/pypi/v/sphinx-book-theme.svg
+[pypi-link]: https://pypi.org/project/sphinx-book-theme
```

### Comparing `tskit_book_theme-0.3.2/docs/launch.md` & `tskit_book_theme-1.0.1/docs/content/launch.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 documentation's repository url:
 
 ```python
 html_theme_options = {
     ...
     "repository_url": "https://github.com/{your-docs-url}",
     "repository_branch": "{your-branch}",
-    "path_to_docs": "{path-relative-to-site-root},
+    "path_to_docs": "{path-relative-to-site-root}",
     ...
 }
 ```
 
 ```{margin} Paired ipynb files
 
 If you're using [Jupytext](https://jupytext.readthedocs.io/en/latest/) to
@@ -58,15 +58,15 @@
 
 To add Google Colab links to your page, add the following configuration:
 
 ```python
 html_theme_options = {
     ...
     "launch_buttons": {
-        "colab_url": "https://{your-colab-url}"
+        "colab_url": "https://colab.research.google.com"
     },
     ...
 }
 ```
 ## Deepnote
 
 To add [Deepnote](https://deepnote.com) links to your page, add the following configuration:
```

### Comparing `tskit_book_theme-0.3.2/docs/notebooks.md` & `tskit_book_theme-1.0.1/docs/content/notebooks.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 This page demonstrates some extra functionality that works with this theme.
 
 ## Markdown + notebooks
 
 As it is markdown, you can embed images, HTML, etc into your posts!
 
-![](./images/cool.jpg)
+![](../images/cool.jpg)
 
 You an also $add_{math}$ and
 
 $$
 math^{blocks}
 $$
```

### Comparing `tskit_book_theme-0.3.2/docs/reference/comments.md` & `tskit_book_theme-1.0.1/docs/reference/comments.md`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/reference/extensions.md` & `tskit_book_theme-1.0.1/docs/reference/extensions.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,18 @@
 - Textual citation {cite:t}`project_jupyter-proc-scipy-2018`, {cite:t}`holdgraf_rapid_2016,project_jupyter-proc-scipy-2018`.
 
 And here's a bibliography:
 
 ```{bibliography}
 ```
 
-:::{seealso}
-See the [paragraph markup page](kitchen-sink/paragraph-markup.rst) for more references styling.
-:::
 
 ## `ABlog` - Blog post list
 
-[ABlog](https://ablog.readthedocs.io/en/latest/) is a Sphinx extension for blogging with Sphinx.
+[ABlog](https://ablog.readthedocs.io/) is a Sphinx extension for blogging with Sphinx.
 
 Here's a sample post list:
 
 ```{postlist}
 :date: "%Y-%m-%d"
 :format: "{date} - {title}"
 :excerpts:
```

### Comparing `tskit_book_theme-0.3.2/docs/reference/notebooks.md` & `tskit_book_theme-1.0.1/docs/reference/notebooks.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,61 +12,62 @@
   name: python3
 ---
 
 # Jupyter notebooks
 
 This is a page to demonstrate the look and feel of Jupyter Notebook elements.
 
-
 ## Hiding elements
 
-### Hiding inputs
+### Hide cells
+
+The following cell is hidden.
+It also has a `thebe-init` tag which means it will be executed when you initialize Thebe.
 
 ```{code-cell} ipython3
-:tags: [remove_cell]
+:tags: [hide-cell, thebe-init]
 
 # Generate some code that we'll use later on in the page
 import numpy as np
 import matplotlib.pyplot as plt
-
-square = np.random.randn(100, 100)
-wide = np.random.randn(100, 1000)
 ```
 
+### Hide inputs
+
 ```{code-cell} ipython3
-:tags: [hide_input]
+:tags: [hide-input]
 
 # Hide input
 square = np.random.randn(100, 100)
 wide = np.random.randn(100, 1000)
 
 fig, ax = plt.subplots()
 ax.imshow(square)
 
 fig, ax = plt.subplots()
 ax.imshow(wide)
 ```
 
-### Hiding outputs
+### Hide outputs
 
 ```{code-cell} ipython3
-:tags: [hide_output]
+:tags: [hide-output]
 
 # Hide output
 square = np.random.randn(100, 100)
 wide = np.random.randn(100, 1000)
 
 fig, ax = plt.subplots()
 ax.imshow(square)
 
 fig, ax = plt.subplots()
 ax.imshow(wide)
 ```
 
-### Hiding markdown
+### Hide markdown
 
 ````{toggle}
 ```{note}
 This is a hidden markdown cell
 
 It should be hidden!
 ```
@@ -75,33 +76,33 @@
 ```{admonition} And here's a toggleable note
 :class: dropdown
 With a body!
 ```
 
 +++
 
-### Hiding both inputs and outputs
+### Hide both inputs and outputs
 
 ```{code-cell} ipython3
-:tags: [hide_output, hide_input]
+:tags: [hide-output, hide-input]
 
 square = np.random.randn(100, 100)
 wide = np.random.randn(100, 1000)
 
 fig, ax = plt.subplots()
 ax.imshow(square)
 
 fig, ax = plt.subplots()
 ax.imshow(wide)
 ```
 
-### Hiding the whole cell
+### Hide the whole cell
 
 ```{code-cell} ipython3
-:tags: [hide_cell]
+:tags: [hide-cell]
 
 square = np.random.randn(100, 100)
 wide = np.random.randn(100, 1000)
 
 fig, ax = plt.subplots()
 ax.imshow(square)
```

### Comparing `tskit_book_theme-0.3.2/docs/reference/special-theme-elements.md` & `tskit_book_theme-1.0.1/docs/reference/special-theme-elements.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 ```{container} full-width
 
 This is some markdown that should be shown at full width.
 
 Here's the Jupyter logo:
 
-![](https://raw.githubusercontent.com/adebar/awesome-jupyter/master/logo.png)
+![](https://raw.githubusercontent.com/adebar/awesome-jupyter/master/assets/logo.png)
 
 :::{note}
 Here's a full-width admonition!
 :::
 
 ```
 
@@ -214,15 +214,15 @@
 a+b
 ```
 
 how does it look?
 
 Markdown cell with images in sidebar
 
-<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" style="max-width:200px" />
+<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-Jupyter_logo.svg.png" />
 
 ````
 +++
 
 ### More content after the margin content
 
 This is extra content after the margins to see if cells overlap and such.
```

### Comparing `tskit_book_theme-0.3.2/docs/reference/thebe.md` & `tskit_book_theme-1.0.1/docs/reference/thebe.md`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/references.bib` & `tskit_book_theme-1.0.1/docs/references.bib`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/docs/tutorials/get-started.md` & `tskit_book_theme-1.0.1/docs/tutorials/get-started.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 :::
 
 ## Install and activate the theme
 
 First install `sphinx-book-theme` with `pip`:
 
 ```
-pip install tskit-book-theme
+pip install sphinx-book-theme
 ```
 
 then, activate the theme in your Sphinx configuration (`conf.py`):
 
 ```
 ...
-html_theme = "tskit_book_theme"
+html_theme = "sphinx_book_theme"
 ...
 ```
 
 This will activate the Sphinx Book Theme for your documentation.
 
 :::{note}
 You may need to comment-out your `html_theme_options` configuration depending on your previous theme.
```

### Comparing `tskit_book_theme-0.3.2/package.json` & `tskit_book_theme-1.0.1/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'repository'": "'https://github.com/executablebooks/sphinx-book-theme'"}*

```diff
@@ -13,12 +13,12 @@
         "sass-loader": "^10.1.1",
         "style-loader": "^1.1.3",
         "webpack": "^4.41.6",
         "webpack-cli": "^3.3.11",
         "webpack-dev-server": "^3.10.3"
     },
     "name": "tskit_book_theme",
-    "repository": "https://github.com/executablebooks/tskit-book-theme",
+    "repository": "https://github.com/executablebooks/sphinx-book-theme",
     "scripts": {
         "build": "webpack"
     }
 }
```

### Comparing `tskit_book_theme-0.3.2/pyproject.toml` & `tskit_book_theme-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -12,72 +12,74 @@
 [tool.pytest.ini_options]
 testpaths = [
     "tests"
 ]
 
 [project]
 name = "tskit-book-theme"
-description = "A clean book theme for tskit ecosystem projects"
+description = "A book theme for tskit projects"
 dynamic = ["version"]
 readme = "README.md"
 
 requires-python = ">=3.7"
 dependencies = [
-  "sphinx>=3,<5",
-  "pydata-sphinx-theme~=0.8.0",
-  "pyyaml",
+  "sphinx>=4,<7",
+  "pydata-sphinx-theme>=0.13.3",
 ]
 
-
 license = { file = "LICENSE" }
 # TODO: Add email of the maintainer
 maintainers = [
-  { name = "Chris Holdgraf", email = "choldgraf@gmail.com" },
+  { name = "Ben Jeffery", email = "ben.jeffery@bdi.ox.ac.uk" },
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3",
   "Framework :: Sphinx",
   "Framework :: Sphinx :: Theme",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
 code_style = [
-    "pre-commit~=2.7.0"
+    "pre-commit"
 ]
 doc = [
-    "ablog~=0.10.13",
+    "ablog",
     "ipywidgets",
     "folium",
     "numpy",
     "matplotlib",
     "numpydoc",
-    "myst-nb~=0.13.2",
+    "myst-nb",
     "nbclient",
     "pandas",
     "plotly",
-    "sphinx~=4.0",  # Force Sphinx to be the latest version
     "sphinx-design",
     "sphinx-examples",
     "sphinx-copybutton",
-    "sphinx-tabs",
-    "sphinx-togglebutton>=0.2.1",
-    "sphinx-thebe>=0.1.1",
-    "sphinxcontrib-bibtex~=2.2",
+    "sphinx-tabs<=3.4.0", # sphinx-tabs 3.4.1 needs docutils >.17, which would conflict with our pin above
+    "docutils==0.17.1", # docutils 0.18, 0.19 need a patch fix https://sourceforge.net/p/docutils/patches/195/, un-pin when 0.20 is released
+    "sphinx-togglebutton",
+    "sphinx-thebe",
+    "sphinxcontrib-bibtex",
     "sphinxcontrib-youtube",
     "sphinxext-opengraph",
 ]
 test = [
-    "beautifulsoup4>=4.6.1,<5",
+    "beautifulsoup4",
     "coverage",
-    "myst-nb~=0.13.2",
-    "pytest~=6.0.1",
+    "myst-nb",
+    "pytest",
     "pytest-cov",
-    "pytest-regressions~=2.0.1",
-    "sphinx_thebe"
+    "pytest-regressions",
+    "sphinx_thebe",
 ]
 
 [project.entry-points]
 "sphinx.html_themes" = { tskit_book_theme = "tskit_book_theme" }
+
+[project.urls]
+Repository = "https://github.com/executablebooks/tskit-book-theme"
+Documentation = "https://tskit.dev"
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/__init__.py` & `tskit_book_theme-1.0.1/src/tskit_book_theme/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,25 +5,32 @@
 from functools import lru_cache
 
 from docutils.parsers.rst.directives.body import Sidebar
 from docutils import nodes as docutil_nodes
 from sphinx.application import Sphinx
 from sphinx.locale import get_translation
 from sphinx.util import logging
+from pydata_sphinx_theme.utils import get_theme_options_dict
 
 from .nodes import SideNoteNode
-
-# from .header_buttons import prep_header_buttons, add_header_buttons
-# from .header_buttons.launch import add_launch_buttons
+from .header_buttons import (
+   prep_header_buttons,
+   add_header_buttons,
+    update_sourcename,
+    update_context_with_repository_info,
+)
+#from .header_buttons.launch import add_launch_buttons
+from .header_buttons.source import add_source_buttons
 from ._transforms import HandleFootnoteTransform
 
-__version__ = "0.3.2"
-"""tskit-book-theme version"""
+__version__ = "1.0.1"
+"""sphinx-book-theme version"""
 
 SPHINX_LOGGER = logging.getLogger(__name__)
+DEFAULT_LOG_TYPE = "sphinxbooktheme"
 MESSAGE_CATALOG_NAME = "booktheme"
 
 
 def get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
     theme_path = parent / "theme" / "tskit_book_theme"
@@ -54,18 +61,19 @@
     # Add the author if it exists
     if app.config.author != "unknown":
         context["author"] = app.config.author
 
     # Translations
     translation = get_translation(MESSAGE_CATALOG_NAME)
     context["translate"] = translation
-    # this is set in the html_theme
-    context["theme_search_bar_text"] = translation(
-        context.get("theme_search_bar_text", "Search the docs ...")
-    )
+
+    # If search text hasn't been manually specified, use a shorter one here
+    theme_options = get_theme_options_dict(app)
+    if "search_bar_text" not in theme_options:
+        context["theme_search_bar_text"] = translation("Search") + "..."
 
 
 @lru_cache(maxsize=None)
 def _gen_hash(path: str) -> str:
     return hashlib.sha1(path.read_bytes()).hexdigest()
 
 
@@ -84,15 +92,15 @@
         # CSS assets are stored in css_files, JS assets in script_files
         asset_type = "css_files" if asset.endswith(".css") else "script_files"
         if asset_type in context:
             # Define paths to the original asset file, and its linked file in Sphinx
             asset_sphinx_link = f"_static/{asset}"
             asset_source_path = theme_static / asset
             if not asset_source_path.exists():
-                SPHINX_LOGGER.warn(
+                SPHINX_LOGGER.warning(
                     f"Asset {asset_source_path} does not exist, not linking."
                 )
             # Find this asset in context, and update it to include the digest
             if asset_sphinx_link in context[asset_type]:
                 hash = _gen_hash(asset_source_path)
                 ix = context[asset_type].index(asset_sphinx_link)
                 context[asset_type][ix] = asset_sphinx_link + "?digest=" + hash
@@ -108,18 +116,20 @@
     # will define their own CSS file, so if a sub-theme is used, this code is
     # run but the book theme CSS file won't be linked in Sphinx.
     if app.config.html_theme == "tskit_book_theme":
         assets.append("styles/tskit-book-theme.css")
     hash_assets_for_files(assets, get_html_theme_path() / "static", context)
 
 
-def update_thebe_config(app):
+def update_mode_thebe_config(app):
     """Update thebe configuration with SBT-specific values"""
-    theme_options = app.env.config.html_theme_options
+    theme_options = get_theme_options_dict(app)
     if theme_options.get("launch_buttons", {}).get("thebe") is True:
+        # In case somebody specifies they want thebe in a launch button
+        # but has not activated the sphinx_thebe extension.
         if not hasattr(app.env.config, "thebe_config"):
             SPHINX_LOGGER.warning(
                 (
                     "Thebe is activated but not added to extensions list. "
                     "Add `sphinx_thebe` to your site's extensions list."
                 )
             )
@@ -142,14 +152,27 @@
             # Explicitly check in case branch is ""
             branch = "master"
         thebe_config["repository_branch"] = branch
 
     app.env.config.thebe_config = thebe_config
 
 
+def check_deprecation_keys(app):
+    """Warns about the deprecated keys."""
+
+    deprecated_config_list = ["single_page"]
+    for key in deprecated_config_list:
+        if key in get_theme_options_dict(app):
+            SPHINX_LOGGER.warning(
+                f"'{key}' was deprecated from version 0.3.4 onwards. See the CHANGELOG for more information: https://github.com/executablebooks/sphinx-book-theme/blob/master/CHANGELOG.md"  # noqa: E501
+                f"[{DEFAULT_LOG_TYPE}]",
+                type=DEFAULT_LOG_TYPE,
+            )
+
+
 class Margin(Sidebar):
     """Goes in the margin to the right of the page."""
 
     optional_arguments = 1
     required_arguments = 0
 
     def run(self):
@@ -161,45 +184,83 @@
 
         # Remove the "title" node if it is empty
         if not self.arguments:
             nodes[0].children.pop(0)
         return nodes
 
 
+def update_general_config(app):
+    theme_dir = get_html_theme_path()
+    # Update templates for sidebar. Needed for jupyter-book builds as jb
+    # uses an instance of Sphinx class from sphinx.application to build the app.
+    # The __init__ function of which calls self.config.init_values() just
+    # before emitting `config-inited` event. The init_values function overwrites
+    # templates_path variable.
+    app.config.templates_path.append(os.path.join(theme_dir, "components"))
+
+
+def update_templates(app, pagename, templatename, context, doctree):
+    """Update template names and assets for page build.
+
+    This is a copy of what the pydata theme does here to include a new section
+    - https://github.com/pydata/pydata-sphinx-theme/blob/0a4894fab49befc59eb497811949a1d0ede626eb/src/pydata_sphinx_theme/__init__.py#L173 # noqa: E501
+    """
+    # Allow for more flexibility in template names
+    template_sections = ["theme_footer_content_items"]
+    for section in template_sections:
+        if context.get(section):
+            # Break apart `,` separated strings so we can use , in the defaults
+            if isinstance(context.get(section), str):
+                context[section] = [
+                    ii.strip() for ii in context.get(section).split(",")
+                ]
+
+            # Add `.html` to templates with no suffix
+            for ii, template in enumerate(context.get(section)):
+                if not os.path.splitext(template)[1]:
+                    context[section][ii] = template + ".html"
+
+
 def setup(app: Sphinx):
     # Register theme
     theme_dir = get_html_theme_path()
     app.add_html_theme("tskit_book_theme", theme_dir)
     app.add_js_file("scripts/tskit-book-theme.js")
 
     # Translations
     locale_dir = os.path.join(theme_dir, "static", "locales")
     app.add_message_catalog(MESSAGE_CATALOG_NAME, locale_dir)
 
     # Events
-    app.connect("builder-inited", update_thebe_config)
+    app.connect("builder-inited", update_mode_thebe_config)
+    app.connect("builder-inited", check_deprecation_keys)
+    app.connect("builder-inited", update_sourcename)
+    app.connect("builder-inited", update_context_with_repository_info)
+    app.connect("builder-inited", update_general_config)
     app.connect("html-page-context", add_metadata_to_page)
     app.connect("html-page-context", hash_html_assets)
+    app.connect("html-page-context", update_templates)
 
     # Nodes
     SideNoteNode.add_node(app)
 
     # Header buttons
-    # Commented out as this created duplicate buttons
-    #     app.connect("html-page-context", prep_header_buttons)
-    #     app.connect("html-page-context", add_launch_buttons)
-    # Bump priority by 1 so that it runs after the pydata theme sets up the edit URL.
-    #     app.connect("html-page-context", add_header_buttons, priority=501)
+    app.connect("html-page-context", prep_header_buttons)
+    # Bump priority so that it runs after the pydata theme sets up the edit URL func.
+#     app.connect("html-page-context", add_launch_buttons, priority=501)
+    app.connect("html-page-context", add_source_buttons, priority=501)
+#     app.connect("html-page-context", add_header_buttons, priority=501)
 
     # Directives
-    app.add_directive("margin", Margin, override=True)
+    #app.add_directive("margin", Margin)
 
     # Post-transforms
     app.add_post_transform(HandleFootnoteTransform)
 
-    # Update templates for sidebar
+    # Update templates for sidebar, for builds where config-inited is not called
+    # (does not work in case of jupyter-book)
     app.config.templates_path.append(os.path.join(theme_dir, "components"))
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/_compile_translations.py` & `tskit_book_theme-1.0.1/src/tskit_book_theme/_compile_translations.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             )
             if not out_path.parent.exists():
                 out_path.parent.mkdir(parents=True)
             if not out_path.exists():
                 header = f"""
 msgid ""
 msgstr ""
-"Project-Id-Version: Tskit-Book-Theme\\n"
+"Project-Id-Version: Sphinx-Book-Theme\\n"
 "MIME-Version: 1.0\\n"
 "Content-Type: text/plain; charset=UTF-8\\n"
 "Content-Transfer-Encoding: 8bit\\n"
 "Language: {language}\\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\\n"
 """
                 out_path.write_text(header)
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/_transforms.py` & `tskit_book_theme-1.0.1/src/tskit_book_theme/_transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from sphinx.transforms.post_transforms import SphinxPostTransform
 from typing import Any
 from docutils import nodes as docutil_nodes
 from sphinx import addnodes as sphinx_nodes
+from pydata_sphinx_theme.utils import get_theme_options_dict
 from .nodes import SideNoteNode
-import copy
 
 
 class HandleFootnoteTransform(SphinxPostTransform):
     """Transform footnotes into side/marginnotes."""
 
     default_priority = 1
     formats = ("html",)
 
     def run(self, **kwargs: Any) -> None:
-        theme_options = self.env.config.html_theme_options
+        theme_options = get_theme_options_dict(self.app)
         if theme_options.get("use_sidenotes", False) is False:
             return None
         # Cycle through footnote references, and move their content next to the
         # reference. This lets us display the reference in the margin,
         # or just below on narrow screens.
         for ref_node in self.document.traverse(docutil_nodes.footnote_reference):
             parent = None
@@ -27,44 +27,48 @@
                 if (
                     len(foot_node.attributes["backrefs"])
                     and foot_node.attributes["backrefs"][0]
                     == ref_node.attributes["ids"][0]
                 ):
                     parent = foot_node.parent
                     # second children of footnote node is the content text
-                    text = foot_node.children[1].astext()
+                    foot_node_content = foot_node.children[1].children
 
                     sidenote = SideNoteNode()
                     para = docutil_nodes.inline()
                     # first children of footnote node is the label
                     label = foot_node.children[0].astext()
 
-                    if text.startswith("{-}"):
+                    if foot_node_content[0].astext().startswith("{-}"):
                         # marginnotes will have content starting with {-}
                         # remove the number so it doesn't show
                         para.attributes["classes"].append("marginnote")
-                        para.append(docutil_nodes.Text(text.replace("{-}", "")))
+                        foot_node_content[0] = docutil_nodes.Text(
+                            foot_node_content[0].replace("{-}", "")
+                        )
+                        para.children = foot_node_content
 
                         sidenote.attributes["names"].append(f"marginnote-role-{label}")
                     else:
                         # sidenotes are the default behavior if no {-}
                         # in this case we keep the number
                         superscript = docutil_nodes.superscript("", label)
                         para.attributes["classes"].append("sidenote")
-                        para.extend([superscript, docutil_nodes.Text(text)])
+                        parachildren = [superscript] + foot_node_content
+                        para.children = parachildren
 
                         sidenote.attributes["names"].append(f"sidenote-role-{label}")
                         sidenote.append(superscript)
 
                     # If the reference is nested (e.g. in an admonition), duplicate
                     # the content node And place it just before the parent container,
                     # so it works w/ margin. Only show one or another depending on
                     # screen width.
                     node_parent = ref_node.parent
-                    para_dup = copy.deepcopy(para)
+                    para_dup = para.deepcopy()
                     # looping to check parent node
                     while not isinstance(
                         node_parent, (docutil_nodes.section, sphinx_nodes.document)
                     ):
                         # if parent node is another container
                         if not isinstance(
                             node_parent,
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/scripts/index.js` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/scripts/index.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -46,46 +46,14 @@
         } else if (document.webkitExitFullscreen) {
             document.webkitExitFullscreen();
         }
     }
 };
 
 /**
- * Sidebar scroll on load.
- *
- * Detect the active page in the sidebar, and scroll so that it is centered on
- * the screen.
- */
-var scrollToActive = () => {
-    var navbar = document.getElementById("site-navigation");
-    var active_pages = navbar.querySelectorAll(".active");
-    var active_page = active_pages[active_pages.length - 1];
-    // Only scroll the navbar if the active link is lower than 50% of the page
-    if (
-        active_page !== undefined &&
-        active_page.offsetTop > $(window).height() * 0.5
-    ) {
-        navbar.scrollTop = active_page.offsetTop - $(window).height() * 0.2;
-    }
-};
-
-/**
- * Called when the "print to PDF" button is clicked.
- * This is a hack to prevent tooltips from showing up in the printed PDF.
- */
-var printPdf = (el) => {
-    // Detach the tooltip text from DOM to hide in PDF
-    // and then reattach it for HTML
-    let tooltipID = $(el).attr("aria-describedby");
-    let tooltipTextDiv = $("#" + tooltipID).detach();
-    window.print();
-    $("body").append(tooltipTextDiv);
-};
-
-/**
  * Manage scrolling behavior. This is primarily two things:
  *
  * 1. Hide the Table of Contents any time sidebar content is on the screen.
  *
  * This will be triggered any time a sidebar item enters or exits the screen.
  * It adds/removes items from an array if they have entered the screen, and
  * removes them when they exit the screen. It hides the TOC if anything is
@@ -112,30 +80,36 @@
                     }
                 }
             }
         });
 
         // Hide the TOC if any margin content is displayed on the screen
         if (onScreenItems.length > 0) {
-            $("div.bd-toc").removeClass("show");
+            document.querySelector("div.bd-sidebar-secondary").classList.add("hide");
         } else {
-            $("div.bd-toc").addClass("show");
+            document
+                .querySelector("div.bd-sidebar-secondary")
+                .classList.remove("hide");
         }
     };
     let manageScrolledClassOnBody = (entries, observer) => {
         // The pixel is at the top, so if we're < 0 that it means we've scrolled
         if (entries[0].boundingClientRect.y < 0) {
             document.body.classList.add("scrolled");
         } else {
             document.body.classList.remove("scrolled");
         }
     };
 
     // Set up the intersection observer to watch all margin content
-    let tocObserver = new IntersectionObserver(hideTocCallback);
+    let options = {
+        // Trigger callback when the top of a margin item is 1/3 up the screen
+        rootMargin: "0px 0px -33% 0px",
+    };
+    let tocObserver = new IntersectionObserver(hideTocCallback, options);
     // TODO: deprecate popout after v0.5.0
     const selectorClasses = [
         "marginnote",
         "sidenote",
         "margin",
         "margin-caption",
         "full-width",
@@ -147,15 +121,15 @@
         // Use three permutations of each class name because `tag_` and `_` used to be supported
         marginSelector.push(
             ...[
                 `.${ii}`,
                 `.tag_${ii}`,
                 `.${ii.replace("-", "_")}`,
                 `.tag_${ii.replace("-", "_")}`,
-            ]
+            ],
         );
     });
     document.querySelectorAll(marginSelector.join(", ")).forEach((ii) => {
         tocObserver.observe(ii);
     });
 
     // Set up the observer to check if we've scrolled from top of page
@@ -163,71 +137,52 @@
     scrollObserver.observe(document.querySelector(".sbt-scroll-pixel-helper"));
 };
 
 /**
  * Activate Thebe with a custom button click.
  */
 var initThebeSBT = () => {
-    var title = $("div.section h1")[0];
-    if (!$(title).next().hasClass("thebe-launch-button")) {
-        $("<button class='thebe-launch-button'></button>").insertAfter($(title));
+    var title = document.querySelector("section h1");
+    var sibling = title.nextElementSibling;
+    // If the next element after the title isn't a thebe button, add one now.
+    // That way it is initiatlized when thebe is first-clicked and isn't re-added after.
+    if (!sibling.classList.contains("thebe-launch-button")) {
+        title.insertAdjacentHTML(
+            "afterend",
+            "<button class='thebe-launch-button'></button>",
+        );
     }
+    // This function is provided by sphinx-thebe
     initThebe();
 };
 
 /**
- * Use Bootstrap helper function to enable tooltips.
+ * Add no print class to certain DOM elements
  */
-var initTooltips = () => {
-    $(document).ready(function() {
-        $('[data-toggle="tooltip"]').tooltip({
-            trigger: "hover",
-            delay: {
-                show: 500,
-                hide: 100
-            },
-        });
-    });
-};
-
-/**
- * MutationObserver to move the ReadTheDocs button
- */
-function initRTDObserver() {
-    const mutatedCallback = (mutationList, observer) => {
-        mutationList.forEach((mutation) => {
-            // Check whether the mutation is for RTD, which will have a specific structure
-            if (mutation.addedNodes.length === 0) {
-                return;
-            }
-            if (mutation.addedNodes[0].data === undefined) {
-                return;
-            }
-            if (mutation.addedNodes[0].data.search("Inserted RTD Footer") != -1) {
-                mutation.addedNodes.forEach((node) => {
-                    document.getElementById("rtd-footer-container").append(node);
-                });
-            }
-        });
-    };
 
-    const observer = new MutationObserver(mutatedCallback);
-    const config = {
-        childList: true
-    };
-    observer.observe(document.body, config);
+function addNoPrint() {
+    var noPrintSelector = [
+        ".bd-header-announcement",
+        ".bd-header",
+        ".bd-header-article",
+        ".bd-sidebar-primary",
+        ".bd-sidebar-secondary",
+        ".bd-footer-article",
+        ".bd-footer-content",
+        ".bd-footer",
+    ].join(",");
+    document.querySelectorAll(noPrintSelector).forEach((ii) => {
+        ii.classList.add("noprint");
+    });
 }
 
 /**
  * Set up callback functions for UI click actions
  */
 window.initThebeSBT = initThebeSBT;
-window.printPdf = printPdf;
 window.toggleFullScreen = toggleFullScreen;
 
 /**
  * Set up functions to load when the DOM is ready
  */
-sbRunWhenDOMLoaded(initTooltips);
-sbRunWhenDOMLoaded(scrollToActive);
 sbRunWhenDOMLoaded(initTocHide);
-sbRunWhenDOMLoaded(initRTDObserver);
+sbRunWhenDOMLoaded(addNoPrint);
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/content/_images.scss` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/content/_images.scss`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/index.scss` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/index.scss`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,46 @@
-/*! tskit-book-theme CSS
+/*! sphinx-book-theme CSS
  * BSD 3-Clause License
  * Copyright (c) 2020, EBP
  * All rights reserved.
  *
  * This follows the 7-1 pattern described here:
  * https://sass-guidelin.es/#architecture
  */
 // Variables and re-usable SCSS functions
 @import "abstracts/mixins";
 @import "abstracts/variables";
 
 // Basic styling applied throughout site
 @import "base/base";
-@import "base/bootstrap";
 @import "base/typography";
 @import "base/print";
 
 // Major theme layout, skeleton, and whitespace
+@import "sections/announcement";
 @import "sections/article";
-@import "sections/footer-article";
-@import "sections/footer-content";
+@import "sections/article-container";
 @import "sections/header-article";
-@import "sections/headers";
+@import "sections/header-primary";
 @import "sections/sidebar-primary";
 @import "sections/sidebar-secondary";
-@import "sections/sidebars-toggle";
+@import "sections/footer-content";
+@import "sections/footer-article";
 
 // Re-usable components across the theme
-@import "components/buttons";
-@import "components/search.scss";
+@import "components/icon-links";
+@import "components/logo";
+@import "components/search";
 
 // Content blocks in standard Sphinx
-@import "content/admonitions";
-@import "content/code";
-@import "content/field-lists";
-@import "content/footnotes";
-@import "content/glossary";
 @import "content/images";
 @import "content/margin";
-@import "content/math";
 @import "content/quotes";
-@import "content/sidebar";
-@import "content/tableofcontents";
+@import "content/code";
+@import "content/notebooks";
 
 // Content blocks from Sphinx extensions
-@import "extensions/ablog";
+
 @import "extensions/comments";
-@import "extensions/myst-nb";
-@import "extensions/sphinx-tabs";
-@import "extensions/readthedocs";
 @import "extensions/thebe";
 
-// Page-specific CSS
-@import "pages/search";
-
-//tskit specific theming
-@import "tskit/tskit";
+@import "tskit/tskit";
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/sections/_sidebar-primary.scss` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/sections/_sidebar-secondary.scss`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,94 @@
 /*********************************************
-* Left Nav Bar *
+* Table of Contents (right nav bar)          *
 *********************************************/
-#site-navigation {
-  padding-top: 0;
-  width: $leftbar-width-wide;
-  font-size: var(--sbt-sidebar-font-size);
-  top: 0px !important;
-  background: white;
-  border-right: $border-thin;
-  transition: margin-left $animation-time ease 0s,
-    opacity $animation-time ease 0s, visibility $animation-time ease 0s;
-  overflow-y: unset; // To over-ride the pydata theme and allow for sticky items
-  @include fill-vertical-screen-space();
-
-  // On mobile, behave like a slide-out drawer
-  @media (max-width: $breakpoint-md) {
-    position: fixed;
-    width: $leftbar-width-mobile;
-    max-width: 300px;
-    font-size: 1.2em;
-    z-index: $zindex-offcanvas;
-  }
-
-  // The container for the sidebar content (stuff that isn't the RTD button)
-  .bd-sidebar__content {
-    overflow-y: auto;
-    flex-grow: 1;
-    display: flex;
-    flex-direction: column;
-    @include scrollbar-style();
-    @include scrollbar-on-hover();
-  }
-
-  // Apply some basic padding so the dropdown buttons don't overlap w/ scrollbar
-  .bd-sidebar__top,
-  .bd-sidebar__bottom {
-    padding: 0 1rem 0rem 1.5rem;
-  }
 
-  // This should always snap to the bottom even if there's no sidebar content
-  .bd-sidebar__bottom {
-    margin-top: auto;
-    margin-bottom: 2em;
+.bd-sidebar-secondary {
+  // So that it sticks to the top of the page instead of the header height
+  top: 0;
+
+  @media (max-width: $breakpoint-lg) {
+    // So that tooltips don't overlap
+    z-index: $zindex-tooltip + 1;
   }
 
-  nav ul.nav {
-    // Sidebar link color
-    li a,
-    ul li a {
-      color: $non-content-grey;
-    }
-    a:hover,
-    li.active > a,
-    li.active > a:hover {
-      color: rgba(var(--pst-color-link), 1);
-    }
+  // So that we can center the TOC button with the article header buttons
+  .sidebar-secondary-items {
+    padding: 0;
+    display: flex;
+    gap: 0.5rem;
 
-    // Adjust padding to be a bit tighter
-    ul {
-      padding-left: 1rem;
+    // Remove the manual padding since we'll use `gap`
+    .sidebar-secondary-item {
+      padding-top: 0;
+      padding-bottom: 0;
     }
   }
 
-  h1.site-logo {
-    margin: 0.5em 0 0 0;
-    font-size: 1.1em;
-    color: black;
-    text-align: center;
-  }
+  // The 'on this page' title div should take up the full header
+  .onthispage {
+    height: $header-article-height;
+    min-height: $header-article-height;
+    display: flex;
+    align-items: center;
+    margin: 0;
+    color: var(--pst-color-muted);
+  }
+
+  // Wide screen behavior
+  @media (min-width: $breakpoint-lg) {
+    background: var(--pst-color-background);
+    height: fit-content;
+    transition: max-height 0.4s ease;
+
+    // To make sure it shows above the page content
+    z-index: $zindex-middle;
+
+    // Remove padding so that it's flush on the top and left
+    padding: 0;
+
+    // This is the container div for the secondary sidebar nav
+    .toc-item {
+      // Border is a bit less prominent
+      border-left-color: var(--pst-color-surface);
+      // Flush with the top so that we can fix the height of the toc header div
+      padding-top: 0;
+
+      // The table of contents <ul> after the title div
+      nav.page-toc {
+        // Remove extra margin the PST adds for other sidebar items
+        margin-bottom: 0;
 
-  div.navbar_extra_footer {
-    text-align: center;
-    font-size: 0.9em;
-    color: $non-content-grey;
-    margin-bottom: 3em;
-  }
+        // Items after "on this page' should fade in and out
+        transition: opacity 0.4s ease;
+      }
+    }
 
-  // Single page
-  &.single-page {
-    border-right: 0;
-  }
-}
+    // Rules for when sidebar is hidden
+    // the `not:hover` means that hovering over the sidebar will show it again.
+    &.hide:not(:hover) {
+      // Cap the height, and remove the scrollbar
+      max-height: $header-article-height;
+      overflow-y: hidden;
+
+      // Shadow matches what we have in the article header
+      .scrolled & {
+        box-shadow: 0 6px 6px -6px rgba(0, 0, 0, 0.3);
+      }
 
-div.navbar-brand-box {
-  @media (min-width: $breakpoint-md) {
-    padding-top: 2em;
-  }
+      // Show a down carot
+      .onthispage:after {
+        opacity: 1;
+        content: "\f107";
+        font-family: "Font Awesome 5 Free";
+        font-weight: 900;
+        padding-left: 0.5em;
+        transition: opacity 0.3s ease;
+      }
 
-  a.navbar-brand {
-    width: 100%;
-    height: auto;
-    flex-direction: column;
-
-    img {
-      display: block;
-      height: auto;
-      width: auto;
-      max-height: 10vh;
-      max-width: 100%;
-      margin: 0 auto;
-      @media (min-width: $breakpoint-md) {
-        max-height: 15vh !important;
+      // The page-toc list is hidden
+      nav.page-toc {
+        opacity: 0;
       }
     }
   }
 }
-
-nav.bd-links {
-  margin-left: 0px; // Because the PST adds margin by default
-  p.caption,
-  .toctree-l1 a {
-    padding-left: 0em;
-  }
-  // Overriding PyData Theme Defaults so the navigation is always visible
-  overflow-y: visible;
-  max-height: none;
-}
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/tskit/_palette.scss` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/tskit/_palette.scss`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-//
-// Speak to your designer to get the initial colour palette for the project!!!
-//
-// Please do not name your colour variables with the colour they contain. If you do, you will end up with:
-// $red: blue;
-
 $brand-color-1: #1eebb1;
 $brand-color-2: #14e2a8;
 $brand-color-3: #0fa88e;
 $brand-color-4: #0d8b81;
 $brand-color-5: #0a6e74;
 $brand-color-6: #085167;
 $brand-color-7: #053e4e;
@@ -24,8 +18,8 @@
 $color-7: #01232e;
 $color-8: #1c687e;
 $color-9: #80979e;
 $color-10: rgba(29, 29, 27, 0.4);
 $color-11: rgba(255, 255, 255, 0.7);
 
 $box-shadow-1: 0 1.25rem 2.25rem $color-3;
-$box-shadow-2: 0 6px 6px $color-4;
+$box-shadow-2: 0 6px 6px $color-4;
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/styles/tskit/_tskit.scss` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/styles/tskit/_tskit.scss`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 @import "../tskit/palette";
 
-/* TYPOGRAPHY */
-
 $font-family-sans-serif: rothwood, serif;
 $font-family-sans-serif-2: sofia-pro, sans-serif;
 
 @media screen {
   ::-moz-selection {
     background-color: $brand-color-1;
     color: $color-1;
@@ -20,118 +18,93 @@
     font-size: 100%; // 16px
     -webkit-font-smoothing: antialiased;
     -moz-osx-font-smoothing: grayscale;
   }
 
   body {
     font-family: $font-family-sans-serif-2;
-  }
-
-  /* TYPOGRAPHY COLOURS*/
-
-  .main-content {
+    background-color: $brand-color-7;
     color: $color-1;
   }
 
   p {
     color: inherit;
   }
-
-  .content-container a,
-  .content-container a:visited {
-    color: $brand-color-2;
-  }
-
-  .content-container h1,
-  .content-container h2,
-  .content-container h3,
-  .content-container h4,
-  .content-container h5 {
-    color: $brand-color-2;
+  p.caption
+  {
+    color: inherit !important;
   }
 
-  /* DESIGN */
 
-  body {
-    background-color: $brand-color-7;
-    color: $color-1;
-  }
-
-  #site-navigation {
+  .bd-header-article{
+    border-color: $brand-color-2;
+    background-color: $brand-color-2;
     box-shadow: $box-shadow-2;
   }
 
-  nav.bd-links p.caption,
-  #site-navigation nav ul.nav li a,
-  #site-navigation nav ul.nav ul li a {
-    color: $brand-color-6;
-  }
-  #site-navigation nav ul.nav a:hover,
-  #site-navigation nav ul.nav li.active > a,
-  #site-navigation nav ul.nav li.active > a:hover {
-    color: $brand-color-8;
+  .bd-sidebar span.caption-text {
+    color: #323232;
   }
 
-  .sticky-top {
-    .tocsection {
-      border-color: $brand-color-2;
-    }
-
-    .bd-toc {
-      box-shadow: $box-shadow-2;
-      background-color: $brand-color-2;
-
-      nav {
-        background-color: $brand-color-2;
-      }
-    }
-
-    .bd-toc nav > .nav {
-      border-color: $brand-color-2;
-    }
-
-    box-shadow: $box-shadow-2;
+  .bd-toc {
+    border-color: $brand-color-2;
     background-color: $brand-color-2;
-
-    .headerbtn {
-      background-color: transparent;
-    }
+    box-shadow: $box-shadow-2;
   }
 
   .bd-toc nav li.active > a.active {
     border-left: $brand-color-8;
   }
 
   .bd-toc nav a:hover,
   .bd-toc nav li.active > a.active {
     color: $brand-color-8;
   }
 
   .bd-toc .toc-entry a,
+  .bd-toc .toc-entry a:visited,
   .bd-toc div.onthispage {
     color: $brand-color-6;
   }
 
+  .bd-toc-item a:visited{
+    color: #646464 !important;
+  }
+
+  .navbar-nav li a:focus, .navbar-nav li a:hover, .navbar-nav li.current>a {
+    color: $brand-color-3 !important;
+  }
+
+  .sidebar-secondary-item {
+    border-color: $brand-color-2;
+    background-color: $brand-color-2;
+  }
+
   .sd-fs-3,
   .sd-fs-3 > p {
     color: $brand-color-2;
   }
 
-  span.highlighted {
-    background-color: transparentize($brand-color-2, 0.6);
+  .bd-container a,
+  .bd-container a:visited {
+    color: $brand-color-2;
   }
 
-  code,
-  .sig-name {
-    color: $color-11;
+  .bd-container h1,
+  .bd-container h2,
+  .bd-container h3,
+  .bd-container h4,
+  .bd-container h5,
+  .bd-container h6 {
+    color: $brand-color-2;
   }
 
   .admonition,
   div.admonition {
-    box-shadow: $box-shadow-1;
+    box-shadow: $box-shadow-1 !important;
     background-color: $brand-color-8;
   }
 
   .admonition.seealso {
     border-color: $brand-color-2;
 
     .admonition-title {
@@ -140,62 +113,62 @@
 
     .admonition-title:before {
       color: $brand-color-2;
     }
   }
 
   .admonition.note,
-  div.admonition.note {
+  div.admonition.note,
+  {
     border-color: $brand-color-4;
 
     .admonition-title {
       background-color: transparentize($brand-color-4, 0.9);
     }
 
     .admonition-title:before {
       color: $brand-color-4;
     }
   }
 
-  .table {
-    color: inherit;
+  div.deprecated, div.versionadded, div.versionchanged {
+    background-color: transparentize($brand-color-4, 0.9);
+    box-shadow: $box-shadow-1 !important;
   }
 
-  pre,
-  div.contents,
-  div.topic {
-    background-color: $brand-color-8;
-    border-radius: 5px;
+  code.literal {
+    background-color: inherit;
     border: inherit;
-    box-shadow: $box-shadow-1;
-    color: $color-1;
   }
 
-  blockquote {
-    color: $color-1;
+  .highlight {
+    background: inherit !important;
   }
 
-  blockquote div > p + p.attribution,
-  caption {
+  blockquote p{
+    color: white !important;
+  }
+
+  code,
+  .sig-name {
     color: $color-11;
   }
 
-  div.header-article-main .header-article__left a,
-  div.header-article-main .header-article__left button,
-  div.header-article-main .header-article__left label,
-  div.header-article-main .header-article__right a,
-  div.header-article-main .header-article__right button,
-  div.header-article-main .header-article__right label {
-    color: $brand-color-6;
+  aside.sidebar {
+    box-shadow: $box-shadow-1;
+    background-color: $brand-color-8;
   }
 
-  span.guilabel {
-    color: $brand-color-8;
+  .table {
+    color: inherit;
   }
 
+  figure figcaption{
+    color: white;
+  }
   //Notebook stuff, here be dragons
   pre,
   div.contents,
   div.topic,
   div.cell {
     background-color: $brand-color-8;
     border-radius: 5px;
@@ -280,8 +253,20 @@
   .sig.cpp .sc {
     color: $color-11 !important;
   }
 
   .prev-next-area a p.prev-next-title {
     color: inherit !important;
   }
-}
+
+  .viewcode-block:target {
+    background-color: #1a4e56 !important;
+  }
+
+  //Horrible hack, I'm sorry
+  .theme-switch-button {
+    display: none;
+  }
+
+
+
+}
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/README.md` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 ## Structure of translation files
 
 ### Translation source files
 
 The source files for our translations are hand-edited, and contain the raw mapping of words onto various languages.
 They are checked in to `git` history with this repository.
 
-`src/tskit_book_theme/assets/translations/jsons` contains a collection of JSON files that define the translation for various phrases in this repository.
+`src/sphinx_book_theme/assets/translations/jsons` contains a collection of JSON files that define the translation for various phrases in this repository.
 Each file is a different phrase, and its contents define language codes and translated phrases for each language we support.
 They were originally created with [the smodin.io language translator](https://smodin.me/translate-one-text-into-multiple-languages) (see below for how to update them).
 
 ### Compiled translation files
 
 The translation source files are compiled at build time (when we run `stb compile`) automatically.
-This is executed by the Python script at `python src/tskit_book_theme/_compile_translations.py` (more information on that below).
+This is executed by the Python script at `python src/sphinx_book_theme/_compile_translations.py` (more information on that below).
 
 These compiled files are **not checked into `.git` history**, but they **are** bundled with the theme when it is distributed in a package.
 Here's a brief explanation of each:
 
-- `src/tskit_book_theme/theme/tskit_book_theme/static/locales` contains Sphinx locale files that were auto-converted from the files in `jsons/` by the helper script below.
-- `src/tskit_book_theme/_compile_translations.py` is a helper script to auto-generate Sphinx locale files from the JSONs in `jsons/`.
+- `src/sphinx_book_theme/theme/sphinx_book_theme/static/locales` contains Sphinx locale files that were auto-converted from the files in `jsons/` by the helper script below.
+- `src/sphinx_book_theme/_compile_translations.py` is a helper script to auto-generate Sphinx locale files from the JSONs in `jsons/`.
 
 ## Workflow of translations
 
 Here's a short workflow of how to add a new translation, assuming that you are translating using the [smodin.io service](https://smodin.io/translate-one-text-into-multiple-languages).
 
 1. Go to [the smodin.io service](https://smodin.io/translate-one-text-into-multiple-languages)
 2. Select as many languages as you like.
@@ -35,19 +35,19 @@
 4. Click `TRANSLATE` and then `Download JSON`.
 5. This will download a JSON file with a bunch of `language-code: translated-phrase` mappings.
 6. Put this JSON in the `jsons/` folder, and rename it to be the phrase you've translated in English.
    So if the original phrase is `My phrase`, you should name the file `My phrase.json`.
 7. Run [the `prettier` formatter](https://prettier.io/) on this JSON to split it into multiple lines (this makes it easier to read and edit if translations should be updated)
 
    ```bash
-   prettier tskit_book_theme/translations/jsons/<message name>.json
+   prettier sphinx_book_theme/translations/jsons/<message name>.json
    ```
 
-8. Run `python src/tskit_book_theme/_compile_translations.py`
+8. Run `python src/sphinx_book_theme/_compile_translations.py`
 9. This will generate the locale files (`.mo`) that Sphinx uses in its translation machinery, and put them in `locales/<language-code>/LC_MESSAGES/<msg>.mo`.
 
 Sphinx should now know how to translate this message!
 
 ## To update a translation
 
 To update a translation, you may go to the phase you'd like to modify in `jsons/`, then find the entry for the language you'd like to update, and change its value.
-Finally, run `python src/tskit_book_theme/_compile_translations.py` and this will update the `.mo` files.
+Finally, run `python src/sphinx_book_theme/_compile_translations.py` and this will update the `.mo` files.
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/By the.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/By the.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {'3': "{'text': '作者：'}", '31': "{'text': 'Av den'}", '4': "{'text': '作者：'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u041f\u043e"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u7531"
+        "text": "\u4f5c\u8005\uff1a"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u7531"
+        "text": "\u4f5c\u8005\uff1a"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Od strane"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Por el"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "Vid"
+        "text": "Av den"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u0411\u043e"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/By.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/By.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {'17': "{'text': 'Av'}", '24': "{'text': '作者：'}", '26': "{'text': '作者：'}"}*

```diff
@@ -83,15 +83,15 @@
         "language": "Thai",
         "symbol": "th",
         "text": "\u0e42\u0e14\u0e22"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "F\u00f6rbi"
+        "text": "Av"
     },
     {
         "language": "Serbian",
         "symbol": "sr",
         "text": "\u041e\u0434 \u0441\u0442\u0440\u0430\u043d\u0435"
     },
     {
@@ -118,25 +118,25 @@
         "language": "Danish",
         "symbol": "da",
         "text": "Ved"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u901a\u8fc7"
+        "text": "\u4f5c\u8005\uff1a"
     },
     {
         "language": "Bengali",
         "symbol": "bn",
         "text": "\u09a6\u09cd\u09ac\u09be\u09b0\u09be"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u901a\u904e"
+        "text": "\u4f5c\u8005\uff1a"
     },
     {
         "language": "Finnish",
         "symbol": "fi",
         "text": "Tekij\u00e4"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Contents.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/repository.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333329%*

 * *Differences: {'0': "{'text': 'repository'}",*

 * * '1': "{'text': 'مخزن'}",*

 * * '10': "{'text': 'hoidla'}",*

 * * '11': "{'text': 'arkisto'}",*

 * * '12': "{'text': 'dépôt'}",*

 * * '13': "{'text': 'Repository'}",*

 * * '14': "{'text': 'αποθήκη'}",*

 * * '15': "{'text': 'מאגר'}",*

 * * '16': "{'text': 'gudang'}",*

 * * '17': "{'text': 'repository'}",*

 * * '18': "{'text': 'リポジトリ'}",*

 * * '19': "{'text': '저장소'}",*

 * * '2': "{'text': 'хранилище'}",*

 * * '20': "{'text': 'krātuve'}",*

 * * '21': "{'text': 'saugykla'}",*

 * * '22': "{'text': 'oppbevaringssted'}",*

 * * '23': "{'text': 'magazyn'}",*

 * * […]*

```diff
@@ -1,187 +1,187 @@
 [
     {
         "language": "English",
         "symbol": "en",
-        "text": "Contents"
+        "text": "repository"
     },
     {
         "language": "Arabic",
         "symbol": "ar",
-        "text": "\u0645\u062d\u062a\u0648\u064a\u0627\u062a"
+        "text": "\u0645\u062e\u0632\u0646"
     },
     {
         "language": "Bulgarian",
         "symbol": "bg",
-        "text": "\u0421\u044a\u0434\u044a\u0440\u0436\u0430\u043d\u0438\u0435"
+        "text": "\u0445\u0440\u0430\u043d\u0438\u043b\u0438\u0449\u0435"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u5185\u5bb9"
+        "text": "\u4ed3\u5e93"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u5167\u5bb9"
+        "text": "\u5132\u5b58\u5eab"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
-        "text": "Sadr\u017eaj"
+        "text": "spremi\u0161te"
     },
     {
         "language": "Czech",
         "symbol": "cs",
-        "text": "Obsah"
+        "text": "\u00falo\u017ei\u0161t\u011b"
     },
     {
         "language": "Danish",
         "symbol": "da",
-        "text": "Indhold"
+        "text": "lager"
     },
     {
         "language": "Dutch",
         "symbol": "nl",
-        "text": "Inhoud"
+        "text": "repository"
     },
     {
         "language": "Esperanto",
         "symbol": "eo",
-        "text": "Enhavo"
+        "text": "deponejo"
     },
     {
         "language": "Estonian",
         "symbol": "et",
-        "text": "Sisu"
+        "text": "hoidla"
     },
     {
         "language": "Finnish",
         "symbol": "fi",
-        "text": "Sis\u00e4llys"
+        "text": "arkisto"
     },
     {
         "language": "French",
         "symbol": "fr",
-        "text": "Contenu"
+        "text": "d\u00e9p\u00f4t"
     },
     {
         "language": "German",
         "symbol": "de",
-        "text": "Inhalt"
+        "text": "Repository"
     },
     {
         "language": "Greek",
         "symbol": "el",
-        "text": "\u03a0\u03b5\u03c1\u03b9\u03b5\u03c7\u03cc\u03bc\u03b5\u03bd\u03b1"
+        "text": "\u03b1\u03c0\u03bf\u03b8\u03ae\u03ba\u03b7"
     },
     {
         "language": "Hebrew",
         "symbol": "iw",
-        "text": "\u05ea\u05d5\u05db\u05df"
+        "text": "\u05de\u05d0\u05d2\u05e8"
     },
     {
         "language": "Indonesian",
         "symbol": "id",
-        "text": "Isi"
+        "text": "gudang"
     },
     {
         "language": "Italian",
         "symbol": "it",
-        "text": "Contenuti"
+        "text": "repository"
     },
     {
         "language": "Japanese",
         "symbol": "ja",
-        "text": "\u76ee\u6b21"
+        "text": "\u30ea\u30dd\u30b8\u30c8\u30ea"
     },
     {
         "language": "Korean",
         "symbol": "ko",
-        "text": "\ub0b4\uc6a9"
+        "text": "\uc800\uc7a5\uc18c"
     },
     {
         "language": "Latvian",
         "symbol": "lv",
-        "text": "Saturs"
+        "text": "kr\u0101tuve"
     },
     {
         "language": "Lithuanian",
         "symbol": "lt",
-        "text": "Turinys"
+        "text": "saugykla"
     },
     {
         "language": "Norwegian",
         "symbol": "no",
-        "text": "Innhold"
+        "text": "oppbevaringssted"
     },
     {
         "language": "Polish",
         "symbol": "pl",
-        "text": "Zawarto\u015b\u0107"
+        "text": "magazyn"
     },
     {
         "language": "Portuguese",
         "symbol": "pt",
-        "text": "Conte\u00fado"
+        "text": "reposit\u00f3rio"
     },
     {
         "language": "Romanian",
         "symbol": "ro",
-        "text": "Cuprins"
+        "text": "repertoriu"
     },
     {
         "language": "Russian",
         "symbol": "ru",
-        "text": "\u0421\u043e\u0434\u0435\u0440\u0436\u0430\u043d\u0438\u0435"
+        "text": "\u0445\u0440\u0430\u043d\u0438\u043b\u0438\u0449\u0435"
     },
     {
         "language": "Serbian",
         "symbol": "sr",
-        "text": "\u0421\u0430\u0434\u0440\u0436\u0430\u0458"
+        "text": "\u0441\u043f\u0440\u0435\u043c\u0438\u0448\u0442\u0435"
     },
     {
         "language": "Slovak",
         "symbol": "sk",
-        "text": "Obsah"
+        "text": "\u00dalo\u017eisko"
     },
     {
         "language": "Slovenian",
         "symbol": "sl",
-        "text": "Vsebina"
+        "text": "odlagali\u0161\u010de"
     },
     {
         "language": "Spanish",
         "symbol": "es",
-        "text": "Contenido"
+        "text": "repositorio"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "Inneh\u00e5ll"
+        "text": "repositorium"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
-        "text": "\u041c\u0443\u043d\u0434\u0430\u0440\u0438\u04b7\u0430"
+        "text": "\u0430\u043d\u0431\u043e\u0440"
     },
     {
         "language": "Thai",
         "symbol": "th",
-        "text": "\u0e2a\u0e32\u0e23\u0e1a\u0e31\u0e0d"
+        "text": "\u0e17\u0e35\u0e48\u0e40\u0e01\u0e47\u0e1a"
     },
     {
         "language": "Turkish",
         "symbol": "tr",
-        "text": "\u0130\u00e7indekiler"
+        "text": "depo"
     },
     {
         "language": "Ukrainian",
         "symbol": "uk",
-        "text": "\u0417\u043c\u0456\u0441\u0442"
+        "text": "\u0441\u0445\u043e\u0432\u0438\u0449\u0435"
     },
     {
         "language": "Vietnamese",
         "symbol": "vi",
-        "text": "N\u1ed9i dung"
+        "text": "kho"
     }
 ]
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Copyright.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Copyright.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884058%*

 * *Differences: {'31': "{'text': 'Upphovsrätt'}", '4': "{'text': 'Copyright'}"}*

```diff
@@ -18,15 +18,15 @@
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
         "text": "\u7248\u6743"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u7248\u6b0a"
+        "text": "Copyright"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Autorska prava"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Derechos de autor"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "upphovsr\u00e4tt"
+        "text": "Upphovsr\u00e4tt"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u04b2\u0443\u049b\u0443\u049b\u0438 \u043c\u0443\u0430\u043b\u043b\u0438\u0444"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Download notebook file.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Download notebook file.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884058%*

 * *Differences: {'31': "{'text': 'Ladda ner notebook-fil'}", '4': "{'text': '下載 Notebook 檔案'}"}*

```diff
@@ -18,15 +18,15 @@
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
         "text": "\u4e0b\u8f7d\u7b14\u8bb0\u672c\u6587\u4ef6"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u4e0b\u8f09\u7b46\u8a18\u672c\u6587\u4ef6"
+        "text": "\u4e0b\u8f09 Notebook \u6a94\u6848"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Preuzmi datoteku bilje\u017enice"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Descargar archivo de cuaderno"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "Ladda ner anteckningsbokfilen"
+        "text": "Ladda ner notebook-fil"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u0424\u0430\u0439\u043b\u0438 \u0434\u0430\u0444\u0442\u0430\u0440\u0440\u043e \u0437\u0435\u0440\u043a\u0430\u0448\u04e3 \u043a\u0443\u043d\u0435\u0434"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Download source file.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Download source file.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963768115942028%*

 * *Differences: {'4': "{'text': '下載原始檔'}"}*

```diff
@@ -18,15 +18,15 @@
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
         "text": "\u4e0b\u8f7d\u6e90\u6587\u4ef6"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u4e0b\u8f09\u6e90\u6587\u4ef6"
+        "text": "\u4e0b\u8f09\u539f\u59cb\u6a94"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Preuzmi izvornu datoteku"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Download this page.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Download this page.json`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Edit this page.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Edit this page.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884059%*

 * *Differences: {'3': "{'text': '编辑此页面'}", '4': "{'text': '編輯此頁面'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u0420\u0435\u0434\u0430\u043a\u0442\u0438\u0440\u0430\u0439\u0442\u0435 \u0442\u0430\u0437\u0438 \u0441\u0442\u0440\u0430\u043d\u0438\u0446\u0430"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u7f16\u8f91\u8fd9\u4e2a\u9875\u9762"
+        "text": "\u7f16\u8f91\u6b64\u9875\u9762"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u7de8\u8f2f\u9019\u500b\u9801\u9762"
+        "text": "\u7de8\u8f2f\u6b64\u9801\u9762"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Uredite ovu stranicu"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Fullscreen mode.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Fullscreen mode.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954954954954953%*

 * *Differences: {'4': "{'text': '全螢幕模式'}"}*

```diff
@@ -18,15 +18,15 @@
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
         "text": "\u5168\u5c4f\u6a21\u5f0f"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u5168\u5c4f\u6a21\u5f0f"
+        "text": "\u5168\u87a2\u5e55\u6a21\u5f0f"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Na\u010din preko cijelog zaslona"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Last updated on.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Last updated on.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963768115942028%*

 * *Differences: {'26': "{'text': '最後更新時間：'}"}*

```diff
@@ -128,15 +128,15 @@
         "language": "Bengali",
         "symbol": "bn",
         "text": "\u09b8\u09b0\u09cd\u09ac\u09b6\u09c7\u09b7 \u0986\u09aa\u09a1\u09c7\u099f"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u4e0a\u6b21\u66f4\u65b0\u6642\u9593\uff1a"
+        "text": "\u6700\u5f8c\u66f4\u65b0\u6642\u9593\uff1a"
     },
     {
         "language": "Finnish",
         "symbol": "fi",
         "text": "Viimeksi p\u00e4ivitetty"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Launch.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Launch.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {'3': "{'text': '启动'}", '31': "{'text': 'Öppna'}", '4': "{'text': '啟動'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u0421\u0442\u0430\u0440\u0442\u0438\u0440\u0430\u043d\u0435"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u53d1\u5c04"
+        "text": "\u542f\u52a8"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u767c\u5c04"
+        "text": "\u555f\u52d5"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Pokrenite"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Lanzamiento"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "Lansera"
+        "text": "\u00d6ppna"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u041e\u0493\u043e\u0437"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Open an issue.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Open an issue.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {'3': "{'text': '创建议题'}", '31': "{'text': 'Öppna en problemrapport'}", '4': "{'text': '開啟議題'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u041e\u0442\u0432\u043e\u0440\u0435\u0442\u0435 \u043f\u0440\u043e\u0431\u043b\u0435\u043c"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u6253\u5f00\u4e00\u4e2a\u95ee\u9898"
+        "text": "\u521b\u5efa\u8bae\u9898"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u6253\u958b\u4e00\u500b\u554f\u984c"
+        "text": "\u958b\u555f\u8b70\u984c"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Otvorite izdanje"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Abrir un problema"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "\u00d6ppna ett problem"
+        "text": "\u00d6ppna en problemrapport"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u041c\u0430\u0441\u044a\u0430\u043b\u0430\u0440\u043e \u043a\u0443\u0448\u043e\u0435\u0434"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Print to PDF.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Print to PDF.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884059%*

 * *Differences: {'3': "{'text': '列印成 PDF'}", '4': "{'text': '列印成 PDF'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u041f\u0435\u0447\u0430\u0442 \u0432 PDF"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u5217\u5370\u6210PDF"
+        "text": "\u5217\u5370\u6210 PDF"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u5217\u5370\u6210PDF"
+        "text": "\u5217\u5370\u6210 PDF"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Ispis u PDF"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Search the docs.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/suggest edit.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4629629629629629%*

 * *Differences: {'0': "{'text': 'suggest edit'}",*

 * * '1': "{'text': 'أقترح تحرير'}",*

 * * '10': "{'language': 'Chinese Traditional', 'symbol': 'zh-tw', 'text': '提出修改建議'}",*

 * * '11': "{'language': 'Danish', 'symbol': 'da', 'text': 'foreslå redigering'}",*

 * * '12': "{'text': 'soovita muuta'}",*

 * * '14': "{'language': 'Lithuanian', 'symbol': 'lt', 'text': 'pasiūlyti redaguoti'}",*

 * * '15': "{'language': 'Portuguese', 'symbol': 'pt', 'text': 'sugerir edição'}",*

 * * '16': "{'language': 'Serbian', 'symbol': 'sr', 'text': 'предложи уређивање'}",*

 * * '17 […]*

```diff
@@ -1,187 +1,227 @@
 [
     {
         "language": "English",
         "symbol": "en",
-        "text": "Search the docs ..."
+        "text": "suggest edit"
     },
     {
         "language": "Arabic",
         "symbol": "ar",
-        "text": "\u0627\u0628\u062d\u062b \u0641\u064a \u0627\u0644\u0645\u0633\u062a\u0646\u062f\u0627\u062a ..."
+        "text": "\u0623\u0642\u062a\u0631\u062d \u062a\u062d\u0631\u064a\u0631"
     },
     {
-        "language": "Bulgarian",
-        "symbol": "bg",
-        "text": "\u0422\u044a\u0440\u0441\u0435\u043d\u0435 \u0432 \u0434\u043e\u043a\u0443\u043c\u0435\u043d\u0442\u0438\u0442\u0435 ..."
+        "language": "Dutch",
+        "symbol": "nl",
+        "text": "suggereren bewerken"
     },
     {
-        "language": "Chinese Simplified",
-        "symbol": "zh_CN",
-        "text": "\u641c\u7d22\u6587\u6863..."
+        "language": "French",
+        "symbol": "fr",
+        "text": "suggestion de modification"
     },
     {
-        "language": "Chinese Traditional",
-        "symbol": "zh-tw",
-        "text": "\u641c\u7d22\u6587\u6a94..."
+        "language": "German",
+        "symbol": "de",
+        "text": "vorschlagen zu bearbeiten"
     },
     {
-        "language": "Croatian",
-        "symbol": "hr",
-        "text": "Pretra\u017eite dokumente ..."
+        "language": "Italian",
+        "symbol": "it",
+        "text": "suggerisci modifica"
     },
     {
-        "language": "Czech",
-        "symbol": "cs",
-        "text": "Hledat v dokumentech ..."
+        "language": "Japanese",
+        "symbol": "ja",
+        "text": "\u7de8\u96c6\u3092\u63d0\u6848\u3059\u308b"
     },
     {
-        "language": "Danish",
-        "symbol": "da",
-        "text": "S\u00f8g i dokumenterne ..."
+        "language": "Russian",
+        "symbol": "ru",
+        "text": "\u043f\u0440\u0435\u0434\u043b\u043e\u0436\u0438\u0442\u044c \u0440\u0435\u0434\u0430\u043a\u0442\u0438\u0440\u043e\u0432\u0430\u0442\u044c"
     },
     {
-        "language": "Dutch",
-        "symbol": "nl",
-        "text": "Doorzoek de documenten ..."
+        "language": "Spanish",
+        "symbol": "es",
+        "text": "sugerir editar"
     },
     {
-        "language": "Esperanto",
-        "symbol": "eo",
-        "text": "Ser\u0109u la dokumentojn ..."
+        "language": "Chinese Simplified",
+        "symbol": "zh_CN",
+        "text": "\u63d0\u51fa\u4fee\u6539\u5efa\u8bae"
+    },
+    {
+        "language": "Chinese Traditional",
+        "symbol": "zh-tw",
+        "text": "\u63d0\u51fa\u4fee\u6539\u5efa\u8b70"
+    },
+    {
+        "language": "Danish",
+        "symbol": "da",
+        "text": "foresl\u00e5 redigering"
     },
     {
         "language": "Estonian",
         "symbol": "et",
-        "text": "Dokumentidest otsimine ..."
+        "text": "soovita muuta"
     },
     {
-        "language": "Finnish",
-        "symbol": "fi",
-        "text": "Hae dokumenteista ..."
+        "language": "Hebrew",
+        "symbol": "iw",
+        "text": "\u05de\u05e6\u05d9\u05e2 \u05dc\u05e2\u05e8\u05d5\u05da"
     },
     {
-        "language": "French",
-        "symbol": "fr",
-        "text": "Rechercher dans les documents ..."
+        "language": "Lithuanian",
+        "symbol": "lt",
+        "text": "pasi\u016blyti redaguoti"
     },
     {
-        "language": "German",
-        "symbol": "de",
-        "text": "Durchsuchen Sie die Dokumente ..."
+        "language": "Portuguese",
+        "symbol": "pt",
+        "text": "sugerir edi\u00e7\u00e3o"
+    },
+    {
+        "language": "Serbian",
+        "symbol": "sr",
+        "text": "\u043f\u0440\u0435\u0434\u043b\u043e\u0436\u0438 \u0443\u0440\u0435\u0452\u0438\u0432\u0430\u045a\u0435"
     },
     {
         "language": "Greek",
         "symbol": "el",
-        "text": "\u0391\u03bd\u03b1\u03b6\u03ae\u03c4\u03b7\u03c3\u03b7 \u03c3\u03c4\u03b1 \u03ad\u03b3\u03b3\u03c1\u03b1\u03c6\u03b1 ..."
+        "text": "\u03c0\u03c1\u03bf\u03c4\u03b5\u03af\u03bd\u03c9 \u03b5\u03c0\u03b5\u03be\u03b5\u03c1\u03b3\u03b1\u03c3\u03af\u03b1"
     },
     {
-        "language": "Hebrew",
-        "symbol": "iw",
-        "text": "\u05d7\u05e4\u05e9 \u05d1\u05de\u05e1\u05de\u05db\u05d9\u05dd ..."
+        "language": "Polish",
+        "symbol": "pl",
+        "text": "zaproponuj edycj\u0119"
     },
     {
-        "language": "Indonesian",
-        "symbol": "id",
-        "text": "Telusuri dokumen ..."
+        "language": "Thai",
+        "symbol": "th",
+        "text": "\u0e41\u0e19\u0e30\u0e19\u0e33\u0e41\u0e01\u0e49\u0e44\u0e02"
     },
     {
-        "language": "Italian",
-        "symbol": "it",
-        "text": "Cerca nei documenti ..."
+        "language": "Czech",
+        "symbol": "cs",
+        "text": "navrhnout \u00fapravy"
     },
     {
-        "language": "Japanese",
-        "symbol": "ja",
-        "text": "\u30c9\u30ad\u30e5\u30e1\u30f3\u30c8\u3092\u691c\u7d22..."
+        "language": "Slovenian",
+        "symbol": "sl",
+        "text": "predlagajte urejanje"
+    },
+    {
+        "language": "Swedish",
+        "symbol": "sv",
+        "text": "f\u00f6resl\u00e5 \u00e4ndring"
+    },
+    {
+        "language": "Norwegian",
+        "symbol": "no",
+        "text": "foresl\u00e5 redigering"
     },
     {
         "language": "Korean",
         "symbol": "ko",
-        "text": "\ubb38\uc11c \uac80\uc0c9 ..."
+        "text": "\ud3b8\uc9d1 \uc81c\uc548"
     },
     {
-        "language": "Latvian",
-        "symbol": "lv",
-        "text": "Mekl\u0113t dokumentos ..."
+        "language": "Indonesian",
+        "symbol": "id",
+        "text": "menyarankan edit"
     },
     {
-        "language": "Lithuanian",
-        "symbol": "lt",
-        "text": "Ie\u0161koti dokumentuose ..."
+        "language": "Filipino",
+        "symbol": "tl",
+        "text": "iminumungkahi i-edit"
     },
     {
-        "language": "Norwegian",
-        "symbol": "no",
-        "text": "S\u00f8k i dokumentene ..."
+        "language": "Croatian",
+        "symbol": "hr",
+        "text": "predlo\u017ei ure\u0111ivanje"
     },
     {
-        "language": "Polish",
-        "symbol": "pl",
-        "text": "Przeszukaj dokumenty ..."
+        "language": "Catalan",
+        "symbol": "ca",
+        "text": "suggerir edici\u00f3"
     },
     {
-        "language": "Portuguese",
-        "symbol": "pt",
-        "text": "Pesquise os documentos ..."
+        "language": "Marathi",
+        "symbol": "mr",
+        "text": "\u0938\u0902\u092a\u093e\u0926\u0928 \u0938\u0941\u091a\u0935\u093e"
     },
     {
-        "language": "Romanian",
-        "symbol": "ro",
-        "text": "C\u0103uta\u021bi documente ..."
+        "language": "Tamil",
+        "symbol": "ta",
+        "text": "\u0ba4\u0bbf\u0bb0\u0bc1\u0ba4\u0bcd\u0ba4 \u0baa\u0bb0\u0bbf\u0ba8\u0bcd\u0ba4\u0bc1\u0bb0\u0bc8\u0b95\u0bcd\u0b95\u0bb5\u0bc1\u0bae\u0bcd"
     },
     {
-        "language": "Russian",
-        "symbol": "ru",
-        "text": "\u0418\u0441\u043a\u0430\u0442\u044c \u0432 \u0434\u043e\u043a\u0443\u043c\u0435\u043d\u0442\u0430\u0445 ..."
+        "language": "Turkish",
+        "symbol": "tr",
+        "text": "d\u00fczenleme \u00f6ner"
     },
     {
-        "language": "Serbian",
-        "symbol": "sr",
-        "text": "\u041f\u0440\u0435\u0442\u0440\u0430\u0436\u0438\u0442\u0435 \u0434\u043e\u043a\u0443\u043c\u0435\u043d\u0442\u0435 ..."
+        "language": "Vietnamese",
+        "symbol": "vi",
+        "text": "\u0111\u1ec1 ngh\u1ecb ch\u1ec9nh s\u1eeda"
+    },
+    {
+        "language": "Ukrainian",
+        "symbol": "uk",
+        "text": "\u0437\u0430\u043f\u0440\u043e\u043f\u043e\u043d\u0443\u0432\u0430\u0442\u0438 \u0440\u0435\u0434\u0430\u0433\u0443\u0432\u0430\u0442\u0438"
+    },
+    {
+        "language": "Telugu",
+        "symbol": "te",
+        "text": "\u0c38\u0c35\u0c30\u0c3f\u0c02\u0c1a\u0c2e\u0c28\u0c3f \u0c38\u0c42\u0c1a\u0c3f\u0c02\u0c1a\u0c02\u0c21\u0c3f"
     },
     {
         "language": "Slovak",
         "symbol": "sk",
-        "text": "H\u013eada\u0165 v dokumentoch ..."
+        "text": "navrhn\u00fa\u0165 \u00fapravu"
     },
     {
-        "language": "Slovenian",
-        "symbol": "sl",
-        "text": "Poi\u0161\u010dite dokumente ..."
+        "language": "Romanian",
+        "symbol": "ro",
+        "text": "sugereaz\u0103 editare"
     },
     {
-        "language": "Spanish",
-        "symbol": "es",
-        "text": "Buscar los documentos ..."
+        "language": "Malay",
+        "symbol": "ms",
+        "text": "cadangkan edit"
     },
     {
-        "language": "Swedish",
-        "symbol": "sv",
-        "text": "S\u00f6k i dokumenten ..."
+        "language": "Urdu",
+        "symbol": "ur",
+        "text": "\u062a\u0631\u0645\u06cc\u0645 \u06a9\u06cc \u062a\u062c\u0648\u06cc\u0632 \u06a9\u0631\u06cc\u06ba"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
-        "text": "\u04b6\u0443\u0441\u0442\u0443\u04b7\u04ef\u0438 \u04b3\u0443\u04b7\u04b7\u0430\u0442\u04b3\u043e ..."
+        "text": "\u043f\u0435\u0448\u043d\u0438\u04b3\u043e\u0434 \u0432\u0438\u0440\u043e\u0438\u0448"
     },
     {
-        "language": "Thai",
-        "symbol": "th",
-        "text": "\u0e04\u0e49\u0e19\u0e2b\u0e32\u0e40\u0e2d\u0e01\u0e2a\u0e32\u0e23 ..."
+        "language": "Malayalam",
+        "symbol": "ml",
+        "text": "\u0d0e\u0d21\u0d3f\u0d31\u0d4d\u0d31\u0d41\u0d1a\u0d46\u0d2f\u0d4d\u0d2f\u0d3e\u0d7b \u0d28\u0d3f\u0d7c\u0d26\u0d4d\u0d26\u0d47\u0d36\u0d3f\u0d15\u0d4d\u0d15\u0d41\u0d15"
     },
     {
-        "language": "Turkish",
-        "symbol": "tr",
-        "text": "Belgelerde ara ..."
+        "language": "Latvian",
+        "symbol": "lv",
+        "text": "ieteikt redi\u0123\u0113t"
     },
     {
-        "language": "Ukrainian",
-        "symbol": "uk",
-        "text": "\u0428\u0443\u043a\u0430\u0442\u0438 \u0432 \u0434\u043e\u043a\u0443\u043c\u0435\u043d\u0442\u0430\u0445 ..."
+        "language": "Finnish",
+        "symbol": "fi",
+        "text": "ehdottaa muokkausta"
     },
     {
-        "language": "Vietnamese",
-        "symbol": "vi",
-        "text": "T\u00ecm ki\u1ebfm t\u00e0i li\u1ec7u ..."
+        "language": "Esperanto",
+        "symbol": "eo",
+        "text": "sugesti redaktadon"
+    },
+    {
+        "language": "Bulgarian",
+        "symbol": "bg",
+        "text": "\u043f\u0440\u0435\u0434\u043b\u043e\u0436\u0438 \u0440\u0435\u0434\u0430\u043a\u0442\u0438\u0440\u0430\u043d\u0435"
     }
 ]
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Source repository.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Source repository.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {'3': "{'text': '源码库'}", '31': "{'text': 'Källkodsrepositorium'}", '4': "{'text': '來源儲存庫'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u0425\u0440\u0430\u043d\u0438\u043b\u0438\u0449\u0435 \u043d\u0430 \u0438\u0437\u0442\u043e\u0447\u043d\u0438\u043a\u0430"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u6e90\u5e93"
+        "text": "\u6e90\u7801\u5e93"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u6e90\u5eab"
+        "text": "\u4f86\u6e90\u5132\u5b58\u5eab"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Izvorno spremi\u0161te"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Repositorio de origen"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "K\u00e4llf\u00f6rvar"
+        "text": "K\u00e4llkodsrepositorium"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u0410\u043d\u0431\u043e\u0440\u0438 \u043c\u0430\u043d\u0431\u0430\u044a"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Sphinx Book Theme.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Sphinx Book Theme.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {'3': "{'text': 'Sphinx Book 主题'}",*

 * * '31': "{'text': 'Sphinx Boktema'}",*

 * * '4': "{'text': 'Sphinx Book 佈景主題'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u0422\u0435\u043c\u0430 \u043d\u0430 \u043a\u043d\u0438\u0433\u0430\u0442\u0430 Sphinx"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u72ee\u8eab\u4eba\u9762\u50cf\u4e66\u4e3b\u9898"
+        "text": "Sphinx Book \u4e3b\u9898"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u7345\u8eab\u4eba\u9762\u50cf\u66f8\u4e3b\u984c"
+        "text": "Sphinx Book \u4f48\u666f\u4e3b\u984c"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Tema knjige Sphinx"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Tema del libro de la esfinge"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "Sphinx boktema"
+        "text": "Sphinx Boktema"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u0421\u0444\u0438\u043d\u043a\u0441 \u041c\u0430\u0432\u0437\u04ef\u0438 \u043a\u0438\u0442\u043e\u0431"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Theme by the.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Theme by the.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884059%*

 * *Differences: {'3': "{'text': '主题作者：'}", '4': "{'text': '佈景主題作者：'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u0422\u0435\u043c\u0430 \u043e\u0442"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u4e3b\u9898\u7531"
+        "text": "\u4e3b\u9898\u4f5c\u8005\uff1a"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u4e3b\u984c\u7531"
+        "text": "\u4f48\u666f\u4e3b\u984c\u4f5c\u8005\uff1a"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Tema autora"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/Toggle navigation.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/Toggle navigation.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884059%*

 * *Differences: {'3': "{'text': '显示或隐藏导航栏'}", '4': "{'text': '顯示或隱藏導覽列'}"}*

```diff
@@ -13,20 +13,20 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u041f\u0440\u0435\u0432\u043a\u043b\u044e\u0447\u0432\u0430\u043d\u0435 \u043d\u0430 \u043d\u0430\u0432\u0438\u0433\u0430\u0446\u0438\u044f\u0442\u0430"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u5207\u6362\u5bfc\u822a"
+        "text": "\u663e\u793a\u6216\u9690\u85cf\u5bfc\u822a\u680f"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
-        "text": "\u5207\u63db\u5c0e\u822a"
+        "text": "\u986f\u793a\u6216\u96b1\u85cf\u5c0e\u89bd\u5217"
     },
     {
         "language": "Croatian",
         "symbol": "hr",
         "text": "Uklju\u010di / isklju\u010di navigaciju"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/next page.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/next page.json`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/open issue.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/open issue.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884059%*

 * *Differences: {'3': "{'text': '创建议题'}", '31': "{'text': 'öppna problemrapport'}"}*

```diff
@@ -13,15 +13,15 @@
         "language": "Bulgarian",
         "symbol": "bg",
         "text": "\u043e\u0442\u0432\u043e\u0440\u0435\u043d \u0431\u0440\u043e\u0439"
     },
     {
         "language": "Chinese Simplified",
         "symbol": "zh_CN",
-        "text": "\u516c\u5f00\u7684\u95ee\u9898"
+        "text": "\u521b\u5efa\u8bae\u9898"
     },
     {
         "language": "Chinese Traditional",
         "symbol": "zh-tw",
         "text": "\u516c\u958b\u7684\u554f\u984c"
     },
     {
@@ -153,15 +153,15 @@
         "language": "Spanish",
         "symbol": "es",
         "text": "Tema abierto"
     },
     {
         "language": "Swedish",
         "symbol": "sv",
-        "text": "\u00f6ppet problem"
+        "text": "\u00f6ppna problemrapport"
     },
     {
         "language": "Tajik",
         "symbol": "tg",
         "text": "\u0431\u0430\u0440\u043e\u0440\u0438\u0448\u0438 \u043a\u0443\u0448\u043e\u0434"
     },
     {
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/assets/translations/jsons/previous page.json` & `tskit_book_theme-1.0.1/src/tskit_book_theme/assets/translations/jsons/previous page.json`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/header_buttons/__init__.py` & `tskit_book_theme-1.0.1/src/tskit_book_theme/header_buttons/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,190 @@
 """Generate metadata for header buttons."""
-
 from sphinx.errors import SphinxError
+from sphinx.locale import get_translation
+from pydata_sphinx_theme.utils import config_provided_by_user, get_theme_options_dict
+
+from sphinx.util import logging
+
+
+LOGGER = logging.getLogger(__name__)
+MESSAGE_CATALOG_NAME = "booktheme"
+translation = get_translation(MESSAGE_CATALOG_NAME)
 
 
-def _as_bool(var):
+def as_bool(var):
     """Cast string as a boolean with some extra checks.
 
     If var is a string, it will be matched to 'true'/'false'
     If var is a bool, it will be returned
     If var is None, it will return False.
     """
     if isinstance(var, str):
         return var.lower() == "true"
     elif isinstance(var, bool):
         return var
     else:
         return False
 
 
+def get_repo_parts(context):
+    """Return the parts of the source repository."""
+    for provider in ["github", "bitbucket", "gitlab"]:
+        if f"{provider.lower()}_url" in context:
+            provider_url = context[f"{provider.lower()}_url"]
+            source_user = context[f"{provider.lower()}_user"]
+            source_repo = context[f"{provider.lower()}_repo"]
+            return provider_url, source_user, source_repo, provider
+
+
+def get_repo_url(context):
+    """Return the provider URL based on what is defined in context."""
+    provider_url, user, repo, provider = get_repo_parts(context)
+    repo_url = f"{provider_url}/{user}/{repo}"
+    return repo_url, provider
+
+
 def prep_header_buttons(app, pagename, templatename, context, doctree):
     """Prep an empty list that we'll populate with header buttons."""
     context["header_buttons"] = []
 
 
 def add_header_buttons(app, pagename, templatename, context, doctree):
-    """Populate the context with header button metadata we'll insert in templates."""
-    opts = app.config.html_theme_options
+    """Add basic and general header buttons, we'll add source/launch later."""
+    opts = get_theme_options_dict(app)
     pathto = context["pathto"]
     header_buttons = context["header_buttons"]
 
     # If we have a suffix, then we have a source file
     suff = context.get("page_source_suffix")
 
-    # Full screen button
-    if _as_bool(opts.get("use_fullscreen_button", True)):
-        header_buttons.append(
-            {
-                "type": "javascript",
-                "javascript": "toggleFullScreen()",
-                "tooltip": "Fullscreen mode",
-                "icon": "fas fa-expand",
-            }
-        )
-
-    # Edit this page button
-    # Add HTML context variables that the pydata theme uses that we configure elsewhere
-    # For some reason the source_suffix sometimes isn't there even when doctree is
-    repo_keywords = [
-        "use_issues_button",
-        "use_edit_page_button",
-        "use_repository_button",
-    ]
-    for key in repo_keywords:
-        opts[key] = _as_bool(opts.get(key))
-
-    if any(opts.get(kw) for kw in repo_keywords):
-        repo_url = opts.get("repository_url", "")
-        if not repo_url:
-            raise SphinxError(
-                "Repository buttons enabled, but repository_url not given. "
-                "Please add a repository_url."
-            )
-        repo_buttons = []
-        if opts.get("use_repository_button"):
-            repo_buttons.append(
-                {
-                    "type": "link",
-                    "url": repo_url,
-                    "tooltip": "Source repository",
-                    "text": "repository",
-                    "icon": "fab fa-github",
-                }
-            )
-
-        if opts.get("use_issues_button"):
-            repo_buttons.append(
-                {
-                    "type": "link",
-                    "url": f"{repo_url}/issues/new?title=Issue%20on%20page%20%2F{context['pagename']}.html&body=Your%20issue%20content%20here.",  # noqa: E501
-                    "text": "open issue",
-                    "tooltip": "Open an issue",
-                    "icon": "fas fa-lightbulb",
-                }
-            )
-
-        if opts.get("use_edit_page_button") and doctree and suff:
-            branch = opts.get("repository_branch", "")
-            if branch == "":
-                branch = "master"
-            relpath = opts.get("path_to_docs", "")
-            org, repo = repo_url.strip("/").split("/")[-2:]
-
-            # Update the context because this is what the get_edit_url function uses.
-            context.update(
-                {
-                    "github_user": org,
-                    "github_repo": repo,
-                    "github_version": branch,
-                    "doc_path": relpath,
-                }
-            )
-
-            repo_buttons.append(
-                {
-                    "type": "link",
-                    "url": context["get_edit_url"](),
-                    "tooltip": "Edit this page",
-                    "text": "suggest edit",
-                    "icon": "fas fa-pencil-alt",
-                }
-            )
-
-        # If we have multiple repo buttons enabled, add a group, otherwise just 1 button
-        if len(repo_buttons) > 1:
-            for rb in repo_buttons:
-                rb["tooltip_placement"] = "left"
-            header_buttons.append(
-                {
-                    "type": "group",
-                    "tooltip": "Source repositories",
-                    "icon": "fab fa-github",
-                    "buttons": repo_buttons,
-                    "label": "repository-buttons",
-                }
-            )
-        elif len(repo_buttons) == 1:
-            # Remove the text since it's just a single button, want just an icon.
-            repo_buttons[0]["text"] = ""
-            header_buttons.extend(repo_buttons)
-
     # Download buttons for various source content.
-    if _as_bool(opts.get("use_download_button", True)) and suff:
+    if as_bool(opts.get("use_download_button", True)) and suff:
         download_buttons = []
 
-        # Create the dropdown list of buttons
+        # An ipynb file if it was created as part of the build (e.g. by MyST-NB)
         if context.get("ipynb_source"):
             download_buttons.append(
                 {
                     "type": "link",
                     "url": f'{pathto("_sources", 1)}/{context.get("ipynb_source")}',
                     "text": ".ipynb",
                     "icon": "fas fa-code",
-                    "tooltip": "Download notebook file",
-                    "tooltip_placement": "left",
+                    "tooltip": translation("Download notebook file"),
+                    "label": "download-notebook-button",
                 }
             )
 
+        # Download the source file
         download_buttons.append(
             {
                 "type": "link",
                 "url": f'{pathto("_sources", 1)}/{context["sourcename"]}',
                 "text": suff,
-                "tooltip": "Download source file",
-                "tooltip_placement": "left",
+                "tooltip": translation("Download source file"),
                 "icon": "fas fa-file",
+                "label": "download-source-button",
             }
         )
         download_buttons.append(
             {
                 "type": "javascript",
-                "javascript": "printPdf(this)",
+                "javascript": "window.print()",
                 "text": ".pdf",
-                "tooltip": "Print to PDF",
-                "tooltip_placement": "left",
+                "tooltip": translation("Print to PDF"),
                 "icon": "fas fa-file-pdf",
+                "label": "download-pdf-button",
             }
         )
 
         # Add the group
         header_buttons.append(
             {
                 "type": "group",
-                "tooltip": "Download this page",
+                "tooltip": translation("Download this page"),
                 "icon": "fas fa-download",
                 "buttons": download_buttons,
                 "label": "download-buttons",
             }
         )
+
+    # Full screen button
+    if as_bool(opts.get("use_fullscreen_button", True)):
+        header_buttons.append(
+            {
+                "type": "javascript",
+                "javascript": "toggleFullScreen()",
+                "tooltip": translation("Fullscreen mode"),
+                "icon": "fas fa-expand",
+                "label": "fullscreen-button",
+            }
+        )
+
+
+def update_sourcename(app):
+    # Download the source file
+    # Sphinx defaults to .txt for html_source_suffix even though the pages almost
+    # always are stored in their native suffix (.rst, .md, or .ipynb). So unless
+    # the user manually specifies an html_source_suffix, default to an empty string.
+    # _raw_config is the configuration as provided by the user.
+    # If a key isn't in it, then the user didn't provide it
+    if not config_provided_by_user(app, "html_sourcelink_suffix"):
+        app.config.html_sourcelink_suffix = ""
+
+
+def update_context_with_repository_info(app):
+    """Update pydata `html_context` options for source from `repository_url`.
+
+    We do this because we use repository_url as one config to define the URL,
+    while the PST uses a collection of {provider}_{key} pairs in html_context.
+    So here we insert those context variables on our own.
+    """
+    opts = get_theme_options_dict(app)
+    context = app.config.html_context
+
+    # This is the way to give repository info. If it doesn't exist, do nothing.
+    repo_url = opts.get("repository_url", "")
+    if not repo_url:
+        return
+
+    # Check for manually given options first
+    branch = opts.get("repository_branch", "")
+    provider = opts.get("repository_provider", "")
+    relpath = opts.get("path_to_docs", "")
+    if branch == "":
+        branch = "main"
+
+    # We assume the final two parts of the repository URL are the org/repo
+    provider_url, org, repo = repo_url.strip("/").rsplit("/", 2)
+
+    # Infer the provider if it wasn't manually given
+    default_provider_urls = {
+        "bitbucket": "bitbucket.org",
+        "github": "github.com",
+        "gitlab": "gitlab.com",
+    }
+
+    # If no provider is given, try to infer one from the repo url
+    if provider == "":
+        for iprov in default_provider_urls.keys():
+            if iprov in provider_url.lower():
+                provider = iprov
+                break
+
+    # If provider is still empty, raise an error because we don't recognize it
+    if provider == "":
+        raise SphinxError(
+            (
+                f"Provider not recognized in repository url {repo_url}. "
+                "If you're using a custom provider URL, specify `repository_provider`"
+            )
+        )
+
+    # Update the context because this is what the get_edit_url function uses.
+    repository_information = {
+        f"{provider}_user": org,
+        f"{provider}_repo": repo,
+        f"{provider}_version": branch,
+        f"{provider}_url": provider_url,
+        "doc_path": relpath,
+    }
+    context.update(repository_information)
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/header_buttons/launch.py` & `tskit_book_theme-1.0.1/src/tskit_book_theme/header_buttons/launch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+"""Launch buttons for Binder / Thebe / Colab / etc."""
 from pathlib import Path
 from typing import Any, Dict, Optional
-from urllib.parse import urlencode
+from urllib.parse import urlencode, quote
 
 from docutils.nodes import document
 from sphinx.application import Sphinx
+from sphinx.locale import get_translation
 from sphinx.util import logging
 from shutil import copy2
 
+from . import get_repo_parts, get_repo_url
+
 
 SPHINX_LOGGER = logging.getLogger(__name__)
 
+MESSAGE_CATALOG_NAME = "booktheme"
+translation = get_translation(MESSAGE_CATALOG_NAME)
+
 
 def add_launch_buttons(
     app: Sphinx,
     pagename: str,
     templatename: str,
     context: Dict[str, Any],
     doctree: Optional[document],
@@ -26,29 +33,35 @@
     :param context: A dictionary of values that are given to the template engine,
         to render the page and can be modified to include custom values.
     :param doctree: A doctree when the page is created from a reST documents;
         it will be None when the page is created from an HTML template alone.
 
     """
 
-    # First decide if we'll insert any links
     path = app.env.doc2path(pagename)
     extension = Path(path).suffix
 
-    # If so, insert the URLs depending on the configuration
+    # Don't do anything if no launch provider is configured
     config_theme = app.config["html_theme_options"]
     launch_buttons = config_theme.get("launch_buttons", {})
-    if not launch_buttons or not _is_notebook(app, pagename):
+    if (
+        not launch_buttons
+        or not _is_notebook(app, context)
+        or not any(
+            launch_buttons.get(key)
+            for key in ("binderhub_url", "jupyterhub_url", "thebe", "colab_url")
+        )
+    ):
         return
 
     # Grab the header buttons from context as it should already exist.
     header_buttons = context["header_buttons"]
 
     # Check if we have a markdown notebook, and if so then add a link to the context
-    if _is_notebook(app, pagename) and (
+    if _is_notebook(app, context) and (
         context["sourcename"].endswith(".md")
         or context["sourcename"].endswith(".md.txt")
     ):
         # Figure out the folders we want
         out_dir = Path(app.outdir)
         build_dir = out_dir.parent
         ntbk_dir = build_dir.joinpath("jupyter_execute")
@@ -57,18 +70,17 @@
         path_ntbk = ntbk_dir.joinpath(pagename).with_suffix(".ipynb")
         path_new_notebook = sources_dir.joinpath(pagename).with_suffix(".ipynb")
         # Copy the notebook to `_sources` dir so it can be downloaded
         path_new_notebook.parent.mkdir(exist_ok=True, parents=True)
         copy2(path_ntbk, path_new_notebook)
         context["ipynb_source"] = pagename + ".ipynb"
 
-    repo_url = _get_repo_url(config_theme)
-
-    # Parse the repo parts from the URL
-    org, repo = _split_repo_url(repo_url)
+    # Get repository URL information that we'll use to build links
+    repo_url, _ = get_repo_url(context)
+    provider_url, org, repo, provider = get_repo_parts(context)
     if org is None and repo is None:
         # Skip the rest because the repo_url isn't right
         return
 
     branch = _get_branch(config_theme)
 
     # Construct the extra URL parts (app and relative path)
@@ -99,24 +111,33 @@
     launch_buttons_list = []
 
     # Now build infrastructure-specific links
     jupyterhub_url = launch_buttons.get("jupyterhub_url", "").strip("/")
     binderhub_url = launch_buttons.get("binderhub_url", "").strip("/")
     colab_url = launch_buttons.get("colab_url", "").strip("/")
     deepnote_url = launch_buttons.get("deepnote_url", "").strip("/")
+
+    # Loop through each provider and add a button for it if needed
     if binderhub_url:
-        url = (
-            f"{binderhub_url}/v2/gh/{org}/{repo}/{branch}?"
-            f"urlpath={ui_pre}/{path_rel_repo}"
-        )
+        # Any non-standard repository URL should be passed-through raw
+        if provider_url not in ["https://github.com", "https://gitlab.com"]:
+            # Generic git repository using the full repo URL as a fallback
+            url = f"{binderhub_url}/v2/git/{quote(repo_url)}/{branch}"
+        elif provider.lower() == "github":
+            url = f"{binderhub_url}/v2/gh/{org}/{repo}/{branch}"
+        elif provider.lower() == "gitlab":
+            # Binder uses %2F for gitlab for some reason
+            url = f"{binderhub_url}/v2/gl/{org}%2F{repo}/{branch}"
+
+        url = f"{url}?urlpath={ui_pre}/{path_rel_repo}"
         launch_buttons_list.append(
             {
                 "type": "link",
                 "text": "Binder",
-                "tooltip": "Launch on Binder",
+                "tooltip": translation("Launch on") + "Binder",
                 "icon": "_static/images/logo_binder.svg",
                 "url": url,
             }
         )
 
     if jupyterhub_url:
         url_params = urlencode(
@@ -126,66 +147,70 @@
             safe="/",
         )
         url = f"{jupyterhub_url}/hub/user-redirect/git-pull?{url_params}"
         launch_buttons_list.append(
             {
                 "type": "link",
                 "text": "JupyterHub",
-                "tooltip": "Launch on JupyterHub",
+                "tooltip": translation("Launch on") + "JupyterHub",
                 "icon": "_static/images/logo_jupyterhub.svg",
                 "url": url,
             }
         )
 
     if colab_url:
-        url = f"{colab_url}/github/{org}/{repo}/blob/{branch}/{path_rel_repo}"
-        launch_buttons_list.append(
-            {
-                "type": "link",
-                "text": "Colab",
-                "tooltip": "Launch on Colab",
-                "icon": "_static/images/logo_colab.png",
-                "url": url,
-            }
-        )
+        if provider.lower() != "github":
+            SPHINX_LOGGER.warning(f"Provider {provider} not supported on colab.")
+        else:
+            url = f"{colab_url}/github/{org}/{repo}/blob/{branch}/{path_rel_repo}"
+            launch_buttons_list.append(
+                {
+                    "type": "link",
+                    "text": "Colab",
+                    "tooltip": translation("Launch on") + "Colab",
+                    "icon": "_static/images/logo_colab.png",
+                    "url": url,
+                }
+            )
 
     if deepnote_url:
-        github_path = f"%2F{org}%2F{repo}%2Fblob%2F{branch}%2F{path_rel_repo}"
-        url = f"{deepnote_url}/launch?url=https%3A%2F%2Fgithub.com{github_path}"
-        launch_buttons_list.append(
-            {
-                "type": "link",
-                "text": "Deepnote",
-                "tooltip": "Launch on Deepnote",
-                "icon": "_static/images/logo_deepnote.svg",
-                "url": url,
-            }
-        )
+        if provider.lower() != "github":
+            SPHINX_LOGGER.warning(f"Provider {provider} not supported on Deepnote.")
+        else:
+            github_path = f"%2F{org}%2F{repo}%2Fblob%2F{branch}%2F{path_rel_repo}"
+            url = f"{deepnote_url}/launch?url=https%3A%2F%2Fgithub.com{github_path}"
+            launch_buttons_list.append(
+                {
+                    "type": "link",
+                    "text": "Deepnote",
+                    "tooltip": translation("Launch on") + "Deepnote",
+                    "icon": "_static/images/logo_deepnote.svg",
+                    "url": url,
+                }
+            )
 
     # Add thebe flag in context
     if launch_buttons.get("thebe", False):
         launch_buttons_list.append(
             {
                 "type": "javascript",
-                "text": "Live Code",
-                "tooltip": "Launch Thebe",
+                "text": translation("Live Code"),
+                "tooltip": translation("Launch Thebe"),
                 "javascript": "initThebeSBT()",
                 "icon": "fas fa-play",
                 "label": "launch-thebe",
             }
         )
         context["use_thebe"] = True
 
     # Add the buttons to header_buttons
-    for lb in launch_buttons_list:
-        lb["tooltip_placement"] = "left"
     header_buttons.append(
         {
             "type": "group",
-            "tooltip": "Launch interactive content",
+            "tooltip": translation("Launch interactive content"),
             "icon": "fas fa-rocket",
             "buttons": launch_buttons_list,
             "label": "launch-buttons",
         }
     )
 
 
@@ -198,25 +223,25 @@
         SPHINX_LOGGER.warning(
             f"Currently Binder/JupyterHub repositories must be on GitHub, got {url}"
         )
         org = repo = None
     return org, repo
 
 
-def _get_repo_url(config):
-    repo_url = config.get("repository_url")
-    if not repo_url:
-        raise ValueError(
-            "You must provide the key: `repository_url` to use launch buttons."
-        )
-    return repo_url
-
-
-def _is_notebook(app, pagename):
-    return app.env.metadata[pagename].get("kernelspec")
+def _is_notebook(app, context):
+    pagename = context["pagename"]
+    metadata = app.env.metadata[pagename]
+    if "kernelspec" in metadata:
+        # Most notebooks will have this
+        return True
+    elif "ipynb" in context.get("page_source_suffix", ""):
+        # Just in case, check for the suffix since some people remove the kernelspec
+        return True
+    else:
+        return False
 
 
 def _get_branch(config_theme):
     branch = config_theme.get("repository_branch")
     if not branch:
         branch = "master"
     return branch
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/nodes.py` & `tskit_book_theme-1.0.1/src/tskit_book_theme/nodes.py`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/components/sbt-sidebar-nav.html` & `tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/components/sbt-sidebar-nav.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <nav class="bd-links" id="bd-docs-nav" aria-label="Main">
-    <div class="bd-toc-item active">
+    <div class="bd-toc-item navbar-nav active">
         {% if theme_home_page_in_toc == True %}
         {#- This mimicks the pydata theme list style so we can append an extra item at the top #}
         <ul class="nav bd-sidenav bd-sidenav__home-link">
             <li class="toctree-l1{% if pagename == root_doc %} current active{% endif %}">
                 <a class="reference internal" href="{{ pathto(root_doc) }}">
                     {{ root_title }}
                 </a>
             </li>
         </ul>
         {% endif -%}
 
-        {# Ref: https://github.com/pydata/pydata-sphinx-theme/blob/8453f38ea6543e778bfc12d5c38239d25b8e30f8/src/pydata_sphinx_theme/__init__.py#L68 #}
-        {{- generate_nav_html(
+        {# Ref: https://github.com/pydata/pydata-sphinx-theme/blob/ebf7f704879a1cdc6016d6111062103353ac7677/src/pydata_sphinx_theme/__init__.py#L302 #}
+        {{- generate_toctree_html(
             startdepth=0,
             kind="sidebar",
             maxdepth=4,
             collapse=False,
             includehidden=True,
             titles_only=True,
             show_nav_level=theme_show_navbar_depth) }}
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/macros/buttons.html` & `tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/macros/buttons.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,62 @@
 {# Utility macros we'll re-use below -#}
-{% macro render_tooltip_metadata(tooltip, tooltip_placement) -%}
-data-toggle="tooltip"
-data-placement="{{ tooltip_placement }}"
-title="{{ translate(tooltip) }}"
-{%- endmacro %}
-
-
 {% macro render_inner_html(icon, text) %}
 {# used across multiple button types #}
 {% if icon -%}
-<span class="headerbtn__icon-container">
+<span class="btn__icon-container">
   {% if icon.startswith("fa") -%}
     <i class="{{ icon }}"></i>
   {% else %}
     <img src="{{ pathto(icon, 1) }}">
   {% endif -%}
 </span>
 {% endif %}
-{%- if text %}<span class="headerbtn__text-container">{{ translate(text) }}</span>{% endif -%}
+{%- if text %}<span class="btn__text-container">{{ translate(text) }}</span>{% endif -%}
 {% endmacro %}
 
 
-{% macro render_link_button(url, tooltip=None, icon=None, text=None, label=None, tooltip_placement="bottom") -%}
-<a href="{{ url }}"
-   class="headerbtn{% if label %} headerbtn-{{ label }}{% endif %}"
-   {% if tooltip %}{{ render_tooltip_metadata(tooltip, tooltip_placement) }}{% endif %}
+{% macro render_link_button(url, tooltip=None, tooltip_placement="bottom", icon=None, text=None, label=None, classes="") -%}
+<a href="{{ url }}" target="_blank"
+   class="btn btn-sm{% if label %} btn-{{ label }}{% endif %}{% if classes %} {{ classes }}{% endif %}"
+   {% if tooltip %}title="{{ translate(tooltip) }}"{% endif %}
+   data-bs-placement="{{ tooltip_placement }}" data-bs-toggle="tooltip"
 >
   {{ render_inner_html(icon, text) }}
 </a>
 {% endmacro %}
 
 
-{% macro render_js_button(javascript, tooltip=None, icon=None, text=None, label=None, tooltip_placement="bottom") %}
+{% macro render_js_button(javascript, tooltip=None, tooltip_placement="bottom", icon=None, text=None, label=None, classes="") %}
 <button onclick="{{ javascript }}"
-  class="headerbtn{% if label %} headerbtn-{{ label }}{% endif %}"
-  {% if tooltip %}{{ render_tooltip_metadata(tooltip, tooltip_placement) }}{% endif %}
+  class="btn btn-sm{% if label %} btn-{{ label }}{% endif %}{% if classes %} {{ classes }}{% endif %}"
+  {% if tooltip %}title="{{ translate(tooltip) }}"{% endif %}
+  data-bs-placement="{{ tooltip_placement }}" data-bs-toggle="tooltip"
 >
   {{ render_inner_html(icon, text) }}
 </button>
 {% endmacro %}
 
 
-{% macro render_label_input_button(for_input, tooltip=None, icon=None, text=None, label=None, tooltip_placement="bottom") -%}
-<label for="{{ for_input }}"
-  class="headerbtn{% if label %} headerbtn-{{ label }}{% endif %}"
-  {% if tooltip %}{{ render_tooltip_metadata(tooltip, tooltip_placement) }}{% endif %}
->
-  {{ render_inner_html(icon, text) }}
-</label>
-{% endmacro %}
-
-
-{% macro render_button_group(buttons, icon, tooltip=None, label=None) %}
-<div class="menu-dropdown{% if label %} menu-dropdown-{{ label }}{% endif %}">
-  <button class="headerbtn menu-dropdown__trigger"
-      aria-label="{{ tooltip }}">
-      <i class="{{ icon }}"></i>
+{% macro render_button_group(buttons, icon, tooltip=None, label=None, classes="") %}
+{# A bootstrap dropdown #}
+{# Bootstrap dropdown ref: https://getbootstrap.com/docs/5.2/components/dropdowns/ #}
+<div class="dropdown{% if label %} dropdown-{{ label }}{% endif %}{% if classes %} {{ classes }}{% endif %}">
+  <button class="btn dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false" aria-label="{{tooltip}}">
+    <i class="{{ icon }}"></i>
   </button>
-  <div class="menu-dropdown__content">
-    <ul>
+  <ul class="dropdown-menu">
       {%- for button in buttons %}
-      <li>
-        {{ render_funcs[button.pop("type")](**button) }}
-      </li>
+      {% set btype = button.get("type") %}
+      {% set bopts = button.copy() %}
+      {% set _ = bopts.pop("type") %}
+      <li>{{ render_funcs[btype](classes="dropdown-item", tooltip_placement="left", **bopts) }}</li>
       {% endfor %}
-    </ul>
-  </div>
+  </ul>
 </div>
 {% endmacro %}
 
 {%- set render_funcs = {
   "group" : render_button_group,
   "javascript" : render_js_button,
   "link": render_link_button,
-  "input_label": render_label_input_button,
 }
 -%}
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-{# Utility macros we'll re-use below -#} {% macro render_tooltip_metadata
-(tooltip, tooltip_placement) -%} data-toggle="tooltip" data-placement="{
-{ tooltip_placement }}" title="{{ translate(tooltip) }}" {%- endmacro %} {%
-macro render_inner_html(icon, text) %} {# used across multiple button types #}
-{% if icon -%}  {% if icon.startswith("fa") -%}  {% else %} [{{ pathto(icon, 1)
-}}] {% endif -%}  {% endif %} {%- if text %}{{ translate(text) }}{% endif -%}
-{% endmacro %} {% macro render_link_button(url, tooltip=None, icon=None,
-text=None, label=None, tooltip_placement="bottom") -%}
-% if tooltip %}{{ render_tooltip_metadata(tooltip, tooltip_placement) }}{%
-endif %} > {{ render_inner_html(icon, text) }}
- {% endmacro %} {% macro render_js_button(javascript, tooltip=None, icon=None,
-text=None, label=None, tooltip_placement="bottom") %}
-% if tooltip %}{{ render_tooltip_metadata(tooltip, tooltip_placement) }}{%
-endif %} > {{ render_inner_html(icon, text) }}  {% endmacro %} {% macro
-render_label_input_button(for_input, tooltip=None, icon=None, text=None,
-label=None, tooltip_placement="bottom") -%}
-% if tooltip %}{{ render_tooltip_metadata(tooltip, tooltip_placement) }}{%
-endif %} > {{ render_inner_html(icon, text) }}  {% endmacro %} {% macro
-render_button_group(buttons, icon, tooltip=None, label=None) %}
+{# Utility macros we'll re-use below -#} {% macro render_inner_html(icon, text)
+%} {# used across multiple button types #} {% if icon -%}  {% if
+icon.startswith("fa") -%}  {% else %} [{{ pathto(icon, 1) }}] {% endif -%}  {%
+endif %} {%- if text %}{{ translate(text) }}{% endif -%} {% endmacro %} {%
+macro render_link_button(url, tooltip=None, tooltip_placement="bottom",
+icon=None, text=None, label=None, classes="") -%}
+% if tooltip %}title="{{ translate(tooltip) }}"{% endif %} data-bs-placement="{
+{ tooltip_placement }}" data-bs-toggle="tooltip" > {{ render_inner_html(icon,
+text) }}
+ {% endmacro %} {% macro render_js_button(javascript, tooltip=None,
+tooltip_placement="bottom", icon=None, text=None, label=None, classes="") %}
+% if tooltip %}title="{{ translate(tooltip) }}"{% endif %} data-bs-placement="{
+{ tooltip_placement }}" data-bs-toggle="tooltip" > {{ render_inner_html(icon,
+text) }}  {% endmacro %} {% macro render_button_group(buttons, icon,
+tooltip=None, label=None, classes="") %} {# A bootstrap dropdown #} {#
+Bootstrap dropdown ref: https://getbootstrap.com/docs/5.2/components/dropdowns/
+#}
 
-    * {%- for button in buttons %}
-    * {{ render_funcs[button.pop("type")](**button) }}
+    * {%- for button in buttons %} {% set btype = button.get("type") %} {% set
+      bopts = button.copy() %} {% set _ = bopts.pop("type") %}
+    * {{ render_funcs[btype](classes="dropdown-item", tooltip_placement="left",
+      **bopts) }}
     * {% endfor %}
 {% endmacro %} {%- set render_funcs = { "group" : render_button_group,
-"javascript" : render_js_button, "link": render_link_button, "input_label":
-render_label_input_button, } -%}
+"javascript" : render_js_button, "link": render_link_button, } -%}
```

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_binder.svg` & `tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_colab.png` & `tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_deepnote.svg` & `tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_jupyterhub.svg` & `tskit_book_theme-1.0.1/src/tskit_book_theme/theme/tskit_book_theme/static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/tests/sites/base/Makefile` & `tskit_book_theme-1.0.1/tests/sites/base/Makefile`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/tests/sites/base/conf.py` & `tskit_book_theme-1.0.1/tests/sites/base/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ["myst_nb", "sphinx_thebe"]
-html_theme = "tskit_book_theme"
+html_theme = "sphinx_book_theme"
 html_copy_source = True
 html_sourcelink_suffix = ""
-jupyter_execute_notebooks = "auto"
+nb_execution_mode = "auto"
 
 # Base options, we can add other key/vals later
 html_theme_options = {
     "path_to_docs": "TESTPATH",
-    "repository_url": "https://github.com/benjeffery/tskit-book-theme",
+    "repository_url": "https://github.com/executablebooks/sphinx-book-theme",
     # "repository_branch": "master",  # Not using this, should default to master
     "launch_buttons": {
         "binderhub_url": "https://mybinder.org",
         "jupyterhub_url": "https://datahub.berkeley.edu",
         "colab_url": "https://colab.research.google.com",
         "deepnote_url": "https://deepnote.com",
         "notebook_interface": "jupyterlab",
```

### Comparing `tskit_book_theme-0.3.2/tests/sites/base/section1/ntbk.ipynb` & `tskit_book_theme-1.0.1/tests/sites/base/section1/ntbk.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['pygments_lexer']}}"}*

```diff
@@ -36,14 +36,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
             "version": "3.8.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `tskit_book_theme-0.3.2/tests/sites/base/section1/ntbk_julia.ipynb` & `tskit_book_theme-1.0.1/tests/sites/base/section1/ntbk_julia.ipynb`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/tests/sites/base/section1/ntbk_octave.ipynb` & `tskit_book_theme-1.0.1/tests/sites/base/section1/ntbk_octave.ipynb`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/tests/sites/parallel-build/Makefile` & `tskit_book_theme-1.0.1/tests/sites/parallel-build/Makefile`

 * *Files identical despite different names*

### Comparing `tskit_book_theme-0.3.2/tests/test_build/build__header-article.html` & `tskit_book_theme-1.0.1/tests/test_build/header__repo-buttons--all-on.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,276 +1,251 @@
 00000000: 3c64 6976 2063 6c61 7373 3d22 6865 6164  <div class="head
-00000010: 6572 2d61 7274 6963 6c65 2072 6f77 2073  er-article row s
-00000020: 7469 636b 792d 746f 7020 6e6f 7072 696e  ticky-top noprin
-00000030: 7422 3e0a 203c 6469 7620 636c 6173 733d  t">. <div class=
-00000040: 2263 6f6c 2070 792d 3120 642d 666c 6578  "col py-1 d-flex
-00000050: 2068 6561 6465 722d 6172 7469 636c 652d   header-article-
-00000060: 6d61 696e 223e 0a20 203c 6469 7620 636c  main">.  <div cl
-00000070: 6173 733d 2268 6561 6465 722d 6172 7469  ass="header-arti
-00000080: 636c 655f 5f6c 6566 7422 3e0a 2020 203c  cle__left">.   <
-00000090: 6c61 6265 6c20 636c 6173 733d 2268 6561  label class="hea
-000000a0: 6465 7262 746e 2220 6461 7461 2d70 6c61  derbtn" data-pla
-000000b0: 6365 6d65 6e74 3d22 7269 6768 7422 2064  cement="right" d
-000000c0: 6174 612d 746f 6767 6c65 3d22 746f 6f6c  ata-toggle="tool
-000000d0: 7469 7022 2066 6f72 3d22 5f5f 6e61 7669  tip" for="__navi
-000000e0: 6761 7469 6f6e 2220 7469 746c 653d 2254  gation" title="T
-000000f0: 6f67 676c 6520 6e61 7669 6761 7469 6f6e  oggle navigation
-00000100: 223e 0a20 2020 203c 7370 616e 2063 6c61  ">.    <span cla
-00000110: 7373 3d22 6865 6164 6572 6274 6e5f 5f69  ss="headerbtn__i
-00000120: 636f 6e2d 636f 6e74 6169 6e65 7222 3e0a  con-container">.
-00000130: 2020 2020 203c 6920 636c 6173 733d 2266       <i class="f
-00000140: 6173 2066 612d 6261 7273 223e 0a20 2020  as fa-bars">.   
-00000150: 2020 3c2f 693e 0a20 2020 203c 2f73 7061    </i>.    </spa
-00000160: 6e3e 0a20 2020 3c2f 6c61 6265 6c3e 0a20  n>.   </label>. 
-00000170: 203c 2f64 6976 3e0a 2020 3c64 6976 2063   </div>.  <div c
-00000180: 6c61 7373 3d22 6865 6164 6572 2d61 7274  lass="header-art
-00000190: 6963 6c65 5f5f 7269 6768 7422 3e0a 2020  icle__right">.  
-000001a0: 203c 6469 7620 636c 6173 733d 226d 656e   <div class="men
-000001b0: 752d 6472 6f70 646f 776e 206d 656e 752d  u-dropdown menu-
-000001c0: 6472 6f70 646f 776e 2d6c 6175 6e63 682d  dropdown-launch-
-000001d0: 6275 7474 6f6e 7322 3e0a 2020 2020 3c62  buttons">.    <b
-000001e0: 7574 746f 6e20 6172 6961 2d6c 6162 656c  utton aria-label
-000001f0: 3d22 4c61 756e 6368 2069 6e74 6572 6163  ="Launch interac
-00000200: 7469 7665 2063 6f6e 7465 6e74 2220 636c  tive content" cl
-00000210: 6173 733d 2268 6561 6465 7262 746e 206d  ass="headerbtn m
-00000220: 656e 752d 6472 6f70 646f 776e 5f5f 7472  enu-dropdown__tr
-00000230: 6967 6765 7222 3e0a 2020 2020 203c 6920  igger">.     <i 
-00000240: 636c 6173 733d 2266 6173 2066 612d 726f  class="fas fa-ro
-00000250: 636b 6574 223e 0a20 2020 2020 3c2f 693e  cket">.     </i>
-00000260: 0a20 2020 203c 2f62 7574 746f 6e3e 0a20  .    </button>. 
-00000270: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-00000280: 656e 752d 6472 6f70 646f 776e 5f5f 636f  enu-dropdown__co
-00000290: 6e74 656e 7422 3e0a 2020 2020 203c 756c  ntent">.     <ul
-000002a0: 3e0a 2020 2020 2020 3c6c 693e 0a20 2020  >.      <li>.   
-000002b0: 2020 2020 3c61 2063 6c61 7373 3d22 6865      <a class="he
-000002c0: 6164 6572 6274 6e22 2064 6174 612d 706c  aderbtn" data-pl
-000002d0: 6163 656d 656e 743d 226c 6566 7422 2064  acement="left" d
-000002e0: 6174 612d 746f 6767 6c65 3d22 746f 6f6c  ata-toggle="tool
-000002f0: 7469 7022 2068 7265 663d 2268 7474 7073  tip" href="https
-00000300: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
-00000310: 7632 2f67 682f 6578 6563 7574 6162 6c65  v2/gh/executable
-00000320: 626f 6f6b 732f 7370 6869 6e78 2d62 6f6f  books/sphinx-boo
-00000330: 6b2d 7468 656d 652f 6d61 7374 6572 3f75  k-theme/master?u
-00000340: 726c 7061 7468 3d6c 6162 2f74 7265 652f  rlpath=lab/tree/
-00000350: 5445 5354 5041 5448 2f73 6563 7469 6f6e  TESTPATH/section
-00000360: 312f 6e74 626b 2e69 7079 6e62 2220 7469  1/ntbk.ipynb" ti
-00000370: 746c 653d 224c 6175 6e63 6820 6f6e 2042  tle="Launch on B
-00000380: 696e 6465 7222 3e0a 2020 2020 2020 2020  inder">.        
-00000390: 3c73 7061 6e20 636c 6173 733d 2268 6561  <span class="hea
-000003a0: 6465 7262 746e 5f5f 6963 6f6e 2d63 6f6e  derbtn__icon-con
-000003b0: 7461 696e 6572 223e 0a20 2020 2020 2020  tainer">.       
-000003c0: 2020 3c69 6d67 2073 7263 3d22 2e2e 2f5f    <img src="../_
-000003d0: 7374 6174 6963 2f69 6d61 6765 732f 6c6f  static/images/lo
-000003e0: 676f 5f62 696e 6465 722e 7376 6722 2f3e  go_binder.svg"/>
-000003f0: 0a20 2020 2020 2020 203c 2f73 7061 6e3e  .        </span>
-00000400: 0a20 2020 2020 2020 203c 7370 616e 2063  .        <span c
-00000410: 6c61 7373 3d22 6865 6164 6572 6274 6e5f  lass="headerbtn_
-00000420: 5f74 6578 742d 636f 6e74 6169 6e65 7222  _text-container"
-00000430: 3e0a 2020 2020 2020 2020 2042 696e 6465  >.         Binde
-00000440: 720a 2020 2020 2020 2020 3c2f 7370 616e  r.        </span
-00000450: 3e0a 2020 2020 2020 203c 2f61 3e0a 2020  >.       </a>.  
-00000460: 2020 2020 3c2f 6c69 3e0a 2020 2020 2020      </li>.      
-00000470: 3c6c 693e 0a20 2020 2020 2020 3c61 2063  <li>.       <a c
-00000480: 6c61 7373 3d22 6865 6164 6572 6274 6e22  lass="headerbtn"
-00000490: 2064 6174 612d 706c 6163 656d 656e 743d   data-placement=
-000004a0: 226c 6566 7422 2064 6174 612d 746f 6767  "left" data-togg
-000004b0: 6c65 3d22 746f 6f6c 7469 7022 2068 7265  le="tooltip" hre
-000004c0: 663d 2268 7474 7073 3a2f 2f64 6174 6168  f="https://datah
-000004d0: 7562 2e62 6572 6b65 6c65 792e 6564 752f  ub.berkeley.edu/
-000004e0: 6875 622f 7573 6572 2d72 6564 6972 6563  hub/user-redirec
-000004f0: 742f 6769 742d 7075 6c6c 3f72 6570 6f3d  t/git-pull?repo=
-00000500: 6874 7470 7325 3341 2f2f 6769 7468 7562  https%3A//github
-00000510: 2e63 6f6d 2f65 7865 6375 7461 626c 6562  .com/executableb
-00000520: 6f6f 6b73 2f73 7068 696e 782d 626f 6f6b  ooks/sphinx-book
-00000530: 2d74 6865 6d65 2661 6d70 3b75 726c 7061  -theme&amp;urlpa
-00000540: 7468 3d6c 6162 2f74 7265 652f 7370 6869  th=lab/tree/sphi
-00000550: 6e78 2d62 6f6f 6b2d 7468 656d 652f 5445  nx-book-theme/TE
-00000560: 5354 5041 5448 2f73 6563 7469 6f6e 312f  STPATH/section1/
-00000570: 6e74 626b 2e69 7079 6e62 2661 6d70 3b62  ntbk.ipynb&amp;b
-00000580: 7261 6e63 683d 6d61 7374 6572 2220 7469  ranch=master" ti
-00000590: 746c 653d 224c 6175 6e63 6820 6f6e 204a  tle="Launch on J
-000005a0: 7570 7974 6572 4875 6222 3e0a 2020 2020  upyterHub">.    
-000005b0: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-000005c0: 2268 6561 6465 7262 746e 5f5f 6963 6f6e  "headerbtn__icon
-000005d0: 2d63 6f6e 7461 696e 6572 223e 0a20 2020  -container">.   
-000005e0: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
-000005f0: 2e2e 2f5f 7374 6174 6963 2f69 6d61 6765  ../_static/image
-00000600: 732f 6c6f 676f 5f6a 7570 7974 6572 6875  s/logo_jupyterhu
-00000610: 622e 7376 6722 2f3e 0a20 2020 2020 2020  b.svg"/>.       
-00000620: 203c 2f73 7061 6e3e 0a20 2020 2020 2020   </span>.       
-00000630: 203c 7370 616e 2063 6c61 7373 3d22 6865   <span class="he
-00000640: 6164 6572 6274 6e5f 5f74 6578 742d 636f  aderbtn__text-co
-00000650: 6e74 6169 6e65 7222 3e0a 2020 2020 2020  ntainer">.      
-00000660: 2020 204a 7570 7974 6572 4875 620a 2020     JupyterHub.  
-00000670: 2020 2020 2020 3c2f 7370 616e 3e0a 2020        </span>.  
-00000680: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
-00000690: 3c2f 6c69 3e0a 2020 2020 2020 3c6c 693e  </li>.      <li>
-000006a0: 0a20 2020 2020 2020 3c61 2063 6c61 7373  .       <a class
-000006b0: 3d22 6865 6164 6572 6274 6e22 2064 6174  ="headerbtn" dat
-000006c0: 612d 706c 6163 656d 656e 743d 226c 6566  a-placement="lef
-000006d0: 7422 2064 6174 612d 746f 6767 6c65 3d22  t" data-toggle="
-000006e0: 746f 6f6c 7469 7022 2068 7265 663d 2268  tooltip" href="h
-000006f0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00000700: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00000710: 2f67 6974 6875 622f 6578 6563 7574 6162  /github/executab
-00000720: 6c65 626f 6f6b 732f 7370 6869 6e78 2d62  lebooks/sphinx-b
-00000730: 6f6f 6b2d 7468 656d 652f 626c 6f62 2f6d  ook-theme/blob/m
-00000740: 6173 7465 722f 5445 5354 5041 5448 2f73  aster/TESTPATH/s
-00000750: 6563 7469 6f6e 312f 6e74 626b 2e69 7079  ection1/ntbk.ipy
-00000760: 6e62 2220 7469 746c 653d 224c 6175 6e63  nb" title="Launc
-00000770: 6820 6f6e 2043 6f6c 6162 223e 0a20 2020  h on Colab">.   
-00000780: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-00000790: 3d22 6865 6164 6572 6274 6e5f 5f69 636f  ="headerbtn__ico
-000007a0: 6e2d 636f 6e74 6169 6e65 7222 3e0a 2020  n-container">.  
-000007b0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-000007c0: 222e 2e2f 5f73 7461 7469 632f 696d 6167  "../_static/imag
-000007d0: 6573 2f6c 6f67 6f5f 636f 6c61 622e 706e  es/logo_colab.pn
-000007e0: 6722 2f3e 0a20 2020 2020 2020 203c 2f73  g"/>.        </s
-000007f0: 7061 6e3e 0a20 2020 2020 2020 203c 7370  pan>.        <sp
-00000800: 616e 2063 6c61 7373 3d22 6865 6164 6572  an class="header
-00000810: 6274 6e5f 5f74 6578 742d 636f 6e74 6169  btn__text-contai
-00000820: 6e65 7222 3e0a 2020 2020 2020 2020 2043  ner">.         C
-00000830: 6f6c 6162 0a20 2020 2020 2020 203c 2f73  olab.        </s
-00000840: 7061 6e3e 0a20 2020 2020 2020 3c2f 613e  pan>.       </a>
-00000850: 0a20 2020 2020 203c 2f6c 693e 0a20 2020  .      </li>.   
-00000860: 2020 203c 6c69 3e0a 2020 2020 2020 203c     <li>.       <
-00000870: 6120 636c 6173 733d 2268 6561 6465 7262  a class="headerb
-00000880: 746e 2220 6461 7461 2d70 6c61 6365 6d65  tn" data-placeme
-00000890: 6e74 3d22 6c65 6674 2220 6461 7461 2d74  nt="left" data-t
-000008a0: 6f67 676c 653d 2274 6f6f 6c74 6970 2220  oggle="tooltip" 
-000008b0: 6872 6566 3d22 6874 7470 733a 2f2f 6465  href="https://de
-000008c0: 6570 6e6f 7465 2e63 6f6d 2f6c 6175 6e63  epnote.com/launc
-000008d0: 683f 7572 6c3d 6874 7470 7325 3341 2532  h?url=https%3A%2
-000008e0: 4625 3246 6769 7468 7562 2e63 6f6d 2532  F%2Fgithub.com%2
-000008f0: 4665 7865 6375 7461 626c 6562 6f6f 6b73  Fexecutablebooks
-00000900: 2532 4673 7068 696e 782d 626f 6f6b 2d74  %2Fsphinx-book-t
-00000910: 6865 6d65 2532 4662 6c6f 6225 3246 6d61  heme%2Fblob%2Fma
-00000920: 7374 6572 2532 4654 4553 5450 4154 482f  ster%2FTESTPATH/
-00000930: 7365 6374 696f 6e31 2f6e 7462 6b2e 6970  section1/ntbk.ip
-00000940: 796e 6222 2074 6974 6c65 3d22 4c61 756e  ynb" title="Laun
-00000950: 6368 206f 6e20 4465 6570 6e6f 7465 223e  ch on Deepnote">
-00000960: 0a20 2020 2020 2020 203c 7370 616e 2063  .        <span c
-00000970: 6c61 7373 3d22 6865 6164 6572 6274 6e5f  lass="headerbtn_
-00000980: 5f69 636f 6e2d 636f 6e74 6169 6e65 7222  _icon-container"
-00000990: 3e0a 2020 2020 2020 2020 203c 696d 6720  >.         <img 
-000009a0: 7372 633d 222e 2e2f 5f73 7461 7469 632f  src="../_static/
-000009b0: 696d 6167 6573 2f6c 6f67 6f5f 6465 6570  images/logo_deep
-000009c0: 6e6f 7465 2e73 7667 222f 3e0a 2020 2020  note.svg"/>.    
-000009d0: 2020 2020 3c2f 7370 616e 3e0a 2020 2020      </span>.    
-000009e0: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-000009f0: 2268 6561 6465 7262 746e 5f5f 7465 7874  "headerbtn__text
-00000a00: 2d63 6f6e 7461 696e 6572 223e 0a20 2020  -container">.   
-00000a10: 2020 2020 2020 4465 6570 6e6f 7465 0a20        Deepnote. 
-00000a20: 2020 2020 2020 203c 2f73 7061 6e3e 0a20         </span>. 
-00000a30: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
-00000a40: 203c 2f6c 693e 0a20 2020 2020 203c 6c69   </li>.      <li
-00000a50: 3e0a 2020 2020 2020 203c 6275 7474 6f6e  >.       <button
-00000a60: 2063 6c61 7373 3d22 6865 6164 6572 6274   class="headerbt
-00000a70: 6e20 6865 6164 6572 6274 6e2d 6c61 756e  n headerbtn-laun
-00000a80: 6368 2d74 6865 6265 2220 6461 7461 2d70  ch-thebe" data-p
-00000a90: 6c61 6365 6d65 6e74 3d22 6c65 6674 2220  lacement="left" 
-00000aa0: 6461 7461 2d74 6f67 676c 653d 2274 6f6f  data-toggle="too
-00000ab0: 6c74 6970 2220 6f6e 636c 6963 6b3d 2269  ltip" onclick="i
-00000ac0: 6e69 7454 6865 6265 5342 5428 2922 2074  nitThebeSBT()" t
-00000ad0: 6974 6c65 3d22 4c61 756e 6368 2054 6865  itle="Launch The
-00000ae0: 6265 223e 0a20 2020 2020 2020 203c 7370  be">.        <sp
-00000af0: 616e 2063 6c61 7373 3d22 6865 6164 6572  an class="header
-00000b00: 6274 6e5f 5f69 636f 6e2d 636f 6e74 6169  btn__icon-contai
-00000b10: 6e65 7222 3e0a 2020 2020 2020 2020 203c  ner">.         <
-00000b20: 6920 636c 6173 733d 2266 6173 2066 612d  i class="fas fa-
-00000b30: 706c 6179 223e 0a20 2020 2020 2020 2020  play">.         
-00000b40: 3c2f 693e 0a20 2020 2020 2020 203c 2f73  </i>.        </s
-00000b50: 7061 6e3e 0a20 2020 2020 2020 203c 7370  pan>.        <sp
-00000b60: 616e 2063 6c61 7373 3d22 6865 6164 6572  an class="header
-00000b70: 6274 6e5f 5f74 6578 742d 636f 6e74 6169  btn__text-contai
-00000b80: 6e65 7222 3e0a 2020 2020 2020 2020 204c  ner">.         L
-00000b90: 6976 6520 436f 6465 0a20 2020 2020 2020  ive Code.       
-00000ba0: 203c 2f73 7061 6e3e 0a20 2020 2020 2020   </span>.       
-00000bb0: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
-00000bc0: 3c2f 6c69 3e0a 2020 2020 203c 2f75 6c3e  </li>.     </ul>
-00000bd0: 0a20 2020 203c 2f64 6976 3e0a 2020 203c  .    </div>.   <
-00000be0: 2f64 6976 3e0a 2020 203c 6275 7474 6f6e  /div>.   <button
-00000bf0: 2063 6c61 7373 3d22 6865 6164 6572 6274   class="headerbt
-00000c00: 6e22 2064 6174 612d 706c 6163 656d 656e  n" data-placemen
-00000c10: 743d 2262 6f74 746f 6d22 2064 6174 612d  t="bottom" data-
-00000c20: 746f 6767 6c65 3d22 746f 6f6c 7469 7022  toggle="tooltip"
-00000c30: 206f 6e63 6c69 636b 3d22 746f 6767 6c65   onclick="toggle
-00000c40: 4675 6c6c 5363 7265 656e 2829 2220 7469  FullScreen()" ti
-00000c50: 746c 653d 2246 756c 6c73 6372 6565 6e20  tle="Fullscreen 
-00000c60: 6d6f 6465 223e 0a20 2020 203c 7370 616e  mode">.    <span
-00000c70: 2063 6c61 7373 3d22 6865 6164 6572 6274   class="headerbt
-00000c80: 6e5f 5f69 636f 6e2d 636f 6e74 6169 6e65  n__icon-containe
-00000c90: 7222 3e0a 2020 2020 203c 6920 636c 6173  r">.     <i clas
-00000ca0: 733d 2266 6173 2066 612d 6578 7061 6e64  s="fas fa-expand
-00000cb0: 223e 0a20 2020 2020 3c2f 693e 0a20 2020  ">.     </i>.   
-00000cc0: 203c 2f73 7061 6e3e 0a20 2020 3c2f 6275   </span>.   </bu
-00000cd0: 7474 6f6e 3e0a 2020 203c 6469 7620 636c  tton>.   <div cl
-00000ce0: 6173 733d 226d 656e 752d 6472 6f70 646f  ass="menu-dropdo
-00000cf0: 776e 206d 656e 752d 6472 6f70 646f 776e  wn menu-dropdown
-00000d00: 2d64 6f77 6e6c 6f61 642d 6275 7474 6f6e  -download-button
-00000d10: 7322 3e0a 2020 2020 3c62 7574 746f 6e20  s">.    <button 
-00000d20: 6172 6961 2d6c 6162 656c 3d22 446f 776e  aria-label="Down
-00000d30: 6c6f 6164 2074 6869 7320 7061 6765 2220  load this page" 
-00000d40: 636c 6173 733d 2268 6561 6465 7262 746e  class="headerbtn
-00000d50: 206d 656e 752d 6472 6f70 646f 776e 5f5f   menu-dropdown__
-00000d60: 7472 6967 6765 7222 3e0a 2020 2020 203c  trigger">.     <
-00000d70: 6920 636c 6173 733d 2266 6173 2066 612d  i class="fas fa-
-00000d80: 646f 776e 6c6f 6164 223e 0a20 2020 2020  download">.     
-00000d90: 3c2f 693e 0a20 2020 203c 2f62 7574 746f  </i>.    </butto
-00000da0: 6e3e 0a20 2020 203c 6469 7620 636c 6173  n>.    <div clas
-00000db0: 733d 226d 656e 752d 6472 6f70 646f 776e  s="menu-dropdown
-00000dc0: 5f5f 636f 6e74 656e 7422 3e0a 2020 2020  __content">.    
-00000dd0: 203c 756c 3e0a 2020 2020 2020 3c6c 693e   <ul>.      <li>
-00000de0: 0a20 2020 2020 2020 3c61 2063 6c61 7373  .       <a class
-00000df0: 3d22 6865 6164 6572 6274 6e22 2064 6174  ="headerbtn" dat
-00000e00: 612d 706c 6163 656d 656e 743d 226c 6566  a-placement="lef
-00000e10: 7422 2064 6174 612d 746f 6767 6c65 3d22  t" data-toggle="
-00000e20: 746f 6f6c 7469 7022 2068 7265 663d 222e  tooltip" href=".
-00000e30: 2e2f 5f73 6f75 7263 6573 2f73 6563 7469  ./_sources/secti
-00000e40: 6f6e 312f 6e74 626b 2e69 7079 6e62 2220  on1/ntbk.ipynb" 
-00000e50: 7469 746c 653d 2244 6f77 6e6c 6f61 6420  title="Download 
-00000e60: 736f 7572 6365 2066 696c 6522 3e0a 2020  source file">.  
-00000e70: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00000e80: 733d 2268 6561 6465 7262 746e 5f5f 6963  s="headerbtn__ic
-00000e90: 6f6e 2d63 6f6e 7461 696e 6572 223e 0a20  on-container">. 
-00000ea0: 2020 2020 2020 2020 3c69 2063 6c61 7373          <i class
-00000eb0: 3d22 6661 7320 6661 2d66 696c 6522 3e0a  ="fas fa-file">.
-00000ec0: 2020 2020 2020 2020 203c 2f69 3e0a 2020           </i>.  
-00000ed0: 2020 2020 2020 3c2f 7370 616e 3e0a 2020        </span>.  
-00000ee0: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00000ef0: 733d 2268 6561 6465 7262 746e 5f5f 7465  s="headerbtn__te
-00000f00: 7874 2d63 6f6e 7461 696e 6572 223e 0a20  xt-container">. 
-00000f10: 2020 2020 2020 2020 2e69 7079 6e62 0a20          .ipynb. 
-00000f20: 2020 2020 2020 203c 2f73 7061 6e3e 0a20         </span>. 
-00000f30: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
-00000f40: 203c 2f6c 693e 0a20 2020 2020 203c 6c69   </li>.      <li
-00000f50: 3e0a 2020 2020 2020 203c 6275 7474 6f6e  >.       <button
-00000f60: 2063 6c61 7373 3d22 6865 6164 6572 6274   class="headerbt
-00000f70: 6e22 2064 6174 612d 706c 6163 656d 656e  n" data-placemen
-00000f80: 743d 226c 6566 7422 2064 6174 612d 746f  t="left" data-to
-00000f90: 6767 6c65 3d22 746f 6f6c 7469 7022 206f  ggle="tooltip" o
-00000fa0: 6e63 6c69 636b 3d22 7072 696e 7450 6466  nclick="printPdf
-00000fb0: 2874 6869 7329 2220 7469 746c 653d 2250  (this)" title="P
-00000fc0: 7269 6e74 2074 6f20 5044 4622 3e0a 2020  rint to PDF">.  
-00000fd0: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00000fe0: 733d 2268 6561 6465 7262 746e 5f5f 6963  s="headerbtn__ic
-00000ff0: 6f6e 2d63 6f6e 7461 696e 6572 223e 0a20  on-container">. 
-00001000: 2020 2020 2020 2020 3c69 2063 6c61 7373          <i class
-00001010: 3d22 6661 7320 6661 2d66 696c 652d 7064  ="fas fa-file-pd
-00001020: 6622 3e0a 2020 2020 2020 2020 203c 2f69  f">.         </i
-00001030: 3e0a 2020 2020 2020 2020 3c2f 7370 616e  >.        </span
-00001040: 3e0a 2020 2020 2020 2020 3c73 7061 6e20  >.        <span 
-00001050: 636c 6173 733d 2268 6561 6465 7262 746e  class="headerbtn
-00001060: 5f5f 7465 7874 2d63 6f6e 7461 696e 6572  __text-container
-00001070: 223e 0a20 2020 2020 2020 2020 2e70 6466  ">.         .pdf
-00001080: 0a20 2020 2020 2020 203c 2f73 7061 6e3e  .        </span>
-00001090: 0a20 2020 2020 2020 3c2f 6275 7474 6f6e  .       </button
-000010a0: 3e0a 2020 2020 2020 3c2f 6c69 3e0a 2020  >.      </li>.  
-000010b0: 2020 203c 2f75 6c3e 0a20 2020 203c 2f64     </ul>.    </d
-000010c0: 6976 3e0a 2020 203c 2f64 6976 3e0a 2020  iv>.   </div>.  
-000010d0: 3c2f 6469 763e 0a20 3c2f 6469 763e 0a20  </div>. </div>. 
-000010e0: 3c21 2d2d 2054 6162 6c65 206f 6620 636f  <!-- Table of co
-000010f0: 6e74 656e 7473 202d 2d3e 0a20 3c64 6976  ntents -->. <div
-00001100: 2063 6c61 7373 3d22 636f 6c2d 6d64 2d33   class="col-md-3
-00001110: 2062 642d 746f 6320 7368 6f77 206e 6f70   bd-toc show nop
-00001120: 7269 6e74 223e 0a20 3c2f 6469 763e 0a3c  rint">. </div>.<
-00001130: 2f64 6976 3e0a                           /div>.
+00000010: 6572 2d61 7274 6963 6c65 2d69 7465 6d73  er-article-items
+00000020: 5f5f 656e 6422 3e0a 203c 6469 7620 636c  __end">. <div cl
+00000030: 6173 733d 2268 6561 6465 722d 6172 7469  ass="header-arti
+00000040: 636c 652d 6974 656d 223e 0a20 203c 6469  cle-item">.  <di
+00000050: 7620 636c 6173 733d 2261 7274 6963 6c65  v class="article
+00000060: 2d68 6561 6465 722d 6275 7474 6f6e 7322  -header-buttons"
+00000070: 3e0a 2020 203c 6469 7620 636c 6173 733d  >.   <div class=
+00000080: 2264 726f 7064 6f77 6e20 6472 6f70 646f  "dropdown dropdo
+00000090: 776e 2d73 6f75 7263 652d 6275 7474 6f6e  wn-source-button
+000000a0: 7322 3e0a 2020 2020 3c62 7574 746f 6e20  s">.    <button 
+000000b0: 6172 6961 2d65 7870 616e 6465 643d 2266  aria-expanded="f
+000000c0: 616c 7365 2220 6172 6961 2d6c 6162 656c  alse" aria-label
+000000d0: 3d22 536f 7572 6365 2072 6570 6f73 6974  ="Source reposit
+000000e0: 6f72 6965 7322 2063 6c61 7373 3d22 6274  ories" class="bt
+000000f0: 6e20 6472 6f70 646f 776e 2d74 6f67 676c  n dropdown-toggl
+00000100: 6522 2064 6174 612d 6273 2d74 6f67 676c  e" data-bs-toggl
+00000110: 653d 2264 726f 7064 6f77 6e22 2074 7970  e="dropdown" typ
+00000120: 653d 2262 7574 746f 6e22 3e0a 2020 2020  e="button">.    
+00000130: 203c 6920 636c 6173 733d 2266 6162 2066   <i class="fab f
+00000140: 612d 6769 7468 7562 223e 0a20 2020 2020  a-github">.     
+00000150: 3c2f 693e 0a20 2020 203c 2f62 7574 746f  </i>.    </butto
+00000160: 6e3e 0a20 2020 203c 756c 2063 6c61 7373  n>.    <ul class
+00000170: 3d22 6472 6f70 646f 776e 2d6d 656e 7522  ="dropdown-menu"
+00000180: 3e0a 2020 2020 203c 6c69 3e0a 2020 2020  >.     <li>.    
+00000190: 2020 3c61 2063 6c61 7373 3d22 6274 6e20    <a class="btn 
+000001a0: 6274 6e2d 736d 2062 746e 2d73 6f75 7263  btn-sm btn-sourc
+000001b0: 652d 7265 706f 7369 746f 7279 2d62 7574  e-repository-but
+000001c0: 746f 6e20 6472 6f70 646f 776e 2d69 7465  ton dropdown-ite
+000001d0: 6d22 2064 6174 612d 6273 2d70 6c61 6365  m" data-bs-place
+000001e0: 6d65 6e74 3d22 6c65 6674 2220 6461 7461  ment="left" data
+000001f0: 2d62 732d 746f 6767 6c65 3d22 746f 6f6c  -bs-toggle="tool
+00000200: 7469 7022 2068 7265 663d 2268 7474 7073  tip" href="https
+00000210: 3a2f 2f67 6974 6875 622e 636f 6d2f 6578  ://github.com/ex
+00000220: 6563 7574 6162 6c65 626f 6f6b 732f 7370  ecutablebooks/sp
+00000230: 6869 6e78 2d62 6f6f 6b2d 7468 656d 6522  hinx-book-theme"
+00000240: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000250: 2074 6974 6c65 3d22 536f 7572 6365 2072   title="Source r
+00000260: 6570 6f73 6974 6f72 7922 3e0a 2020 2020  epository">.    
+00000270: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+00000280: 6274 6e5f 5f69 636f 6e2d 636f 6e74 6169  btn__icon-contai
+00000290: 6e65 7222 3e0a 2020 2020 2020 2020 3c69  ner">.        <i
+000002a0: 2063 6c61 7373 3d22 6661 6220 6661 2d67   class="fab fa-g
+000002b0: 6974 6875 6222 3e0a 2020 2020 2020 2020  ithub">.        
+000002c0: 3c2f 693e 0a20 2020 2020 2020 3c2f 7370  </i>.       </sp
+000002d0: 616e 3e0a 2020 2020 2020 203c 7370 616e  an>.       <span
+000002e0: 2063 6c61 7373 3d22 6274 6e5f 5f74 6578   class="btn__tex
+000002f0: 742d 636f 6e74 6169 6e65 7222 3e0a 2020  t-container">.  
+00000300: 2020 2020 2020 5265 706f 7369 746f 7279        Repository
+00000310: 0a20 2020 2020 2020 3c2f 7370 616e 3e0a  .       </span>.
+00000320: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
+00000330: 3c2f 6c69 3e0a 2020 2020 203c 6c69 3e0a  </li>.     <li>.
+00000340: 2020 2020 2020 3c61 2063 6c61 7373 3d22        <a class="
+00000350: 6274 6e20 6274 6e2d 736d 2062 746e 2d73  btn btn-sm btn-s
+00000360: 6f75 7263 652d 6564 6974 2d62 7574 746f  ource-edit-butto
+00000370: 6e20 6472 6f70 646f 776e 2d69 7465 6d22  n dropdown-item"
+00000380: 2064 6174 612d 6273 2d70 6c61 6365 6d65   data-bs-placeme
+00000390: 6e74 3d22 6c65 6674 2220 6461 7461 2d62  nt="left" data-b
+000003a0: 732d 746f 6767 6c65 3d22 746f 6f6c 7469  s-toggle="toolti
+000003b0: 7022 2068 7265 663d 2268 7474 7073 3a2f  p" href="https:/
+000003c0: 2f67 6974 6875 622e 636f 6d2f 6578 6563  /github.com/exec
+000003d0: 7574 6162 6c65 626f 6f6b 732f 7370 6869  utablebooks/sphi
+000003e0: 6e78 2d62 6f6f 6b2d 7468 656d 652f 6564  nx-book-theme/ed
+000003f0: 6974 2f6d 6169 6e2f 7365 6374 696f 6e31  it/main/section1
+00000400: 2f6e 7462 6b2e 6970 796e 6222 2074 6172  /ntbk.ipynb" tar
+00000410: 6765 743d 225f 626c 616e 6b22 2074 6974  get="_blank" tit
+00000420: 6c65 3d22 5375 6767 6573 7420 6564 6974  le="Suggest edit
+00000430: 223e 0a20 2020 2020 2020 3c73 7061 6e20  ">.       <span 
+00000440: 636c 6173 733d 2262 746e 5f5f 6963 6f6e  class="btn__icon
+00000450: 2d63 6f6e 7461 696e 6572 223e 0a20 2020  -container">.   
+00000460: 2020 2020 203c 6920 636c 6173 733d 2266       <i class="f
+00000470: 6173 2066 612d 7065 6e63 696c 2d61 6c74  as fa-pencil-alt
+00000480: 223e 0a20 2020 2020 2020 203c 2f69 3e0a  ">.        </i>.
+00000490: 2020 2020 2020 203c 2f73 7061 6e3e 0a20         </span>. 
+000004a0: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
+000004b0: 733d 2262 746e 5f5f 7465 7874 2d63 6f6e  s="btn__text-con
+000004c0: 7461 696e 6572 223e 0a20 2020 2020 2020  tainer">.       
+000004d0: 2053 7567 6765 7374 2065 6469 740a 2020   Suggest edit.  
+000004e0: 2020 2020 203c 2f73 7061 6e3e 0a20 2020       </span>.   
+000004f0: 2020 203c 2f61 3e0a 2020 2020 203c 2f6c     </a>.     </l
+00000500: 693e 0a20 2020 2020 3c6c 693e 0a20 2020  i>.     <li>.   
+00000510: 2020 203c 6120 636c 6173 733d 2262 746e     <a class="btn
+00000520: 2062 746e 2d73 6d20 6274 6e2d 736f 7572   btn-sm btn-sour
+00000530: 6365 2d69 7373 7565 732d 6275 7474 6f6e  ce-issues-button
+00000540: 2064 726f 7064 6f77 6e2d 6974 656d 2220   dropdown-item" 
+00000550: 6461 7461 2d62 732d 706c 6163 656d 656e  data-bs-placemen
+00000560: 743d 226c 6566 7422 2064 6174 612d 6273  t="left" data-bs
+00000570: 2d74 6f67 676c 653d 2274 6f6f 6c74 6970  -toggle="tooltip
+00000580: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+00000590: 6769 7468 7562 2e63 6f6d 2f65 7865 6375  github.com/execu
+000005a0: 7461 626c 6562 6f6f 6b73 2f73 7068 696e  tablebooks/sphin
+000005b0: 782d 626f 6f6b 2d74 6865 6d65 2f69 7373  x-book-theme/iss
+000005c0: 7565 732f 6e65 773f 7469 746c 653d 4973  ues/new?title=Is
+000005d0: 7375 6525 3230 6f6e 2532 3070 6167 6525  sue%20on%20page%
+000005e0: 3230 2532 4673 6563 7469 6f6e 312f 6e74  20%2Fsection1/nt
+000005f0: 626b 2e68 746d 6c26 616d 703b 626f 6479  bk.html&amp;body
+00000600: 3d59 6f75 7225 3230 6973 7375 6525 3230  =Your%20issue%20
+00000610: 636f 6e74 656e 7425 3230 6865 7265 2e22  content%20here."
+00000620: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000630: 2074 6974 6c65 3d22 4f70 656e 2061 6e20   title="Open an 
+00000640: 6973 7375 6522 3e0a 2020 2020 2020 203c  issue">.       <
+00000650: 7370 616e 2063 6c61 7373 3d22 6274 6e5f  span class="btn_
+00000660: 5f69 636f 6e2d 636f 6e74 6169 6e65 7222  _icon-container"
+00000670: 3e0a 2020 2020 2020 2020 3c69 2063 6c61  >.        <i cla
+00000680: 7373 3d22 6661 7320 6661 2d6c 6967 6874  ss="fas fa-light
+00000690: 6275 6c62 223e 0a20 2020 2020 2020 203c  bulb">.        <
+000006a0: 2f69 3e0a 2020 2020 2020 203c 2f73 7061  /i>.       </spa
+000006b0: 6e3e 0a20 2020 2020 2020 3c73 7061 6e20  n>.       <span 
+000006c0: 636c 6173 733d 2262 746e 5f5f 7465 7874  class="btn__text
+000006d0: 2d63 6f6e 7461 696e 6572 223e 0a20 2020  -container">.   
+000006e0: 2020 2020 204f 7065 6e20 6973 7375 650a       Open issue.
+000006f0: 2020 2020 2020 203c 2f73 7061 6e3e 0a20         </span>. 
+00000700: 2020 2020 203c 2f61 3e0a 2020 2020 203c       </a>.     <
+00000710: 2f6c 693e 0a20 2020 203c 2f75 6c3e 0a20  /li>.    </ul>. 
+00000720: 2020 3c2f 6469 763e 0a20 2020 3c64 6976    </div>.   <div
+00000730: 2063 6c61 7373 3d22 6472 6f70 646f 776e   class="dropdown
+00000740: 2064 726f 7064 6f77 6e2d 646f 776e 6c6f   dropdown-downlo
+00000750: 6164 2d62 7574 746f 6e73 223e 0a20 2020  ad-buttons">.   
+00000760: 203c 6275 7474 6f6e 2061 7269 612d 6578   <button aria-ex
+00000770: 7061 6e64 6564 3d22 6661 6c73 6522 2061  panded="false" a
+00000780: 7269 612d 6c61 6265 6c3d 2244 6f77 6e6c  ria-label="Downl
+00000790: 6f61 6420 7468 6973 2070 6167 6522 2063  oad this page" c
+000007a0: 6c61 7373 3d22 6274 6e20 6472 6f70 646f  lass="btn dropdo
+000007b0: 776e 2d74 6f67 676c 6522 2064 6174 612d  wn-toggle" data-
+000007c0: 6273 2d74 6f67 676c 653d 2264 726f 7064  bs-toggle="dropd
+000007d0: 6f77 6e22 2074 7970 653d 2262 7574 746f  own" type="butto
+000007e0: 6e22 3e0a 2020 2020 203c 6920 636c 6173  n">.     <i clas
+000007f0: 733d 2266 6173 2066 612d 646f 776e 6c6f  s="fas fa-downlo
+00000800: 6164 223e 0a20 2020 2020 3c2f 693e 0a20  ad">.     </i>. 
+00000810: 2020 203c 2f62 7574 746f 6e3e 0a20 2020     </button>.   
+00000820: 203c 756c 2063 6c61 7373 3d22 6472 6f70   <ul class="drop
+00000830: 646f 776e 2d6d 656e 7522 3e0a 2020 2020  down-menu">.    
+00000840: 203c 6c69 3e0a 2020 2020 2020 3c61 2063   <li>.      <a c
+00000850: 6c61 7373 3d22 6274 6e20 6274 6e2d 736d  lass="btn btn-sm
+00000860: 2062 746e 2d64 6f77 6e6c 6f61 642d 736f   btn-download-so
+00000870: 7572 6365 2d62 7574 746f 6e20 6472 6f70  urce-button drop
+00000880: 646f 776e 2d69 7465 6d22 2064 6174 612d  down-item" data-
+00000890: 6273 2d70 6c61 6365 6d65 6e74 3d22 6c65  bs-placement="le
+000008a0: 6674 2220 6461 7461 2d62 732d 746f 6767  ft" data-bs-togg
+000008b0: 6c65 3d22 746f 6f6c 7469 7022 2068 7265  le="tooltip" hre
+000008c0: 663d 222e 2e2f 5f73 6f75 7263 6573 2f73  f="../_sources/s
+000008d0: 6563 7469 6f6e 312f 6e74 626b 2e69 7079  ection1/ntbk.ipy
+000008e0: 6e62 2220 7461 7267 6574 3d22 5f62 6c61  nb" target="_bla
+000008f0: 6e6b 2220 7469 746c 653d 2244 6f77 6e6c  nk" title="Downl
+00000900: 6f61 6420 736f 7572 6365 2066 696c 6522  oad source file"
+00000910: 3e0a 2020 2020 2020 203c 7370 616e 2063  >.       <span c
+00000920: 6c61 7373 3d22 6274 6e5f 5f69 636f 6e2d  lass="btn__icon-
+00000930: 636f 6e74 6169 6e65 7222 3e0a 2020 2020  container">.    
+00000940: 2020 2020 3c69 2063 6c61 7373 3d22 6661      <i class="fa
+00000950: 7320 6661 2d66 696c 6522 3e0a 2020 2020  s fa-file">.    
+00000960: 2020 2020 3c2f 693e 0a20 2020 2020 2020      </i>.       
+00000970: 3c2f 7370 616e 3e0a 2020 2020 2020 203c  </span>.       <
+00000980: 7370 616e 2063 6c61 7373 3d22 6274 6e5f  span class="btn_
+00000990: 5f74 6578 742d 636f 6e74 6169 6e65 7222  _text-container"
+000009a0: 3e0a 2020 2020 2020 2020 2e69 7079 6e62  >.        .ipynb
+000009b0: 0a20 2020 2020 2020 3c2f 7370 616e 3e0a  .       </span>.
+000009c0: 2020 2020 2020 3c2f 613e 0a20 2020 2020        </a>.     
+000009d0: 3c2f 6c69 3e0a 2020 2020 203c 6c69 3e0a  </li>.     <li>.
+000009e0: 2020 2020 2020 3c62 7574 746f 6e20 636c        <button cl
+000009f0: 6173 733d 2262 746e 2062 746e 2d73 6d20  ass="btn btn-sm 
+00000a00: 6274 6e2d 646f 776e 6c6f 6164 2d70 6466  btn-download-pdf
+00000a10: 2d62 7574 746f 6e20 6472 6f70 646f 776e  -button dropdown
+00000a20: 2d69 7465 6d22 2064 6174 612d 6273 2d70  -item" data-bs-p
+00000a30: 6c61 6365 6d65 6e74 3d22 6c65 6674 2220  lacement="left" 
+00000a40: 6461 7461 2d62 732d 746f 6767 6c65 3d22  data-bs-toggle="
+00000a50: 746f 6f6c 7469 7022 206f 6e63 6c69 636b  tooltip" onclick
+00000a60: 3d22 7769 6e64 6f77 2e70 7269 6e74 2829  ="window.print()
+00000a70: 2220 7469 746c 653d 2250 7269 6e74 2074  " title="Print t
+00000a80: 6f20 5044 4622 3e0a 2020 2020 2020 203c  o PDF">.       <
+00000a90: 7370 616e 2063 6c61 7373 3d22 6274 6e5f  span class="btn_
+00000aa0: 5f69 636f 6e2d 636f 6e74 6169 6e65 7222  _icon-container"
+00000ab0: 3e0a 2020 2020 2020 2020 3c69 2063 6c61  >.        <i cla
+00000ac0: 7373 3d22 6661 7320 6661 2d66 696c 652d  ss="fas fa-file-
+00000ad0: 7064 6622 3e0a 2020 2020 2020 2020 3c2f  pdf">.        </
+00000ae0: 693e 0a20 2020 2020 2020 3c2f 7370 616e  i>.       </span
+00000af0: 3e0a 2020 2020 2020 203c 7370 616e 2063  >.       <span c
+00000b00: 6c61 7373 3d22 6274 6e5f 5f74 6578 742d  lass="btn__text-
+00000b10: 636f 6e74 6169 6e65 7222 3e0a 2020 2020  container">.    
+00000b20: 2020 2020 2e70 6466 0a20 2020 2020 2020      .pdf.       
+00000b30: 3c2f 7370 616e 3e0a 2020 2020 2020 3c2f  </span>.      </
+00000b40: 6275 7474 6f6e 3e0a 2020 2020 203c 2f6c  button>.     </l
+00000b50: 693e 0a20 2020 203c 2f75 6c3e 0a20 2020  i>.    </ul>.   
+00000b60: 3c2f 6469 763e 0a20 2020 3c62 7574 746f  </div>.   <butto
+00000b70: 6e20 636c 6173 733d 2262 746e 2062 746e  n class="btn btn
+00000b80: 2d73 6d20 6274 6e2d 6675 6c6c 7363 7265  -sm btn-fullscre
+00000b90: 656e 2d62 7574 746f 6e22 2064 6174 612d  en-button" data-
+00000ba0: 6273 2d70 6c61 6365 6d65 6e74 3d22 626f  bs-placement="bo
+00000bb0: 7474 6f6d 2220 6461 7461 2d62 732d 746f  ttom" data-bs-to
+00000bc0: 6767 6c65 3d22 746f 6f6c 7469 7022 206f  ggle="tooltip" o
+00000bd0: 6e63 6c69 636b 3d22 746f 6767 6c65 4675  nclick="toggleFu
+00000be0: 6c6c 5363 7265 656e 2829 2220 7469 746c  llScreen()" titl
+00000bf0: 653d 2246 756c 6c73 6372 6565 6e20 6d6f  e="Fullscreen mo
+00000c00: 6465 223e 0a20 2020 203c 7370 616e 2063  de">.    <span c
+00000c10: 6c61 7373 3d22 6274 6e5f 5f69 636f 6e2d  lass="btn__icon-
+00000c20: 636f 6e74 6169 6e65 7222 3e0a 2020 2020  container">.    
+00000c30: 203c 6920 636c 6173 733d 2266 6173 2066   <i class="fas f
+00000c40: 612d 6578 7061 6e64 223e 0a20 2020 2020  a-expand">.     
+00000c50: 3c2f 693e 0a20 2020 203c 2f73 7061 6e3e  </i>.    </span>
+00000c60: 0a20 2020 3c2f 6275 7474 6f6e 3e0a 2020  .   </button>.  
+00000c70: 203c 7363 7269 7074 3e0a 2020 2020 646f   <script>.    do
+00000c80: 6375 6d65 6e74 2e77 7269 7465 2860 0a20  cument.write(`. 
+00000c90: 203c 6275 7474 6f6e 2063 6c61 7373 3d22   <button class="
+00000ca0: 7468 656d 652d 7377 6974 6368 2d62 7574  theme-switch-but
+00000cb0: 746f 6e20 6274 6e20 6274 6e2d 736d 2062  ton btn btn-sm b
+00000cc0: 746e 2d6f 7574 6c69 6e65 2d70 7269 6d61  tn-outline-prima
+00000cd0: 7279 206e 6176 6261 722d 6274 6e20 726f  ry navbar-btn ro
+00000ce0: 756e 6465 642d 6369 7263 6c65 2220 7469  unded-circle" ti
+00000cf0: 746c 653d 226c 6967 6874 2f64 6172 6b22  tle="light/dark"
+00000d00: 2061 7269 612d 6c61 6265 6c3d 226c 6967   aria-label="lig
+00000d10: 6874 2f64 6172 6b22 2064 6174 612d 6273  ht/dark" data-bs
+00000d20: 2d70 6c61 6365 6d65 6e74 3d22 626f 7474  -placement="bott
+00000d30: 6f6d 2220 6461 7461 2d62 732d 746f 6767  om" data-bs-togg
+00000d40: 6c65 3d22 746f 6f6c 7469 7022 3e0a 2020  le="tooltip">.  
+00000d50: 2020 3c73 7061 6e20 636c 6173 733d 2274    <span class="t
+00000d60: 6865 6d65 2d73 7769 7463 6822 2064 6174  heme-switch" dat
+00000d70: 612d 6d6f 6465 3d22 6c69 6768 7422 3e3c  a-mode="light"><
+00000d80: 6920 636c 6173 733d 2266 612d 736f 6c69  i class="fa-soli
+00000d90: 6420 6661 2d73 756e 223e 3c2f 693e 3c2f  d fa-sun"></i></
+00000da0: 7370 616e 3e0a 2020 2020 3c73 7061 6e20  span>.    <span 
+00000db0: 636c 6173 733d 2274 6865 6d65 2d73 7769  class="theme-swi
+00000dc0: 7463 6822 2064 6174 612d 6d6f 6465 3d22  tch" data-mode="
+00000dd0: 6461 726b 223e 3c69 2063 6c61 7373 3d22  dark"><i class="
+00000de0: 6661 2d73 6f6c 6964 2066 612d 6d6f 6f6e  fa-solid fa-moon
+00000df0: 223e 3c2f 693e 3c2f 7370 616e 3e0a 2020  "></i></span>.  
+00000e00: 2020 3c73 7061 6e20 636c 6173 733d 2274    <span class="t
+00000e10: 6865 6d65 2d73 7769 7463 6822 2064 6174  heme-switch" dat
+00000e20: 612d 6d6f 6465 3d22 6175 746f 223e 3c69  a-mode="auto"><i
+00000e30: 2063 6c61 7373 3d22 6661 2d73 6f6c 6964   class="fa-solid
+00000e40: 2066 612d 6369 7263 6c65 2d68 616c 662d   fa-circle-half-
+00000e50: 7374 726f 6b65 223e 3c2f 693e 3c2f 7370  stroke"></i></sp
+00000e60: 616e 3e0a 2020 3c2f 6275 7474 6f6e 3e0a  an>.  </button>.
+00000e70: 6029 3b0a 2020 203c 2f73 6372 6970 743e  `);.   </script>
+00000e80: 0a20 2020 3c73 6372 6970 743e 0a20 2020  .   <script>.   
+00000e90: 2064 6f63 756d 656e 742e 7772 6974 6528   document.write(
+00000ea0: 600a 2020 3c62 7574 746f 6e20 636c 6173  `.  <button clas
+00000eb0: 733d 2262 746e 2062 746e 2d73 6d20 6e61  s="btn btn-sm na
+00000ec0: 7662 6172 2d62 746e 2073 6561 7263 682d  vbar-btn search-
+00000ed0: 6275 7474 6f6e 2073 6561 7263 682d 6275  button search-bu
+00000ee0: 7474 6f6e 5f5f 6275 7474 6f6e 2220 7469  tton__button" ti
+00000ef0: 746c 653d 2253 6561 7263 6822 2061 7269  tle="Search" ari
+00000f00: 612d 6c61 6265 6c3d 2253 6561 7263 6822  a-label="Search"
+00000f10: 2064 6174 612d 6273 2d70 6c61 6365 6d65   data-bs-placeme
+00000f20: 6e74 3d22 626f 7474 6f6d 2220 6461 7461  nt="bottom" data
+00000f30: 2d62 732d 746f 6767 6c65 3d22 746f 6f6c  -bs-toggle="tool
+00000f40: 7469 7022 3e0a 2020 2020 3c69 2063 6c61  tip">.    <i cla
+00000f50: 7373 3d22 6661 2d73 6f6c 6964 2066 612d  ss="fa-solid fa-
+00000f60: 6d61 676e 6966 7969 6e67 2d67 6c61 7373  magnifying-glass
+00000f70: 223e 3c2f 693e 0a20 203c 2f62 7574 746f  "></i>.  </butto
+00000f80: 6e3e 0a60 293b 0a20 2020 3c2f 7363 7269  n>.`);.   </scri
+00000f90: 7074 3e0a 2020 3c2f 6469 763e 0a20 3c2f  pt>.  </div>. </
+00000fa0: 6469 763e 0a3c 2f64 6976 3e0a            div>.</div>.
```

### Comparing `tskit_book_theme-0.3.2/tests/test_build/build__pagetoc--page-multipletitles.html` & `tskit_book_theme-1.0.1/tests/test_build/build__pagetoc--page-multipletitles.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-<div class="col-md-3 bd-toc show noprint">
- <div class="tocsection onthispage pt-5 pb-3">
-  <i class="fas fa-list">
-  </i>
-  Contents
- </div>
- <nav aria-label="Page" id="bd-toc-nav">
-  <ul class="visible nav section-nav flex-column">
-   <li class="toc-h1 nav-item toc-entry">
-    <a class="reference internal nav-link" href="#">
-     4.1. A page with multiple top-level titles
-    </a>
+<div class="bd-sidebar-secondary bd-toc">
+ <div class="sidebar-secondary-items sidebar-secondary__inner">
+  <div class="sidebar-secondary-item">
+   <div class="page-toc tocsection onthispage">
+    <i class="fa-solid fa-list">
+    </i>
+    Contents
+   </div>
+   <nav class="bd-toc-nav page-toc">
     <ul class="visible nav section-nav flex-column">
-     <li class="toc-h2 nav-item toc-entry">
-      <a class="reference internal nav-link" href="#a-sub-heading">
-       4.1.1. A sub-heading
+     <li class="toc-h1 nav-item toc-entry">
+      <a class="reference internal nav-link" href="#">
+       4.1. A page with multiple top-level titles
       </a>
+      <ul class="visible nav section-nav flex-column">
+       <li class="toc-h2 nav-item toc-entry">
+        <a class="reference internal nav-link" href="#a-sub-heading">
+         4.1.1. A sub-heading
+        </a>
+       </li>
+      </ul>
      </li>
-    </ul>
-   </li>
-   <li class="toc-h1 nav-item toc-entry">
-    <a class="reference internal nav-link" href="#another-top-level-title">
-     4.2. Another top-level title
-    </a>
-    <ul class="visible nav section-nav flex-column">
-     <li class="toc-h2 nav-item toc-entry">
-      <a class="reference internal nav-link" href="#another-sub-heading">
-       4.2.1. Another sub-heading
+     <li class="toc-h1 nav-item toc-entry">
+      <a class="reference internal nav-link" href="#another-top-level-title">
+       4.2. Another top-level title
       </a>
+      <ul class="visible nav section-nav flex-column">
+       <li class="toc-h2 nav-item toc-entry">
+        <a class="reference internal nav-link" href="#another-sub-heading">
+         4.2.1. Another sub-heading
+        </a>
+       </li>
+      </ul>
      </li>
     </ul>
-   </li>
-  </ul>
- </nav>
+   </nav>
+  </div>
+ </div>
 </div>
```

### Comparing `tskit_book_theme-0.3.2/tests/test_build/build__pagetoc--page-onetitle.html` & `tskit_book_theme-1.0.1/tests/test_build/build__pagetoc--page-onetitle.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-<div class="col-md-3 bd-toc show noprint">
- <div class="tocsection onthispage pt-5 pb-3">
-  <i class="fas fa-list">
-  </i>
-  Contents
+<div class="bd-sidebar-secondary bd-toc">
+ <div class="sidebar-secondary-items sidebar-secondary__inner">
+  <div class="sidebar-secondary-item">
+   <div class="page-toc tocsection onthispage">
+    <i class="fa-solid fa-list">
+    </i>
+    Contents
+   </div>
+   <nav class="bd-toc-nav page-toc">
+    <ul class="visible nav section-nav flex-column">
+     <li class="toc-h2 nav-item toc-entry">
+      <a class="reference internal nav-link" href="#here-s-a-sub-heading">
+       4.3.1. Here’s a sub-heading
+      </a>
+     </li>
+     <li class="toc-h2 nav-item toc-entry">
+      <a class="reference internal nav-link" href="#here-s-another">
+       4.3.2. Here’s another
+      </a>
+     </li>
+    </ul>
+   </nav>
+  </div>
  </div>
- <nav aria-label="Page" id="bd-toc-nav">
-  <ul class="visible nav section-nav flex-column">
-   <li class="toc-h2 nav-item toc-entry">
-    <a class="reference internal nav-link" href="#here-s-a-sub-heading">
-     4.3.1. Here’s a sub-heading
-    </a>
-   </li>
-   <li class="toc-h2 nav-item toc-entry">
-    <a class="reference internal nav-link" href="#here-s-another">
-     4.3.2. Here’s another
-    </a>
-   </li>
-  </ul>
- </nav>
 </div>
```

### Comparing `tskit_book_theme-0.3.2/tests/test_build/header__repo-buttons--all-on.html` & `tskit_book_theme-1.0.1/tests/test_build/header__repo-buttons--custom-branch.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,212 @@
 00000000: 3c64 6976 2063 6c61 7373 3d22 6865 6164  <div class="head
-00000010: 6572 2d61 7274 6963 6c65 5f5f 7269 6768  er-article__righ
-00000020: 7422 3e0a 203c 6275 7474 6f6e 2063 6c61  t">. <button cla
-00000030: 7373 3d22 6865 6164 6572 6274 6e22 2064  ss="headerbtn" d
-00000040: 6174 612d 706c 6163 656d 656e 743d 2262  ata-placement="b
-00000050: 6f74 746f 6d22 2064 6174 612d 746f 6767  ottom" data-togg
-00000060: 6c65 3d22 746f 6f6c 7469 7022 206f 6e63  le="tooltip" onc
-00000070: 6c69 636b 3d22 746f 6767 6c65 4675 6c6c  lick="toggleFull
-00000080: 5363 7265 656e 2829 2220 7469 746c 653d  Screen()" title=
-00000090: 2246 756c 6c73 6372 6565 6e20 6d6f 6465  "Fullscreen mode
-000000a0: 223e 0a20 203c 7370 616e 2063 6c61 7373  ">.  <span class
-000000b0: 3d22 6865 6164 6572 6274 6e5f 5f69 636f  ="headerbtn__ico
-000000c0: 6e2d 636f 6e74 6169 6e65 7222 3e0a 2020  n-container">.  
-000000d0: 203c 6920 636c 6173 733d 2266 6173 2066   <i class="fas f
-000000e0: 612d 6578 7061 6e64 223e 0a20 2020 3c2f  a-expand">.   </
-000000f0: 693e 0a20 203c 2f73 7061 6e3e 0a20 3c2f  i>.  </span>. </
-00000100: 6275 7474 6f6e 3e0a 203c 6469 7620 636c  button>. <div cl
-00000110: 6173 733d 226d 656e 752d 6472 6f70 646f  ass="menu-dropdo
-00000120: 776e 206d 656e 752d 6472 6f70 646f 776e  wn menu-dropdown
-00000130: 2d72 6570 6f73 6974 6f72 792d 6275 7474  -repository-butt
-00000140: 6f6e 7322 3e0a 2020 3c62 7574 746f 6e20  ons">.  <button 
-00000150: 6172 6961 2d6c 6162 656c 3d22 536f 7572  aria-label="Sour
-00000160: 6365 2072 6570 6f73 6974 6f72 6965 7322  ce repositories"
-00000170: 2063 6c61 7373 3d22 6865 6164 6572 6274   class="headerbt
-00000180: 6e20 6d65 6e75 2d64 726f 7064 6f77 6e5f  n menu-dropdown_
-00000190: 5f74 7269 6767 6572 223e 0a20 2020 3c69  _trigger">.   <i
-000001a0: 2063 6c61 7373 3d22 6661 6220 6661 2d67   class="fab fa-g
-000001b0: 6974 6875 6222 3e0a 2020 203c 2f69 3e0a  ithub">.   </i>.
-000001c0: 2020 3c2f 6275 7474 6f6e 3e0a 2020 3c64    </button>.  <d
-000001d0: 6976 2063 6c61 7373 3d22 6d65 6e75 2d64  iv class="menu-d
-000001e0: 726f 7064 6f77 6e5f 5f63 6f6e 7465 6e74  ropdown__content
-000001f0: 223e 0a20 2020 3c75 6c3e 0a20 2020 203c  ">.   <ul>.    <
-00000200: 6c69 3e0a 2020 2020 203c 6120 636c 6173  li>.     <a clas
-00000210: 733d 2268 6561 6465 7262 746e 2220 6461  s="headerbtn" da
-00000220: 7461 2d70 6c61 6365 6d65 6e74 3d22 6c65  ta-placement="le
-00000230: 6674 2220 6461 7461 2d74 6f67 676c 653d  ft" data-toggle=
-00000240: 2274 6f6f 6c74 6970 2220 6872 6566 3d22  "tooltip" href="
-00000250: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000260: 6f6d 2f65 7865 6375 7461 626c 6562 6f6f  om/executableboo
-00000270: 6b73 2f73 7068 696e 782d 626f 6f6b 2d74  ks/sphinx-book-t
-00000280: 6865 6d65 2220 7469 746c 653d 2253 6f75  heme" title="Sou
-00000290: 7263 6520 7265 706f 7369 746f 7279 223e  rce repository">
-000002a0: 0a20 2020 2020 203c 7370 616e 2063 6c61  .      <span cla
-000002b0: 7373 3d22 6865 6164 6572 6274 6e5f 5f69  ss="headerbtn__i
-000002c0: 636f 6e2d 636f 6e74 6169 6e65 7222 3e0a  con-container">.
-000002d0: 2020 2020 2020 203c 6920 636c 6173 733d         <i class=
-000002e0: 2266 6162 2066 612d 6769 7468 7562 223e  "fab fa-github">
-000002f0: 0a20 2020 2020 2020 3c2f 693e 0a20 2020  .       </i>.   
-00000300: 2020 203c 2f73 7061 6e3e 0a20 2020 2020     </span>.     
-00000310: 203c 7370 616e 2063 6c61 7373 3d22 6865   <span class="he
-00000320: 6164 6572 6274 6e5f 5f74 6578 742d 636f  aderbtn__text-co
-00000330: 6e74 6169 6e65 7222 3e0a 2020 2020 2020  ntainer">.      
-00000340: 2072 6570 6f73 6974 6f72 790a 2020 2020   repository.    
-00000350: 2020 3c2f 7370 616e 3e0a 2020 2020 203c    </span>.     <
-00000360: 2f61 3e0a 2020 2020 3c2f 6c69 3e0a 2020  /a>.    </li>.  
-00000370: 2020 3c6c 693e 0a20 2020 2020 3c61 2063    <li>.     <a c
-00000380: 6c61 7373 3d22 6865 6164 6572 6274 6e22  lass="headerbtn"
-00000390: 2064 6174 612d 706c 6163 656d 656e 743d   data-placement=
-000003a0: 226c 6566 7422 2064 6174 612d 746f 6767  "left" data-togg
-000003b0: 6c65 3d22 746f 6f6c 7469 7022 2068 7265  le="tooltip" hre
-000003c0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-000003d0: 622e 636f 6d2f 6578 6563 7574 6162 6c65  b.com/executable
-000003e0: 626f 6f6b 732f 7370 6869 6e78 2d62 6f6f  books/sphinx-boo
-000003f0: 6b2d 7468 656d 652f 6973 7375 6573 2f6e  k-theme/issues/n
-00000400: 6577 3f74 6974 6c65 3d49 7373 7565 2532  ew?title=Issue%2
-00000410: 306f 6e25 3230 7061 6765 2532 3025 3246  0on%20page%20%2F
-00000420: 7365 6374 696f 6e31 2f6e 7462 6b2e 6874  section1/ntbk.ht
-00000430: 6d6c 2661 6d70 3b62 6f64 793d 596f 7572  ml&amp;body=Your
-00000440: 2532 3069 7373 7565 2532 3063 6f6e 7465  %20issue%20conte
-00000450: 6e74 2532 3068 6572 652e 2220 7469 746c  nt%20here." titl
-00000460: 653d 224f 7065 6e20 616e 2069 7373 7565  e="Open an issue
-00000470: 223e 0a20 2020 2020 203c 7370 616e 2063  ">.      <span c
-00000480: 6c61 7373 3d22 6865 6164 6572 6274 6e5f  lass="headerbtn_
-00000490: 5f69 636f 6e2d 636f 6e74 6169 6e65 7222  _icon-container"
-000004a0: 3e0a 2020 2020 2020 203c 6920 636c 6173  >.       <i clas
-000004b0: 733d 2266 6173 2066 612d 6c69 6768 7462  s="fas fa-lightb
-000004c0: 756c 6222 3e0a 2020 2020 2020 203c 2f69  ulb">.       </i
-000004d0: 3e0a 2020 2020 2020 3c2f 7370 616e 3e0a  >.      </span>.
-000004e0: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-000004f0: 733d 2268 6561 6465 7262 746e 5f5f 7465  s="headerbtn__te
-00000500: 7874 2d63 6f6e 7461 696e 6572 223e 0a20  xt-container">. 
-00000510: 2020 2020 2020 6f70 656e 2069 7373 7565        open issue
-00000520: 0a20 2020 2020 203c 2f73 7061 6e3e 0a20  .      </span>. 
-00000530: 2020 2020 3c2f 613e 0a20 2020 203c 2f6c      </a>.    </l
-00000540: 693e 0a20 2020 203c 6c69 3e0a 2020 2020  i>.    <li>.    
-00000550: 203c 6120 636c 6173 733d 2268 6561 6465   <a class="heade
-00000560: 7262 746e 2220 6461 7461 2d70 6c61 6365  rbtn" data-place
-00000570: 6d65 6e74 3d22 6c65 6674 2220 6461 7461  ment="left" data
-00000580: 2d74 6f67 676c 653d 2274 6f6f 6c74 6970  -toggle="tooltip
-00000590: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
-000005a0: 6769 7468 7562 2e63 6f6d 2f65 7865 6375  github.com/execu
-000005b0: 7461 626c 6562 6f6f 6b73 2f73 7068 696e  tablebooks/sphin
-000005c0: 782d 626f 6f6b 2d74 6865 6d65 2f65 6469  x-book-theme/edi
-000005d0: 742f 6d61 7374 6572 2f73 6563 7469 6f6e  t/master/section
-000005e0: 312f 6e74 626b 2e69 7079 6e62 2220 7469  1/ntbk.ipynb" ti
-000005f0: 746c 653d 2245 6469 7420 7468 6973 2070  tle="Edit this p
-00000600: 6167 6522 3e0a 2020 2020 2020 3c73 7061  age">.      <spa
-00000610: 6e20 636c 6173 733d 2268 6561 6465 7262  n class="headerb
-00000620: 746e 5f5f 6963 6f6e 2d63 6f6e 7461 696e  tn__icon-contain
-00000630: 6572 223e 0a20 2020 2020 2020 3c69 2063  er">.       <i c
-00000640: 6c61 7373 3d22 6661 7320 6661 2d70 656e  lass="fas fa-pen
-00000650: 6369 6c2d 616c 7422 3e0a 2020 2020 2020  cil-alt">.      
-00000660: 203c 2f69 3e0a 2020 2020 2020 3c2f 7370   </i>.      </sp
-00000670: 616e 3e0a 2020 2020 2020 3c73 7061 6e20  an>.      <span 
-00000680: 636c 6173 733d 2268 6561 6465 7262 746e  class="headerbtn
-00000690: 5f5f 7465 7874 2d63 6f6e 7461 696e 6572  __text-container
-000006a0: 223e 0a20 2020 2020 2020 7375 6767 6573  ">.       sugges
-000006b0: 7420 6564 6974 0a20 2020 2020 203c 2f73  t edit.      </s
-000006c0: 7061 6e3e 0a20 2020 2020 3c2f 613e 0a20  pan>.     </a>. 
-000006d0: 2020 203c 2f6c 693e 0a20 2020 3c2f 756c     </li>.   </ul
-000006e0: 3e0a 2020 3c2f 6469 763e 0a20 3c2f 6469  >.  </div>. </di
-000006f0: 763e 0a20 3c64 6976 2063 6c61 7373 3d22  v>. <div class="
-00000700: 6d65 6e75 2d64 726f 7064 6f77 6e20 6d65  menu-dropdown me
-00000710: 6e75 2d64 726f 7064 6f77 6e2d 646f 776e  nu-dropdown-down
-00000720: 6c6f 6164 2d62 7574 746f 6e73 223e 0a20  load-buttons">. 
-00000730: 203c 6275 7474 6f6e 2061 7269 612d 6c61   <button aria-la
-00000740: 6265 6c3d 2244 6f77 6e6c 6f61 6420 7468  bel="Download th
-00000750: 6973 2070 6167 6522 2063 6c61 7373 3d22  is page" class="
-00000760: 6865 6164 6572 6274 6e20 6d65 6e75 2d64  headerbtn menu-d
-00000770: 726f 7064 6f77 6e5f 5f74 7269 6767 6572  ropdown__trigger
-00000780: 223e 0a20 2020 3c69 2063 6c61 7373 3d22  ">.   <i class="
-00000790: 6661 7320 6661 2d64 6f77 6e6c 6f61 6422  fas fa-download"
-000007a0: 3e0a 2020 203c 2f69 3e0a 2020 3c2f 6275  >.   </i>.  </bu
-000007b0: 7474 6f6e 3e0a 2020 3c64 6976 2063 6c61  tton>.  <div cla
-000007c0: 7373 3d22 6d65 6e75 2d64 726f 7064 6f77  ss="menu-dropdow
-000007d0: 6e5f 5f63 6f6e 7465 6e74 223e 0a20 2020  n__content">.   
-000007e0: 3c75 6c3e 0a20 2020 203c 6c69 3e0a 2020  <ul>.    <li>.  
-000007f0: 2020 203c 6120 636c 6173 733d 2268 6561     <a class="hea
-00000800: 6465 7262 746e 2220 6461 7461 2d70 6c61  derbtn" data-pla
-00000810: 6365 6d65 6e74 3d22 6c65 6674 2220 6461  cement="left" da
-00000820: 7461 2d74 6f67 676c 653d 2274 6f6f 6c74  ta-toggle="toolt
-00000830: 6970 2220 6872 6566 3d22 2e2e 2f5f 736f  ip" href="../_so
-00000840: 7572 6365 732f 7365 6374 696f 6e31 2f6e  urces/section1/n
-00000850: 7462 6b2e 6970 796e 6222 2074 6974 6c65  tbk.ipynb" title
-00000860: 3d22 446f 776e 6c6f 6164 2073 6f75 7263  ="Download sourc
-00000870: 6520 6669 6c65 223e 0a20 2020 2020 203c  e file">.      <
-00000880: 7370 616e 2063 6c61 7373 3d22 6865 6164  span class="head
-00000890: 6572 6274 6e5f 5f69 636f 6e2d 636f 6e74  erbtn__icon-cont
-000008a0: 6169 6e65 7222 3e0a 2020 2020 2020 203c  ainer">.       <
-000008b0: 6920 636c 6173 733d 2266 6173 2066 612d  i class="fas fa-
-000008c0: 6669 6c65 223e 0a20 2020 2020 2020 3c2f  file">.       </
-000008d0: 693e 0a20 2020 2020 203c 2f73 7061 6e3e  i>.      </span>
-000008e0: 0a20 2020 2020 203c 7370 616e 2063 6c61  .      <span cla
-000008f0: 7373 3d22 6865 6164 6572 6274 6e5f 5f74  ss="headerbtn__t
-00000900: 6578 742d 636f 6e74 6169 6e65 7222 3e0a  ext-container">.
-00000910: 2020 2020 2020 202e 6970 796e 620a 2020         .ipynb.  
-00000920: 2020 2020 3c2f 7370 616e 3e0a 2020 2020      </span>.    
-00000930: 203c 2f61 3e0a 2020 2020 3c2f 6c69 3e0a   </a>.    </li>.
-00000940: 2020 2020 3c6c 693e 0a20 2020 2020 3c62      <li>.     <b
-00000950: 7574 746f 6e20 636c 6173 733d 2268 6561  utton class="hea
-00000960: 6465 7262 746e 2220 6461 7461 2d70 6c61  derbtn" data-pla
-00000970: 6365 6d65 6e74 3d22 6c65 6674 2220 6461  cement="left" da
-00000980: 7461 2d74 6f67 676c 653d 2274 6f6f 6c74  ta-toggle="toolt
-00000990: 6970 2220 6f6e 636c 6963 6b3d 2270 7269  ip" onclick="pri
-000009a0: 6e74 5064 6628 7468 6973 2922 2074 6974  ntPdf(this)" tit
-000009b0: 6c65 3d22 5072 696e 7420 746f 2050 4446  le="Print to PDF
-000009c0: 223e 0a20 2020 2020 203c 7370 616e 2063  ">.      <span c
-000009d0: 6c61 7373 3d22 6865 6164 6572 6274 6e5f  lass="headerbtn_
-000009e0: 5f69 636f 6e2d 636f 6e74 6169 6e65 7222  _icon-container"
-000009f0: 3e0a 2020 2020 2020 203c 6920 636c 6173  >.       <i clas
-00000a00: 733d 2266 6173 2066 612d 6669 6c65 2d70  s="fas fa-file-p
-00000a10: 6466 223e 0a20 2020 2020 2020 3c2f 693e  df">.       </i>
-00000a20: 0a20 2020 2020 203c 2f73 7061 6e3e 0a20  .      </span>. 
-00000a30: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-00000a40: 3d22 6865 6164 6572 6274 6e5f 5f74 6578  ="headerbtn__tex
-00000a50: 742d 636f 6e74 6169 6e65 7222 3e0a 2020  t-container">.  
-00000a60: 2020 2020 202e 7064 660a 2020 2020 2020       .pdf.      
-00000a70: 3c2f 7370 616e 3e0a 2020 2020 203c 2f62  </span>.     </b
-00000a80: 7574 746f 6e3e 0a20 2020 203c 2f6c 693e  utton>.    </li>
-00000a90: 0a20 2020 3c2f 756c 3e0a 2020 3c2f 6469  .   </ul>.  </di
-00000aa0: 763e 0a20 3c2f 6469 763e 0a3c 2f64 6976  v>. </div>.</div
-00000ab0: 3e0a                                     >.
+00000010: 6572 2d61 7274 6963 6c65 2d69 7465 6d73  er-article-items
+00000020: 5f5f 656e 6422 3e0a 203c 6469 7620 636c  __end">. <div cl
+00000030: 6173 733d 2268 6561 6465 722d 6172 7469  ass="header-arti
+00000040: 636c 652d 6974 656d 223e 0a20 203c 6469  cle-item">.  <di
+00000050: 7620 636c 6173 733d 2261 7274 6963 6c65  v class="article
+00000060: 2d68 6561 6465 722d 6275 7474 6f6e 7322  -header-buttons"
+00000070: 3e0a 2020 203c 6469 7620 636c 6173 733d  >.   <div class=
+00000080: 2264 726f 7064 6f77 6e20 6472 6f70 646f  "dropdown dropdo
+00000090: 776e 2d6c 6175 6e63 682d 6275 7474 6f6e  wn-launch-button
+000000a0: 7322 3e0a 2020 2020 3c62 7574 746f 6e20  s">.    <button 
+000000b0: 6172 6961 2d65 7870 616e 6465 643d 2266  aria-expanded="f
+000000c0: 616c 7365 2220 6172 6961 2d6c 6162 656c  alse" aria-label
+000000d0: 3d22 4c61 756e 6368 2069 6e74 6572 6163  ="Launch interac
+000000e0: 7469 7665 2063 6f6e 7465 6e74 2220 636c  tive content" cl
+000000f0: 6173 733d 2262 746e 2064 726f 7064 6f77  ass="btn dropdow
+00000100: 6e2d 746f 6767 6c65 2220 6461 7461 2d62  n-toggle" data-b
+00000110: 732d 746f 6767 6c65 3d22 6472 6f70 646f  s-toggle="dropdo
+00000120: 776e 2220 7479 7065 3d22 6275 7474 6f6e  wn" type="button
+00000130: 223e 0a20 2020 2020 3c69 2063 6c61 7373  ">.     <i class
+00000140: 3d22 6661 7320 6661 2d72 6f63 6b65 7422  ="fas fa-rocket"
+00000150: 3e0a 2020 2020 203c 2f69 3e0a 2020 2020  >.     </i>.    
+00000160: 3c2f 6275 7474 6f6e 3e0a 2020 2020 3c75  </button>.    <u
+00000170: 6c20 636c 6173 733d 2264 726f 7064 6f77  l class="dropdow
+00000180: 6e2d 6d65 6e75 223e 0a20 2020 2020 3c6c  n-menu">.     <l
+00000190: 693e 0a20 2020 2020 203c 6120 636c 6173  i>.      <a clas
+000001a0: 733d 2262 746e 2062 746e 2d73 6d20 6472  s="btn btn-sm dr
+000001b0: 6f70 646f 776e 2d69 7465 6d22 2064 6174  opdown-item" dat
+000001c0: 612d 6273 2d70 6c61 6365 6d65 6e74 3d22  a-bs-placement="
+000001d0: 6c65 6674 2220 6461 7461 2d62 732d 746f  left" data-bs-to
+000001e0: 6767 6c65 3d22 746f 6f6c 7469 7022 2068  ggle="tooltip" h
+000001f0: 7265 663d 2268 7474 7073 3a2f 2f6d 7962  ref="https://myb
+00000200: 696e 6465 722e 6f72 672f 7632 2f67 682f  inder.org/v2/gh/
+00000210: 6578 6563 7574 6162 6c65 626f 6f6b 732f  executablebooks/
+00000220: 7370 6869 6e78 2d62 6f6f 6b2d 7468 656d  sphinx-book-them
+00000230: 652f 666f 6f3f 7572 6c70 6174 683d 7472  e/foo?urlpath=tr
+00000240: 6565 2f73 6563 7469 6f6e 312f 6e74 626b  ee/section1/ntbk
+00000250: 2e69 7079 6e62 2220 7461 7267 6574 3d22  .ipynb" target="
+00000260: 5f62 6c61 6e6b 2220 7469 746c 653d 224c  _blank" title="L
+00000270: 6175 6e63 6820 6f6e 4269 6e64 6572 223e  aunch onBinder">
+00000280: 0a20 2020 2020 2020 3c73 7061 6e20 636c  .       <span cl
+00000290: 6173 733d 2262 746e 5f5f 6963 6f6e 2d63  ass="btn__icon-c
+000002a0: 6f6e 7461 696e 6572 223e 0a20 2020 2020  ontainer">.     
+000002b0: 2020 203c 696d 6720 7372 633d 222e 2e2f     <img src="../
+000002c0: 5f73 7461 7469 632f 696d 6167 6573 2f6c  _static/images/l
+000002d0: 6f67 6f5f 6269 6e64 6572 2e73 7667 222f  ogo_binder.svg"/
+000002e0: 3e0a 2020 2020 2020 203c 2f73 7061 6e3e  >.       </span>
+000002f0: 0a20 2020 2020 2020 3c73 7061 6e20 636c  .       <span cl
+00000300: 6173 733d 2262 746e 5f5f 7465 7874 2d63  ass="btn__text-c
+00000310: 6f6e 7461 696e 6572 223e 0a20 2020 2020  ontainer">.     
+00000320: 2020 2042 696e 6465 720a 2020 2020 2020     Binder.      
+00000330: 203c 2f73 7061 6e3e 0a20 2020 2020 203c   </span>.      <
+00000340: 2f61 3e0a 2020 2020 203c 2f6c 693e 0a20  /a>.     </li>. 
+00000350: 2020 203c 2f75 6c3e 0a20 2020 3c2f 6469     </ul>.   </di
+00000360: 763e 0a20 2020 3c61 2063 6c61 7373 3d22  v>.   <a class="
+00000370: 6274 6e20 6274 6e2d 736d 2062 746e 2d73  btn btn-sm btn-s
+00000380: 6f75 7263 652d 6564 6974 2d62 7574 746f  ource-edit-butto
+00000390: 6e22 2064 6174 612d 6273 2d70 6c61 6365  n" data-bs-place
+000003a0: 6d65 6e74 3d22 626f 7474 6f6d 2220 6461  ment="bottom" da
+000003b0: 7461 2d62 732d 746f 6767 6c65 3d22 746f  ta-bs-toggle="to
+000003c0: 6f6c 7469 7022 2068 7265 663d 2268 7474  oltip" href="htt
+000003d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000003e0: 6578 6563 7574 6162 6c65 626f 6f6b 732f  executablebooks/
+000003f0: 7370 6869 6e78 2d62 6f6f 6b2d 7468 656d  sphinx-book-them
+00000400: 652f 6564 6974 2f66 6f6f 2f73 6563 7469  e/edit/foo/secti
+00000410: 6f6e 312f 6e74 626b 2e69 7079 6e62 2220  on1/ntbk.ipynb" 
+00000420: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
+00000430: 7469 746c 653d 2253 7567 6765 7374 2065  title="Suggest e
+00000440: 6469 7422 3e0a 2020 2020 3c73 7061 6e20  dit">.    <span 
+00000450: 636c 6173 733d 2262 746e 5f5f 6963 6f6e  class="btn__icon
+00000460: 2d63 6f6e 7461 696e 6572 223e 0a20 2020  -container">.   
+00000470: 2020 3c69 2063 6c61 7373 3d22 6661 7320    <i class="fas 
+00000480: 6661 2d70 656e 6369 6c2d 616c 7422 3e0a  fa-pencil-alt">.
+00000490: 2020 2020 203c 2f69 3e0a 2020 2020 3c2f       </i>.    </
+000004a0: 7370 616e 3e0a 2020 203c 2f61 3e0a 2020  span>.   </a>.  
+000004b0: 203c 6469 7620 636c 6173 733d 2264 726f   <div class="dro
+000004c0: 7064 6f77 6e20 6472 6f70 646f 776e 2d64  pdown dropdown-d
+000004d0: 6f77 6e6c 6f61 642d 6275 7474 6f6e 7322  ownload-buttons"
+000004e0: 3e0a 2020 2020 3c62 7574 746f 6e20 6172  >.    <button ar
+000004f0: 6961 2d65 7870 616e 6465 643d 2266 616c  ia-expanded="fal
+00000500: 7365 2220 6172 6961 2d6c 6162 656c 3d22  se" aria-label="
+00000510: 446f 776e 6c6f 6164 2074 6869 7320 7061  Download this pa
+00000520: 6765 2220 636c 6173 733d 2262 746e 2064  ge" class="btn d
+00000530: 726f 7064 6f77 6e2d 746f 6767 6c65 2220  ropdown-toggle" 
+00000540: 6461 7461 2d62 732d 746f 6767 6c65 3d22  data-bs-toggle="
+00000550: 6472 6f70 646f 776e 2220 7479 7065 3d22  dropdown" type="
+00000560: 6275 7474 6f6e 223e 0a20 2020 2020 3c69  button">.     <i
+00000570: 2063 6c61 7373 3d22 6661 7320 6661 2d64   class="fas fa-d
+00000580: 6f77 6e6c 6f61 6422 3e0a 2020 2020 203c  ownload">.     <
+00000590: 2f69 3e0a 2020 2020 3c2f 6275 7474 6f6e  /i>.    </button
+000005a0: 3e0a 2020 2020 3c75 6c20 636c 6173 733d  >.    <ul class=
+000005b0: 2264 726f 7064 6f77 6e2d 6d65 6e75 223e  "dropdown-menu">
+000005c0: 0a20 2020 2020 3c6c 693e 0a20 2020 2020  .     <li>.     
+000005d0: 203c 6120 636c 6173 733d 2262 746e 2062   <a class="btn b
+000005e0: 746e 2d73 6d20 6274 6e2d 646f 776e 6c6f  tn-sm btn-downlo
+000005f0: 6164 2d73 6f75 7263 652d 6275 7474 6f6e  ad-source-button
+00000600: 2064 726f 7064 6f77 6e2d 6974 656d 2220   dropdown-item" 
+00000610: 6461 7461 2d62 732d 706c 6163 656d 656e  data-bs-placemen
+00000620: 743d 226c 6566 7422 2064 6174 612d 6273  t="left" data-bs
+00000630: 2d74 6f67 676c 653d 2274 6f6f 6c74 6970  -toggle="tooltip
+00000640: 2220 6872 6566 3d22 2e2e 2f5f 736f 7572  " href="../_sour
+00000650: 6365 732f 7365 6374 696f 6e31 2f6e 7462  ces/section1/ntb
+00000660: 6b2e 6970 796e 6222 2074 6172 6765 743d  k.ipynb" target=
+00000670: 225f 626c 616e 6b22 2074 6974 6c65 3d22  "_blank" title="
+00000680: 446f 776e 6c6f 6164 2073 6f75 7263 6520  Download source 
+00000690: 6669 6c65 223e 0a20 2020 2020 2020 3c73  file">.       <s
+000006a0: 7061 6e20 636c 6173 733d 2262 746e 5f5f  pan class="btn__
+000006b0: 6963 6f6e 2d63 6f6e 7461 696e 6572 223e  icon-container">
+000006c0: 0a20 2020 2020 2020 203c 6920 636c 6173  .        <i clas
+000006d0: 733d 2266 6173 2066 612d 6669 6c65 223e  s="fas fa-file">
+000006e0: 0a20 2020 2020 2020 203c 2f69 3e0a 2020  .        </i>.  
+000006f0: 2020 2020 203c 2f73 7061 6e3e 0a20 2020       </span>.   
+00000700: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00000710: 2262 746e 5f5f 7465 7874 2d63 6f6e 7461  "btn__text-conta
+00000720: 696e 6572 223e 0a20 2020 2020 2020 202e  iner">.        .
+00000730: 6970 796e 620a 2020 2020 2020 203c 2f73  ipynb.       </s
+00000740: 7061 6e3e 0a20 2020 2020 203c 2f61 3e0a  pan>.      </a>.
+00000750: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+00000760: 3c6c 693e 0a20 2020 2020 203c 6275 7474  <li>.      <butt
+00000770: 6f6e 2063 6c61 7373 3d22 6274 6e20 6274  on class="btn bt
+00000780: 6e2d 736d 2062 746e 2d64 6f77 6e6c 6f61  n-sm btn-downloa
+00000790: 642d 7064 662d 6275 7474 6f6e 2064 726f  d-pdf-button dro
+000007a0: 7064 6f77 6e2d 6974 656d 2220 6461 7461  pdown-item" data
+000007b0: 2d62 732d 706c 6163 656d 656e 743d 226c  -bs-placement="l
+000007c0: 6566 7422 2064 6174 612d 6273 2d74 6f67  eft" data-bs-tog
+000007d0: 676c 653d 2274 6f6f 6c74 6970 2220 6f6e  gle="tooltip" on
+000007e0: 636c 6963 6b3d 2277 696e 646f 772e 7072  click="window.pr
+000007f0: 696e 7428 2922 2074 6974 6c65 3d22 5072  int()" title="Pr
+00000800: 696e 7420 746f 2050 4446 223e 0a20 2020  int to PDF">.   
+00000810: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00000820: 2262 746e 5f5f 6963 6f6e 2d63 6f6e 7461  "btn__icon-conta
+00000830: 696e 6572 223e 0a20 2020 2020 2020 203c  iner">.        <
+00000840: 6920 636c 6173 733d 2266 6173 2066 612d  i class="fas fa-
+00000850: 6669 6c65 2d70 6466 223e 0a20 2020 2020  file-pdf">.     
+00000860: 2020 203c 2f69 3e0a 2020 2020 2020 203c     </i>.       <
+00000870: 2f73 7061 6e3e 0a20 2020 2020 2020 3c73  /span>.       <s
+00000880: 7061 6e20 636c 6173 733d 2262 746e 5f5f  pan class="btn__
+00000890: 7465 7874 2d63 6f6e 7461 696e 6572 223e  text-container">
+000008a0: 0a20 2020 2020 2020 202e 7064 660a 2020  .        .pdf.  
+000008b0: 2020 2020 203c 2f73 7061 6e3e 0a20 2020       </span>.   
+000008c0: 2020 203c 2f62 7574 746f 6e3e 0a20 2020     </button>.   
+000008d0: 2020 3c2f 6c69 3e0a 2020 2020 3c2f 756c    </li>.    </ul
+000008e0: 3e0a 2020 203c 2f64 6976 3e0a 2020 203c  >.   </div>.   <
+000008f0: 6275 7474 6f6e 2063 6c61 7373 3d22 6274  button class="bt
+00000900: 6e20 6274 6e2d 736d 2062 746e 2d66 756c  n btn-sm btn-ful
+00000910: 6c73 6372 6565 6e2d 6275 7474 6f6e 2220  lscreen-button" 
+00000920: 6461 7461 2d62 732d 706c 6163 656d 656e  data-bs-placemen
+00000930: 743d 2262 6f74 746f 6d22 2064 6174 612d  t="bottom" data-
+00000940: 6273 2d74 6f67 676c 653d 2274 6f6f 6c74  bs-toggle="toolt
+00000950: 6970 2220 6f6e 636c 6963 6b3d 2274 6f67  ip" onclick="tog
+00000960: 676c 6546 756c 6c53 6372 6565 6e28 2922  gleFullScreen()"
+00000970: 2074 6974 6c65 3d22 4675 6c6c 7363 7265   title="Fullscre
+00000980: 656e 206d 6f64 6522 3e0a 2020 2020 3c73  en mode">.    <s
+00000990: 7061 6e20 636c 6173 733d 2262 746e 5f5f  pan class="btn__
+000009a0: 6963 6f6e 2d63 6f6e 7461 696e 6572 223e  icon-container">
+000009b0: 0a20 2020 2020 3c69 2063 6c61 7373 3d22  .     <i class="
+000009c0: 6661 7320 6661 2d65 7870 616e 6422 3e0a  fas fa-expand">.
+000009d0: 2020 2020 203c 2f69 3e0a 2020 2020 3c2f       </i>.    </
+000009e0: 7370 616e 3e0a 2020 203c 2f62 7574 746f  span>.   </butto
+000009f0: 6e3e 0a20 2020 3c73 6372 6970 743e 0a20  n>.   <script>. 
+00000a00: 2020 2064 6f63 756d 656e 742e 7772 6974     document.writ
+00000a10: 6528 600a 2020 3c62 7574 746f 6e20 636c  e(`.  <button cl
+00000a20: 6173 733d 2274 6865 6d65 2d73 7769 7463  ass="theme-switc
+00000a30: 682d 6275 7474 6f6e 2062 746e 2062 746e  h-button btn btn
+00000a40: 2d73 6d20 6274 6e2d 6f75 746c 696e 652d  -sm btn-outline-
+00000a50: 7072 696d 6172 7920 6e61 7662 6172 2d62  primary navbar-b
+00000a60: 746e 2072 6f75 6e64 6564 2d63 6972 636c  tn rounded-circl
+00000a70: 6522 2074 6974 6c65 3d22 6c69 6768 742f  e" title="light/
+00000a80: 6461 726b 2220 6172 6961 2d6c 6162 656c  dark" aria-label
+00000a90: 3d22 6c69 6768 742f 6461 726b 2220 6461  ="light/dark" da
+00000aa0: 7461 2d62 732d 706c 6163 656d 656e 743d  ta-bs-placement=
+00000ab0: 2262 6f74 746f 6d22 2064 6174 612d 6273  "bottom" data-bs
+00000ac0: 2d74 6f67 676c 653d 2274 6f6f 6c74 6970  -toggle="tooltip
+00000ad0: 223e 0a20 2020 203c 7370 616e 2063 6c61  ">.    <span cla
+00000ae0: 7373 3d22 7468 656d 652d 7377 6974 6368  ss="theme-switch
+00000af0: 2220 6461 7461 2d6d 6f64 653d 226c 6967  " data-mode="lig
+00000b00: 6874 223e 3c69 2063 6c61 7373 3d22 6661  ht"><i class="fa
+00000b10: 2d73 6f6c 6964 2066 612d 7375 6e22 3e3c  -solid fa-sun"><
+00000b20: 2f69 3e3c 2f73 7061 6e3e 0a20 2020 203c  /i></span>.    <
+00000b30: 7370 616e 2063 6c61 7373 3d22 7468 656d  span class="them
+00000b40: 652d 7377 6974 6368 2220 6461 7461 2d6d  e-switch" data-m
+00000b50: 6f64 653d 2264 6172 6b22 3e3c 6920 636c  ode="dark"><i cl
+00000b60: 6173 733d 2266 612d 736f 6c69 6420 6661  ass="fa-solid fa
+00000b70: 2d6d 6f6f 6e22 3e3c 2f69 3e3c 2f73 7061  -moon"></i></spa
+00000b80: 6e3e 0a20 2020 203c 7370 616e 2063 6c61  n>.    <span cla
+00000b90: 7373 3d22 7468 656d 652d 7377 6974 6368  ss="theme-switch
+00000ba0: 2220 6461 7461 2d6d 6f64 653d 2261 7574  " data-mode="aut
+00000bb0: 6f22 3e3c 6920 636c 6173 733d 2266 612d  o"><i class="fa-
+00000bc0: 736f 6c69 6420 6661 2d63 6972 636c 652d  solid fa-circle-
+00000bd0: 6861 6c66 2d73 7472 6f6b 6522 3e3c 2f69  half-stroke"></i
+00000be0: 3e3c 2f73 7061 6e3e 0a20 203c 2f62 7574  ></span>.  </but
+00000bf0: 746f 6e3e 0a60 293b 0a20 2020 3c2f 7363  ton>.`);.   </sc
+00000c00: 7269 7074 3e0a 2020 203c 7363 7269 7074  ript>.   <script
+00000c10: 3e0a 2020 2020 646f 6375 6d65 6e74 2e77  >.    document.w
+00000c20: 7269 7465 2860 0a20 203c 6275 7474 6f6e  rite(`.  <button
+00000c30: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
+00000c40: 736d 206e 6176 6261 722d 6274 6e20 7365  sm navbar-btn se
+00000c50: 6172 6368 2d62 7574 746f 6e20 7365 6172  arch-button sear
+00000c60: 6368 2d62 7574 746f 6e5f 5f62 7574 746f  ch-button__butto
+00000c70: 6e22 2074 6974 6c65 3d22 5365 6172 6368  n" title="Search
+00000c80: 2220 6172 6961 2d6c 6162 656c 3d22 5365  " aria-label="Se
+00000c90: 6172 6368 2220 6461 7461 2d62 732d 706c  arch" data-bs-pl
+00000ca0: 6163 656d 656e 743d 2262 6f74 746f 6d22  acement="bottom"
+00000cb0: 2064 6174 612d 6273 2d74 6f67 676c 653d   data-bs-toggle=
+00000cc0: 2274 6f6f 6c74 6970 223e 0a20 2020 203c  "tooltip">.    <
+00000cd0: 6920 636c 6173 733d 2266 612d 736f 6c69  i class="fa-soli
+00000ce0: 6420 6661 2d6d 6167 6e69 6679 696e 672d  d fa-magnifying-
+00000cf0: 676c 6173 7322 3e3c 2f69 3e0a 2020 3c2f  glass"></i>.  </
+00000d00: 6275 7474 6f6e 3e0a 6029 3b0a 2020 203c  button>.`);.   <
+00000d10: 2f73 6372 6970 743e 0a20 203c 2f64 6976  /script>.  </div
+00000d20: 3e0a 203c 2f64 6976 3e0a 3c2f 6469 763e  >. </div>.</div>
+00000d30: 0a                                       .
```

### Comparing `tskit_book_theme-0.3.2/tests/test_build/header__repo-buttons--custom-branch.html` & `tskit_book_theme-1.0.1/tests/test_build/header__repo-buttons--all-off.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,144 @@
 00000000: 3c64 6976 2063 6c61 7373 3d22 6865 6164  <div class="head
-00000010: 6572 2d61 7274 6963 6c65 5f5f 7269 6768  er-article__righ
-00000020: 7422 3e0a 203c 6469 7620 636c 6173 733d  t">. <div class=
-00000030: 226d 656e 752d 6472 6f70 646f 776e 206d  "menu-dropdown m
-00000040: 656e 752d 6472 6f70 646f 776e 2d6c 6175  enu-dropdown-lau
-00000050: 6e63 682d 6275 7474 6f6e 7322 3e0a 2020  nch-buttons">.  
-00000060: 3c62 7574 746f 6e20 6172 6961 2d6c 6162  <button aria-lab
-00000070: 656c 3d22 4c61 756e 6368 2069 6e74 6572  el="Launch inter
-00000080: 6163 7469 7665 2063 6f6e 7465 6e74 2220  active content" 
-00000090: 636c 6173 733d 2268 6561 6465 7262 746e  class="headerbtn
-000000a0: 206d 656e 752d 6472 6f70 646f 776e 5f5f   menu-dropdown__
-000000b0: 7472 6967 6765 7222 3e0a 2020 203c 6920  trigger">.   <i 
-000000c0: 636c 6173 733d 2266 6173 2066 612d 726f  class="fas fa-ro
-000000d0: 636b 6574 223e 0a20 2020 3c2f 693e 0a20  cket">.   </i>. 
-000000e0: 203c 2f62 7574 746f 6e3e 0a20 203c 6469   </button>.  <di
-000000f0: 7620 636c 6173 733d 226d 656e 752d 6472  v class="menu-dr
-00000100: 6f70 646f 776e 5f5f 636f 6e74 656e 7422  opdown__content"
-00000110: 3e0a 2020 203c 756c 3e0a 2020 2020 3c6c  >.   <ul>.    <l
-00000120: 693e 0a20 2020 2020 3c61 2063 6c61 7373  i>.     <a class
-00000130: 3d22 6865 6164 6572 6274 6e22 2064 6174  ="headerbtn" dat
-00000140: 612d 706c 6163 656d 656e 743d 226c 6566  a-placement="lef
-00000150: 7422 2064 6174 612d 746f 6767 6c65 3d22  t" data-toggle="
-00000160: 746f 6f6c 7469 7022 2068 7265 663d 2268  tooltip" href="h
-00000170: 7474 7073 3a2f 2f6d 7962 696e 6465 722e  ttps://mybinder.
-00000180: 6f72 672f 7632 2f67 682f 6578 6563 7574  org/v2/gh/execut
-00000190: 6162 6c65 626f 6f6b 732f 7370 6869 6e78  ablebooks/sphinx
-000001a0: 2d62 6f6f 6b2d 7468 656d 652f 666f 6f3f  -book-theme/foo?
-000001b0: 7572 6c70 6174 683d 7472 6565 2f73 6563  urlpath=tree/sec
-000001c0: 7469 6f6e 312f 6e74 626b 2e69 7079 6e62  tion1/ntbk.ipynb
-000001d0: 2220 7469 746c 653d 224c 6175 6e63 6820  " title="Launch 
-000001e0: 6f6e 2042 696e 6465 7222 3e0a 2020 2020  on Binder">.    
-000001f0: 2020 3c73 7061 6e20 636c 6173 733d 2268    <span class="h
-00000200: 6561 6465 7262 746e 5f5f 6963 6f6e 2d63  eaderbtn__icon-c
-00000210: 6f6e 7461 696e 6572 223e 0a20 2020 2020  ontainer">.     
-00000220: 2020 3c69 6d67 2073 7263 3d22 2e2e 2f5f    <img src="../_
-00000230: 7374 6174 6963 2f69 6d61 6765 732f 6c6f  static/images/lo
-00000240: 676f 5f62 696e 6465 722e 7376 6722 2f3e  go_binder.svg"/>
-00000250: 0a20 2020 2020 203c 2f73 7061 6e3e 0a20  .      </span>. 
-00000260: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-00000270: 3d22 6865 6164 6572 6274 6e5f 5f74 6578  ="headerbtn__tex
-00000280: 742d 636f 6e74 6169 6e65 7222 3e0a 2020  t-container">.  
-00000290: 2020 2020 2042 696e 6465 720a 2020 2020       Binder.    
-000002a0: 2020 3c2f 7370 616e 3e0a 2020 2020 203c    </span>.     <
-000002b0: 2f61 3e0a 2020 2020 3c2f 6c69 3e0a 2020  /a>.    </li>.  
-000002c0: 203c 2f75 6c3e 0a20 203c 2f64 6976 3e0a   </ul>.  </div>.
-000002d0: 203c 2f64 6976 3e0a 203c 6275 7474 6f6e   </div>. <button
-000002e0: 2063 6c61 7373 3d22 6865 6164 6572 6274   class="headerbt
-000002f0: 6e22 2064 6174 612d 706c 6163 656d 656e  n" data-placemen
-00000300: 743d 2262 6f74 746f 6d22 2064 6174 612d  t="bottom" data-
-00000310: 746f 6767 6c65 3d22 746f 6f6c 7469 7022  toggle="tooltip"
-00000320: 206f 6e63 6c69 636b 3d22 746f 6767 6c65   onclick="toggle
-00000330: 4675 6c6c 5363 7265 656e 2829 2220 7469  FullScreen()" ti
-00000340: 746c 653d 2246 756c 6c73 6372 6565 6e20  tle="Fullscreen 
-00000350: 6d6f 6465 223e 0a20 203c 7370 616e 2063  mode">.  <span c
-00000360: 6c61 7373 3d22 6865 6164 6572 6274 6e5f  lass="headerbtn_
-00000370: 5f69 636f 6e2d 636f 6e74 6169 6e65 7222  _icon-container"
-00000380: 3e0a 2020 203c 6920 636c 6173 733d 2266  >.   <i class="f
-00000390: 6173 2066 612d 6578 7061 6e64 223e 0a20  as fa-expand">. 
-000003a0: 2020 3c2f 693e 0a20 203c 2f73 7061 6e3e    </i>.  </span>
-000003b0: 0a20 3c2f 6275 7474 6f6e 3e0a 203c 6120  . </button>. <a 
-000003c0: 636c 6173 733d 2268 6561 6465 7262 746e  class="headerbtn
-000003d0: 2220 6461 7461 2d70 6c61 6365 6d65 6e74  " data-placement
-000003e0: 3d22 626f 7474 6f6d 2220 6461 7461 2d74  ="bottom" data-t
-000003f0: 6f67 676c 653d 2274 6f6f 6c74 6970 2220  oggle="tooltip" 
-00000400: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000410: 7468 7562 2e63 6f6d 2f65 7865 6375 7461  thub.com/executa
-00000420: 626c 6562 6f6f 6b73 2f73 7068 696e 782d  blebooks/sphinx-
-00000430: 626f 6f6b 2d74 6865 6d65 2f65 6469 742f  book-theme/edit/
-00000440: 666f 6f2f 7365 6374 696f 6e31 2f6e 7462  foo/section1/ntb
-00000450: 6b2e 6970 796e 6222 2074 6974 6c65 3d22  k.ipynb" title="
-00000460: 4564 6974 2074 6869 7320 7061 6765 223e  Edit this page">
-00000470: 0a20 203c 7370 616e 2063 6c61 7373 3d22  .  <span class="
-00000480: 6865 6164 6572 6274 6e5f 5f69 636f 6e2d  headerbtn__icon-
-00000490: 636f 6e74 6169 6e65 7222 3e0a 2020 203c  container">.   <
-000004a0: 6920 636c 6173 733d 2266 6173 2066 612d  i class="fas fa-
-000004b0: 7065 6e63 696c 2d61 6c74 223e 0a20 2020  pencil-alt">.   
-000004c0: 3c2f 693e 0a20 203c 2f73 7061 6e3e 0a20  </i>.  </span>. 
-000004d0: 3c2f 613e 0a20 3c64 6976 2063 6c61 7373  </a>. <div class
-000004e0: 3d22 6d65 6e75 2d64 726f 7064 6f77 6e20  ="menu-dropdown 
-000004f0: 6d65 6e75 2d64 726f 7064 6f77 6e2d 646f  menu-dropdown-do
-00000500: 776e 6c6f 6164 2d62 7574 746f 6e73 223e  wnload-buttons">
-00000510: 0a20 203c 6275 7474 6f6e 2061 7269 612d  .  <button aria-
-00000520: 6c61 6265 6c3d 2244 6f77 6e6c 6f61 6420  label="Download 
-00000530: 7468 6973 2070 6167 6522 2063 6c61 7373  this page" class
-00000540: 3d22 6865 6164 6572 6274 6e20 6d65 6e75  ="headerbtn menu
-00000550: 2d64 726f 7064 6f77 6e5f 5f74 7269 6767  -dropdown__trigg
-00000560: 6572 223e 0a20 2020 3c69 2063 6c61 7373  er">.   <i class
-00000570: 3d22 6661 7320 6661 2d64 6f77 6e6c 6f61  ="fas fa-downloa
-00000580: 6422 3e0a 2020 203c 2f69 3e0a 2020 3c2f  d">.   </i>.  </
-00000590: 6275 7474 6f6e 3e0a 2020 3c64 6976 2063  button>.  <div c
-000005a0: 6c61 7373 3d22 6d65 6e75 2d64 726f 7064  lass="menu-dropd
-000005b0: 6f77 6e5f 5f63 6f6e 7465 6e74 223e 0a20  own__content">. 
-000005c0: 2020 3c75 6c3e 0a20 2020 203c 6c69 3e0a    <ul>.    <li>.
-000005d0: 2020 2020 203c 6120 636c 6173 733d 2268       <a class="h
-000005e0: 6561 6465 7262 746e 2220 6461 7461 2d70  eaderbtn" data-p
-000005f0: 6c61 6365 6d65 6e74 3d22 6c65 6674 2220  lacement="left" 
-00000600: 6461 7461 2d74 6f67 676c 653d 2274 6f6f  data-toggle="too
-00000610: 6c74 6970 2220 6872 6566 3d22 2e2e 2f5f  ltip" href="../_
-00000620: 736f 7572 6365 732f 7365 6374 696f 6e31  sources/section1
-00000630: 2f6e 7462 6b2e 6970 796e 6222 2074 6974  /ntbk.ipynb" tit
-00000640: 6c65 3d22 446f 776e 6c6f 6164 2073 6f75  le="Download sou
-00000650: 7263 6520 6669 6c65 223e 0a20 2020 2020  rce file">.     
-00000660: 203c 7370 616e 2063 6c61 7373 3d22 6865   <span class="he
-00000670: 6164 6572 6274 6e5f 5f69 636f 6e2d 636f  aderbtn__icon-co
-00000680: 6e74 6169 6e65 7222 3e0a 2020 2020 2020  ntainer">.      
-00000690: 203c 6920 636c 6173 733d 2266 6173 2066   <i class="fas f
-000006a0: 612d 6669 6c65 223e 0a20 2020 2020 2020  a-file">.       
-000006b0: 3c2f 693e 0a20 2020 2020 203c 2f73 7061  </i>.      </spa
-000006c0: 6e3e 0a20 2020 2020 203c 7370 616e 2063  n>.      <span c
-000006d0: 6c61 7373 3d22 6865 6164 6572 6274 6e5f  lass="headerbtn_
-000006e0: 5f74 6578 742d 636f 6e74 6169 6e65 7222  _text-container"
-000006f0: 3e0a 2020 2020 2020 202e 6970 796e 620a  >.       .ipynb.
-00000700: 2020 2020 2020 3c2f 7370 616e 3e0a 2020        </span>.  
-00000710: 2020 203c 2f61 3e0a 2020 2020 3c2f 6c69     </a>.    </li
-00000720: 3e0a 2020 2020 3c6c 693e 0a20 2020 2020  >.    <li>.     
-00000730: 3c62 7574 746f 6e20 636c 6173 733d 2268  <button class="h
-00000740: 6561 6465 7262 746e 2220 6461 7461 2d70  eaderbtn" data-p
-00000750: 6c61 6365 6d65 6e74 3d22 6c65 6674 2220  lacement="left" 
-00000760: 6461 7461 2d74 6f67 676c 653d 2274 6f6f  data-toggle="too
-00000770: 6c74 6970 2220 6f6e 636c 6963 6b3d 2270  ltip" onclick="p
-00000780: 7269 6e74 5064 6628 7468 6973 2922 2074  rintPdf(this)" t
-00000790: 6974 6c65 3d22 5072 696e 7420 746f 2050  itle="Print to P
-000007a0: 4446 223e 0a20 2020 2020 203c 7370 616e  DF">.      <span
-000007b0: 2063 6c61 7373 3d22 6865 6164 6572 6274   class="headerbt
-000007c0: 6e5f 5f69 636f 6e2d 636f 6e74 6169 6e65  n__icon-containe
-000007d0: 7222 3e0a 2020 2020 2020 203c 6920 636c  r">.       <i cl
-000007e0: 6173 733d 2266 6173 2066 612d 6669 6c65  ass="fas fa-file
-000007f0: 2d70 6466 223e 0a20 2020 2020 2020 3c2f  -pdf">.       </
-00000800: 693e 0a20 2020 2020 203c 2f73 7061 6e3e  i>.      </span>
-00000810: 0a20 2020 2020 203c 7370 616e 2063 6c61  .      <span cla
-00000820: 7373 3d22 6865 6164 6572 6274 6e5f 5f74  ss="headerbtn__t
-00000830: 6578 742d 636f 6e74 6169 6e65 7222 3e0a  ext-container">.
-00000840: 2020 2020 2020 202e 7064 660a 2020 2020         .pdf.    
-00000850: 2020 3c2f 7370 616e 3e0a 2020 2020 203c    </span>.     <
-00000860: 2f62 7574 746f 6e3e 0a20 2020 203c 2f6c  /button>.    </l
-00000870: 693e 0a20 2020 3c2f 756c 3e0a 2020 3c2f  i>.   </ul>.  </
-00000880: 6469 763e 0a20 3c2f 6469 763e 0a3c 2f64  div>. </div>.</d
-00000890: 6976 3e0a                                iv>.
+00000010: 6572 2d61 7274 6963 6c65 2d69 7465 6d73  er-article-items
+00000020: 5f5f 656e 6422 3e0a 203c 6469 7620 636c  __end">. <div cl
+00000030: 6173 733d 2268 6561 6465 722d 6172 7469  ass="header-arti
+00000040: 636c 652d 6974 656d 223e 0a20 203c 6469  cle-item">.  <di
+00000050: 7620 636c 6173 733d 2261 7274 6963 6c65  v class="article
+00000060: 2d68 6561 6465 722d 6275 7474 6f6e 7322  -header-buttons"
+00000070: 3e0a 2020 203c 6469 7620 636c 6173 733d  >.   <div class=
+00000080: 2264 726f 7064 6f77 6e20 6472 6f70 646f  "dropdown dropdo
+00000090: 776e 2d64 6f77 6e6c 6f61 642d 6275 7474  wn-download-butt
+000000a0: 6f6e 7322 3e0a 2020 2020 3c62 7574 746f  ons">.    <butto
+000000b0: 6e20 6172 6961 2d65 7870 616e 6465 643d  n aria-expanded=
+000000c0: 2266 616c 7365 2220 6172 6961 2d6c 6162  "false" aria-lab
+000000d0: 656c 3d22 446f 776e 6c6f 6164 2074 6869  el="Download thi
+000000e0: 7320 7061 6765 2220 636c 6173 733d 2262  s page" class="b
+000000f0: 746e 2064 726f 7064 6f77 6e2d 746f 6767  tn dropdown-togg
+00000100: 6c65 2220 6461 7461 2d62 732d 746f 6767  le" data-bs-togg
+00000110: 6c65 3d22 6472 6f70 646f 776e 2220 7479  le="dropdown" ty
+00000120: 7065 3d22 6275 7474 6f6e 223e 0a20 2020  pe="button">.   
+00000130: 2020 3c69 2063 6c61 7373 3d22 6661 7320    <i class="fas 
+00000140: 6661 2d64 6f77 6e6c 6f61 6422 3e0a 2020  fa-download">.  
+00000150: 2020 203c 2f69 3e0a 2020 2020 3c2f 6275     </i>.    </bu
+00000160: 7474 6f6e 3e0a 2020 2020 3c75 6c20 636c  tton>.    <ul cl
+00000170: 6173 733d 2264 726f 7064 6f77 6e2d 6d65  ass="dropdown-me
+00000180: 6e75 223e 0a20 2020 2020 3c6c 693e 0a20  nu">.     <li>. 
+00000190: 2020 2020 203c 6120 636c 6173 733d 2262       <a class="b
+000001a0: 746e 2062 746e 2d73 6d20 6274 6e2d 646f  tn btn-sm btn-do
+000001b0: 776e 6c6f 6164 2d73 6f75 7263 652d 6275  wnload-source-bu
+000001c0: 7474 6f6e 2064 726f 7064 6f77 6e2d 6974  tton dropdown-it
+000001d0: 656d 2220 6461 7461 2d62 732d 706c 6163  em" data-bs-plac
+000001e0: 656d 656e 743d 226c 6566 7422 2064 6174  ement="left" dat
+000001f0: 612d 6273 2d74 6f67 676c 653d 2274 6f6f  a-bs-toggle="too
+00000200: 6c74 6970 2220 6872 6566 3d22 2e2e 2f5f  ltip" href="../_
+00000210: 736f 7572 6365 732f 7365 6374 696f 6e31  sources/section1
+00000220: 2f6e 7462 6b2e 6970 796e 6222 2074 6172  /ntbk.ipynb" tar
+00000230: 6765 743d 225f 626c 616e 6b22 2074 6974  get="_blank" tit
+00000240: 6c65 3d22 446f 776e 6c6f 6164 2073 6f75  le="Download sou
+00000250: 7263 6520 6669 6c65 223e 0a20 2020 2020  rce file">.     
+00000260: 2020 3c73 7061 6e20 636c 6173 733d 2262    <span class="b
+00000270: 746e 5f5f 6963 6f6e 2d63 6f6e 7461 696e  tn__icon-contain
+00000280: 6572 223e 0a20 2020 2020 2020 203c 6920  er">.        <i 
+00000290: 636c 6173 733d 2266 6173 2066 612d 6669  class="fas fa-fi
+000002a0: 6c65 223e 0a20 2020 2020 2020 203c 2f69  le">.        </i
+000002b0: 3e0a 2020 2020 2020 203c 2f73 7061 6e3e  >.       </span>
+000002c0: 0a20 2020 2020 2020 3c73 7061 6e20 636c  .       <span cl
+000002d0: 6173 733d 2262 746e 5f5f 7465 7874 2d63  ass="btn__text-c
+000002e0: 6f6e 7461 696e 6572 223e 0a20 2020 2020  ontainer">.     
+000002f0: 2020 202e 6970 796e 620a 2020 2020 2020     .ipynb.      
+00000300: 203c 2f73 7061 6e3e 0a20 2020 2020 203c   </span>.      <
+00000310: 2f61 3e0a 2020 2020 203c 2f6c 693e 0a20  /a>.     </li>. 
+00000320: 2020 2020 3c6c 693e 0a20 2020 2020 203c      <li>.      <
+00000330: 6275 7474 6f6e 2063 6c61 7373 3d22 6274  button class="bt
+00000340: 6e20 6274 6e2d 736d 2062 746e 2d64 6f77  n btn-sm btn-dow
+00000350: 6e6c 6f61 642d 7064 662d 6275 7474 6f6e  nload-pdf-button
+00000360: 2064 726f 7064 6f77 6e2d 6974 656d 2220   dropdown-item" 
+00000370: 6461 7461 2d62 732d 706c 6163 656d 656e  data-bs-placemen
+00000380: 743d 226c 6566 7422 2064 6174 612d 6273  t="left" data-bs
+00000390: 2d74 6f67 676c 653d 2274 6f6f 6c74 6970  -toggle="tooltip
+000003a0: 2220 6f6e 636c 6963 6b3d 2277 696e 646f  " onclick="windo
+000003b0: 772e 7072 696e 7428 2922 2074 6974 6c65  w.print()" title
+000003c0: 3d22 5072 696e 7420 746f 2050 4446 223e  ="Print to PDF">
+000003d0: 0a20 2020 2020 2020 3c73 7061 6e20 636c  .       <span cl
+000003e0: 6173 733d 2262 746e 5f5f 6963 6f6e 2d63  ass="btn__icon-c
+000003f0: 6f6e 7461 696e 6572 223e 0a20 2020 2020  ontainer">.     
+00000400: 2020 203c 6920 636c 6173 733d 2266 6173     <i class="fas
+00000410: 2066 612d 6669 6c65 2d70 6466 223e 0a20   fa-file-pdf">. 
+00000420: 2020 2020 2020 203c 2f69 3e0a 2020 2020         </i>.    
+00000430: 2020 203c 2f73 7061 6e3e 0a20 2020 2020     </span>.     
+00000440: 2020 3c73 7061 6e20 636c 6173 733d 2262    <span class="b
+00000450: 746e 5f5f 7465 7874 2d63 6f6e 7461 696e  tn__text-contain
+00000460: 6572 223e 0a20 2020 2020 2020 202e 7064  er">.        .pd
+00000470: 660a 2020 2020 2020 203c 2f73 7061 6e3e  f.       </span>
+00000480: 0a20 2020 2020 203c 2f62 7574 746f 6e3e  .      </button>
+00000490: 0a20 2020 2020 3c2f 6c69 3e0a 2020 2020  .     </li>.    
+000004a0: 3c2f 756c 3e0a 2020 203c 2f64 6976 3e0a  </ul>.   </div>.
+000004b0: 2020 203c 6275 7474 6f6e 2063 6c61 7373     <button class
+000004c0: 3d22 6274 6e20 6274 6e2d 736d 2062 746e  ="btn btn-sm btn
+000004d0: 2d66 756c 6c73 6372 6565 6e2d 6275 7474  -fullscreen-butt
+000004e0: 6f6e 2220 6461 7461 2d62 732d 706c 6163  on" data-bs-plac
+000004f0: 656d 656e 743d 2262 6f74 746f 6d22 2064  ement="bottom" d
+00000500: 6174 612d 6273 2d74 6f67 676c 653d 2274  ata-bs-toggle="t
+00000510: 6f6f 6c74 6970 2220 6f6e 636c 6963 6b3d  ooltip" onclick=
+00000520: 2274 6f67 676c 6546 756c 6c53 6372 6565  "toggleFullScree
+00000530: 6e28 2922 2074 6974 6c65 3d22 4675 6c6c  n()" title="Full
+00000540: 7363 7265 656e 206d 6f64 6522 3e0a 2020  screen mode">.  
+00000550: 2020 3c73 7061 6e20 636c 6173 733d 2262    <span class="b
+00000560: 746e 5f5f 6963 6f6e 2d63 6f6e 7461 696e  tn__icon-contain
+00000570: 6572 223e 0a20 2020 2020 3c69 2063 6c61  er">.     <i cla
+00000580: 7373 3d22 6661 7320 6661 2d65 7870 616e  ss="fas fa-expan
+00000590: 6422 3e0a 2020 2020 203c 2f69 3e0a 2020  d">.     </i>.  
+000005a0: 2020 3c2f 7370 616e 3e0a 2020 203c 2f62    </span>.   </b
+000005b0: 7574 746f 6e3e 0a20 2020 3c73 6372 6970  utton>.   <scrip
+000005c0: 743e 0a20 2020 2064 6f63 756d 656e 742e  t>.    document.
+000005d0: 7772 6974 6528 600a 2020 3c62 7574 746f  write(`.  <butto
+000005e0: 6e20 636c 6173 733d 2274 6865 6d65 2d73  n class="theme-s
+000005f0: 7769 7463 682d 6275 7474 6f6e 2062 746e  witch-button btn
+00000600: 2062 746e 2d73 6d20 6274 6e2d 6f75 746c   btn-sm btn-outl
+00000610: 696e 652d 7072 696d 6172 7920 6e61 7662  ine-primary navb
+00000620: 6172 2d62 746e 2072 6f75 6e64 6564 2d63  ar-btn rounded-c
+00000630: 6972 636c 6522 2074 6974 6c65 3d22 6c69  ircle" title="li
+00000640: 6768 742f 6461 726b 2220 6172 6961 2d6c  ght/dark" aria-l
+00000650: 6162 656c 3d22 6c69 6768 742f 6461 726b  abel="light/dark
+00000660: 2220 6461 7461 2d62 732d 706c 6163 656d  " data-bs-placem
+00000670: 656e 743d 2262 6f74 746f 6d22 2064 6174  ent="bottom" dat
+00000680: 612d 6273 2d74 6f67 676c 653d 2274 6f6f  a-bs-toggle="too
+00000690: 6c74 6970 223e 0a20 2020 203c 7370 616e  ltip">.    <span
+000006a0: 2063 6c61 7373 3d22 7468 656d 652d 7377   class="theme-sw
+000006b0: 6974 6368 2220 6461 7461 2d6d 6f64 653d  itch" data-mode=
+000006c0: 226c 6967 6874 223e 3c69 2063 6c61 7373  "light"><i class
+000006d0: 3d22 6661 2d73 6f6c 6964 2066 612d 7375  ="fa-solid fa-su
+000006e0: 6e22 3e3c 2f69 3e3c 2f73 7061 6e3e 0a20  n"></i></span>. 
+000006f0: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+00000700: 7468 656d 652d 7377 6974 6368 2220 6461  theme-switch" da
+00000710: 7461 2d6d 6f64 653d 2264 6172 6b22 3e3c  ta-mode="dark"><
+00000720: 6920 636c 6173 733d 2266 612d 736f 6c69  i class="fa-soli
+00000730: 6420 6661 2d6d 6f6f 6e22 3e3c 2f69 3e3c  d fa-moon"></i><
+00000740: 2f73 7061 6e3e 0a20 2020 203c 7370 616e  /span>.    <span
+00000750: 2063 6c61 7373 3d22 7468 656d 652d 7377   class="theme-sw
+00000760: 6974 6368 2220 6461 7461 2d6d 6f64 653d  itch" data-mode=
+00000770: 2261 7574 6f22 3e3c 6920 636c 6173 733d  "auto"><i class=
+00000780: 2266 612d 736f 6c69 6420 6661 2d63 6972  "fa-solid fa-cir
+00000790: 636c 652d 6861 6c66 2d73 7472 6f6b 6522  cle-half-stroke"
+000007a0: 3e3c 2f69 3e3c 2f73 7061 6e3e 0a20 203c  ></i></span>.  <
+000007b0: 2f62 7574 746f 6e3e 0a60 293b 0a20 2020  /button>.`);.   
+000007c0: 3c2f 7363 7269 7074 3e0a 2020 203c 7363  </script>.   <sc
+000007d0: 7269 7074 3e0a 2020 2020 646f 6375 6d65  ript>.    docume
+000007e0: 6e74 2e77 7269 7465 2860 0a20 203c 6275  nt.write(`.  <bu
+000007f0: 7474 6f6e 2063 6c61 7373 3d22 6274 6e20  tton class="btn 
+00000800: 6274 6e2d 736d 206e 6176 6261 722d 6274  btn-sm navbar-bt
+00000810: 6e20 7365 6172 6368 2d62 7574 746f 6e20  n search-button 
+00000820: 7365 6172 6368 2d62 7574 746f 6e5f 5f62  search-button__b
+00000830: 7574 746f 6e22 2074 6974 6c65 3d22 5365  utton" title="Se
+00000840: 6172 6368 2220 6172 6961 2d6c 6162 656c  arch" aria-label
+00000850: 3d22 5365 6172 6368 2220 6461 7461 2d62  ="Search" data-b
+00000860: 732d 706c 6163 656d 656e 743d 2262 6f74  s-placement="bot
+00000870: 746f 6d22 2064 6174 612d 6273 2d74 6f67  tom" data-bs-tog
+00000880: 676c 653d 2274 6f6f 6c74 6970 223e 0a20  gle="tooltip">. 
+00000890: 2020 203c 6920 636c 6173 733d 2266 612d     <i class="fa-
+000008a0: 736f 6c69 6420 6661 2d6d 6167 6e69 6679  solid fa-magnify
+000008b0: 696e 672d 676c 6173 7322 3e3c 2f69 3e0a  ing-glass"></i>.
+000008c0: 2020 3c2f 6275 7474 6f6e 3e0a 6029 3b0a    </button>.`);.
+000008d0: 2020 203c 2f73 6372 6970 743e 0a20 203c     </script>.  <
+000008e0: 2f64 6976 3e0a 203c 2f64 6976 3e0a 3c2f  /div>. </div>.</
+000008f0: 6469 763e 0a                             div>.
```

### Comparing `tskit_book_theme-0.3.2/tests/test_build/test_header_launchbtns.html` & `tskit_book_theme-1.0.1/tests/test_build/test_header_launchbtns.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,59 @@
-<div class="menu-dropdown menu-dropdown-launch-buttons">
- <button aria-label="Launch interactive content" class="headerbtn menu-dropdown__trigger">
+<div class="dropdown dropdown-launch-buttons">
+ <button aria-expanded="false" aria-label="Launch interactive content" class="btn dropdown-toggle" data-bs-toggle="dropdown" type="button">
   <i class="fas fa-rocket">
   </i>
  </button>
- <div class="menu-dropdown__content">
-  <ul>
-   <li>
-    <a class="headerbtn" data-placement="left" data-toggle="tooltip" href="https://mybinder.org/v2/gh/executablebooks/sphinx-book-theme/master?urlpath=lab/tree/TESTPATH/section1/ntbk.ipynb" title="Launch on Binder">
-     <span class="headerbtn__icon-container">
-      <img src="../_static/images/logo_binder.svg"/>
-     </span>
-     <span class="headerbtn__text-container">
-      Binder
-     </span>
-    </a>
-   </li>
-   <li>
-    <a class="headerbtn" data-placement="left" data-toggle="tooltip" href="https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A//github.com/executablebooks/sphinx-book-theme&amp;urlpath=lab/tree/sphinx-book-theme/TESTPATH/section1/ntbk.ipynb&amp;branch=master" title="Launch on JupyterHub">
-     <span class="headerbtn__icon-container">
-      <img src="../_static/images/logo_jupyterhub.svg"/>
-     </span>
-     <span class="headerbtn__text-container">
-      JupyterHub
-     </span>
-    </a>
-   </li>
-   <li>
-    <a class="headerbtn" data-placement="left" data-toggle="tooltip" href="https://colab.research.google.com/github/executablebooks/sphinx-book-theme/blob/master/TESTPATH/section1/ntbk.ipynb" title="Launch on Colab">
-     <span class="headerbtn__icon-container">
-      <img src="../_static/images/logo_colab.png"/>
-     </span>
-     <span class="headerbtn__text-container">
-      Colab
-     </span>
-    </a>
-   </li>
-   <li>
-    <a class="headerbtn" data-placement="left" data-toggle="tooltip" href="https://deepnote.com/launch?url=https%3A%2F%2Fgithub.com%2Fexecutablebooks%2Fsphinx-book-theme%2Fblob%2Fmaster%2FTESTPATH/section1/ntbk.ipynb" title="Launch on Deepnote">
-     <span class="headerbtn__icon-container">
-      <img src="../_static/images/logo_deepnote.svg"/>
-     </span>
-     <span class="headerbtn__text-container">
-      Deepnote
-     </span>
-    </a>
-   </li>
-   <li>
-    <button class="headerbtn headerbtn-launch-thebe" data-placement="left" data-toggle="tooltip" onclick="initThebeSBT()" title="Launch Thebe">
-     <span class="headerbtn__icon-container">
-      <i class="fas fa-play">
-      </i>
-     </span>
-     <span class="headerbtn__text-container">
-      Live Code
-     </span>
-    </button>
-   </li>
-  </ul>
- </div>
+ <ul class="dropdown-menu">
+  <li>
+   <a class="btn btn-sm dropdown-item" data-bs-placement="left" data-bs-toggle="tooltip" href="https://mybinder.org/v2/gh/executablebooks/sphinx-book-theme/master?urlpath=lab/tree/TESTPATH/section1/ntbk.ipynb" target="_blank" title="Launch onBinder">
+    <span class="btn__icon-container">
+     <img src="../_static/images/logo_binder.svg"/>
+    </span>
+    <span class="btn__text-container">
+     Binder
+    </span>
+   </a>
+  </li>
+  <li>
+   <a class="btn btn-sm dropdown-item" data-bs-placement="left" data-bs-toggle="tooltip" href="https://datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A//github.com/executablebooks/sphinx-book-theme&amp;urlpath=lab/tree/sphinx-book-theme/TESTPATH/section1/ntbk.ipynb&amp;branch=master" target="_blank" title="Launch onJupyterHub">
+    <span class="btn__icon-container">
+     <img src="../_static/images/logo_jupyterhub.svg"/>
+    </span>
+    <span class="btn__text-container">
+     JupyterHub
+    </span>
+   </a>
+  </li>
+  <li>
+   <a class="btn btn-sm dropdown-item" data-bs-placement="left" data-bs-toggle="tooltip" href="https://colab.research.google.com/github/executablebooks/sphinx-book-theme/blob/master/TESTPATH/section1/ntbk.ipynb" target="_blank" title="Launch onColab">
+    <span class="btn__icon-container">
+     <img src="../_static/images/logo_colab.png"/>
+    </span>
+    <span class="btn__text-container">
+     Colab
+    </span>
+   </a>
+  </li>
+  <li>
+   <a class="btn btn-sm dropdown-item" data-bs-placement="left" data-bs-toggle="tooltip" href="https://deepnote.com/launch?url=https%3A%2F%2Fgithub.com%2Fexecutablebooks%2Fsphinx-book-theme%2Fblob%2Fmaster%2FTESTPATH/section1/ntbk.ipynb" target="_blank" title="Launch onDeepnote">
+    <span class="btn__icon-container">
+     <img src="../_static/images/logo_deepnote.svg"/>
+    </span>
+    <span class="btn__text-container">
+     Deepnote
+    </span>
+   </a>
+  </li>
+  <li>
+   <button class="btn btn-sm btn-launch-thebe dropdown-item" data-bs-placement="left" data-bs-toggle="tooltip" onclick="initThebeSBT()" title="Launch Thebe">
+    <span class="btn__icon-container">
+     <i class="fas fa-play">
+     </i>
+    </span>
+    <span class="btn__text-container">
+     Live Code
+    </span>
+   </button>
+  </li>
+ </ul>
 </div>
```

### Comparing `tskit_book_theme-0.3.2/tests/test_build/test_sidenote.html` & `tskit_book_theme-1.0.1/tests/test_build/test_sidenote.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <section id="sidenotes">
  <h2>
   <span class="section-number">
    2.1.
   </span>
   Sidenotes
-  <a class="headerlink" href="#sidenotes" title="Permalink to this headline">
+  <a class="headerlink" href="#sidenotes" title="Permalink to this heading">
    #
   </a>
  </h2>
  <p>
   Some text to test out one sidenote
   <label class="margin-toggle" for="sidenote-role-1">
    <span id="id1">
@@ -33,11 +33,18 @@
    </span>
   </label>
   <input class="margin-toggle" id="sidenote-role-3" name="sidenote-role-3" type="checkbox"/>
   <span class="sidenote">
    <sup>
     3
    </sup>
-   This is another sidenote.
+   This is
+   <em>
+    another
+   </em>
+   <strong>
+    sidenote
+   </strong>
+   .
   </span>
  </p>
 </section>
```

### Comparing `tskit_book_theme-0.3.2/tests/test_locale_convert.py` & `tskit_book_theme-1.0.1/tests/test_locale_convert.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from tskit_book_theme._compile_translations import convert_json
+from sphinx_book_theme._compile_translations import convert_json
 
 
 def test_convert(tmp_path, monkeypatch):
     # Generate folder structures needed
     path_translation = tmp_path / "assets" / "translations"
     path_jsons = path_translation / "jsons"
-    path_compiled = tmp_path / "theme" / "tskit_book_theme" / "static" / "locales"
+    path_compiled = tmp_path / "theme" / "sphinx_book_theme" / "static" / "locales"
     path_jsons.mkdir(parents=True)
     (path_jsons / "test.json").write_text(
         '[{"language":"English","symbol":"en","text":"Text"},'
         '{"language":"Other","symbol":"ot","text":"Translate"}]'
     )
     monkeypatch.setattr("subprocess.check_call", lambda args: None)
     convert_json(path_translation)
```

### Comparing `tskit_book_theme-0.3.2/tox.ini` & `tskit_book_theme-1.0.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # To rebuild the tox environment, for example when dependencies change, use
 # `tox -r`
 
 # Note: if the following error is encountered: `ImportError while loading conftest`
 # then then deleting compiled files has been found to fix it: `find . -name \*.pyc -delete`
 
 [tox]
-envlist = py39-sphinx4
+envlist = py39-sphinx6
 
 [testenv]
 usedevelop=true
 passenv = TERM  # To make terminal coloring / other variables pass through
 
 [testenv:py{37,38,39}-pre-commit]
 extras = code_style
@@ -39,13 +39,13 @@
 extras =
     doc
 deps =
     sphinx-theme-builder[cli]
 commands =
     stb serve docs --open-browser
 
-[testenv:py{37,38,39}-sphinx{3,4}]
+[testenv:py{37,38,39}-sphinx{5,6}]
 extras = test
 deps =
-    sphinx3: sphinx>=3,<4
-    sphinx4: sphinx>=4,<5
+    sphinx5: sphinx>=5,<6
+    sphinx6: sphinx>=6,<7
 commands = pytest {posargs}
```

### Comparing `tskit_book_theme-0.3.2/webpack.config.js` & `tskit_book_theme-1.0.1/webpack.config.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Webpack configuration for tskit-book-theme
+// Webpack configuration for sphinx-book-theme
 const {
     resolve
 } = require("path");
 const OptimizeCssAssetsPlugin = require("optimize-css-assets-webpack-plugin");
 const TerserPlugin = require("terser-webpack-plugin");
 const dedent = require("dedent");
 
@@ -11,15 +11,15 @@
     exec
 } = require("child_process");
 exec("python src/tskit_book_theme/_compile_translations.py");
 
 // Paths for various assets (sources and destinations)
 const staticPath = resolve(
     __dirname,
-    "src/tskit_book_theme/theme/tskit_book_theme/static"
+    "src/tskit_book_theme/theme/tskit_book_theme/static",
 );
 
 module.exports = {
     mode: "production",
     devtool: "source-map",
     entry: {
         "tskit-book-theme": ["./src/tskit_book_theme/assets/scripts/index.js"],
```

### Comparing `tskit_book_theme-0.3.2/PKG-INFO` & `tskit_book_theme-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tskit-book-theme
-Version: 0.3.2
-Summary: A clean book theme for tskit ecosystem projects
-Maintainer-Email: Chris Holdgraf <choldgraf@gmail.com>
+Version: 1.0.1
+Summary: A book theme for tskit projects
+Maintainer-Email: Ben Jeffery <ben.jeffery@bdi.ox.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Chris Holdgraf
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -34,91 +34,90 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Project-URL: Repository, https://github.com/executablebooks/tskit-book-theme
+Project-URL: Documentation, https://tskit.dev
 Requires-Python: >=3.7
-Requires-Dist: sphinx<5,>=3
-Requires-Dist: pydata-sphinx-theme~=0.8.0
-Requires-Dist: pyyaml
-Requires-Dist: pre-commit~=2.7.0; extra == "code_style"
-Requires-Dist: ablog~=0.10.13; extra == "doc"
+Requires-Dist: sphinx<7,>=4
+Requires-Dist: pydata-sphinx-theme>=0.13.3
+Requires-Dist: pre-commit; extra == "code-style"
+Requires-Dist: ablog; extra == "doc"
 Requires-Dist: ipywidgets; extra == "doc"
 Requires-Dist: folium; extra == "doc"
 Requires-Dist: numpy; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
-Requires-Dist: myst-nb~=0.13.2; extra == "doc"
+Requires-Dist: myst-nb; extra == "doc"
 Requires-Dist: nbclient; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
 Requires-Dist: plotly; extra == "doc"
-Requires-Dist: sphinx~=4.0; extra == "doc"
 Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-examples; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
-Requires-Dist: sphinx-tabs; extra == "doc"
-Requires-Dist: sphinx-togglebutton>=0.2.1; extra == "doc"
-Requires-Dist: sphinx-thebe>=0.1.1; extra == "doc"
-Requires-Dist: sphinxcontrib-bibtex~=2.2; extra == "doc"
+Requires-Dist: sphinx-tabs<=3.4.0; extra == "doc"
+Requires-Dist: docutils==0.17.1; extra == "doc"
+Requires-Dist: sphinx-togglebutton; extra == "doc"
+Requires-Dist: sphinx-thebe; extra == "doc"
+Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
 Requires-Dist: sphinxcontrib-youtube; extra == "doc"
 Requires-Dist: sphinxext-opengraph; extra == "doc"
-Requires-Dist: beautifulsoup4<5,>=4.6.1; extra == "test"
+Requires-Dist: beautifulsoup4; extra == "test"
 Requires-Dist: coverage; extra == "test"
-Requires-Dist: myst-nb~=0.13.2; extra == "test"
-Requires-Dist: pytest~=6.0.1; extra == "test"
+Requires-Dist: myst-nb; extra == "test"
+Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-regressions~=2.0.1; extra == "test"
+Requires-Dist: pytest-regressions; extra == "test"
 Requires-Dist: sphinx_thebe; extra == "test"
 Provides-Extra: code_style
 Provides-Extra: doc
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
-# tskit-book-theme
+# sphinx-book-theme
 
 [![codecov][codecov-badge]][codecov-link] [![Documentation Status][rtd-badge]][rtd-link] [![PyPI][pypi-badge]][pypi-link]
 
-**An interactive book theme for tskit ecosystem projects**.
-
-Forked from sphinx-book-theme.
+**An interactive book theme for Sphinx**.
 
 This is a lightweight Sphinx theme designed to mimic the look-and-feel of an
 interactive book. It has the following primary features:
 
-* **Bootstrap 4**
+* **Bootstrap 5**
   for visual elements and functionality.
 * **Flexible content layout** that is inspired by beautiful online books,
   such as [the Edward Tufte CSS guide](https://edwardtufte.github.io/tufte-css/)
 * **Visual classes designed for Jupyter Notebooks**. Cell inputs, outputs,
   and interactive functionality are all supported.
 * **Launch buttons for online interactivity**. For pages that are built with
   computational material, connect your site to an online BinderHub for interactive content.
 
 ## Get started
 
-To get started with `tskit-book-theme`, first install it with `pip`:
+To get started with `sphinx-book-theme`, first install it with `pip`:
 
 ```
-pip install tskit-book-theme
+pip install sphinx-book-theme
 ```
 
 then, activate the theme in your Sphinx configuration (`conf.py`):
 
 ```
 ...
-html_theme = "tskit_book_theme"
+html_theme = "sphinx_book_theme"
 ...
 ```
 
 This will activate the Sphinx Book Theme for your documentation. Note that you may
 need to change your `html_theme_options` configuration depending on your previous
 theme. See the pages to the left for information about what you can configure with
-`tskit-book-theme`.
+`sphinx-book-theme`.
 
 ## Documentation
 
 See [the Sphinx Book Theme documentation](https://sphinx-book-theme.readthedocs.io/en/latest/)
 for more information.
 
 [codecov-badge]: https://codecov.io/gh/executablebooks/sphinx-book-theme/branch/master/graph/badge.svg
```

