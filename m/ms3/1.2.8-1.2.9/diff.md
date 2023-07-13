# Comparing `tmp/ms3-1.2.8.tar.gz` & `tmp/ms3-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms3-1.2.8.tar", last modified: Tue May  2 15:36:47 2023, max compression
+gzip compressed data, was "ms3-1.2.9.tar", last modified: Thu May 11 15:37:56 2023, max compression
```

## Comparing `ms3-1.2.8.tar` & `ms3-1.2.9.tar`

### file list

```diff
@@ -1,317 +1,317 @@
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.910134 ms3-1.2.8/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      586 2020-05-03 17:52:04.000000 ms3-1.2.8/.coveragerc
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/.github/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.703466 ms3-1.2.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      752 2023-05-02 08:27:28.000000 ms3-1.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      599 2023-05-02 08:27:28.000000 ms3-1.2.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.706799 ms3-1.2.8/.github/workflows/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      669 2023-01-28 14:33:36.000000 ms3-1.2.8/.github/workflows/draft-pdf.yml
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      541 2023-05-02 08:27:28.000000 ms3-1.2.8/.gitignore
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2020-07-06 00:26:02.000000 ms3-1.2.8/AUTHORS.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    23371 2023-05-02 15:33:29.000000 ms3-1.2.8/CHANGELOG.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    34500 2020-05-07 11:55:51.000000 ms3-1.2.8/LICENSE.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-05-02 15:36:47.910134 ms3-1.2.8/PKG-INFO
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4026 2023-05-01 12:14:08.000000 ms3-1.2.8/README.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2094 2022-12-15 11:35:36.000000 ms3-1.2.8/codemeta.json
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.713466 ms3-1.2.8/docs/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/.nojekyll
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7593 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/Makefile
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-01-28 14:33:36.000000 ms3-1.2.8/docs/README.md
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.713466 ms3-1.2.8/docs/_intersphinx/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      646 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/_intersphinx/bs4_objects.inv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1799 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/_intersphinx/bs4_objects.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.713466 ms3-1.2.8/docs/_static/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       18 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/_static/.gitignore
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/authors.rst
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.716799 ms3-1.2.8/docs/build/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.buildinfo
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.736800 ms3-1.2.8/docs/build/.doctrees/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.736800 ms3-1.2.8/docs/build/.doctrees/api/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2579 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/api/modules.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   619252 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/api/ms3.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3406 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/authors.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6354 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/changelog.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 10423401 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/environment.pickle
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14745 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/index.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7547 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/install.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4679 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/intro.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96686 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/license.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35413 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/manual.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4590 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.doctrees/quick.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/.nojekyll
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.760133 ms3-1.2.8/docs/build/doctrees/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4366 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/README.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3594 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/authors.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154262 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/changelog.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 13487965 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/environment.pickle
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35248 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/index.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7812 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/install.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97335 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/license.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.783466 ms3-1.2.8/docs/build/doctrees/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 14283956 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/manual/index.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.806800 ms3-1.2.8/docs/build/doctrees/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79212 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/old_src/quick_old.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    78946 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/quick.doctree
--rw-r--r--   0 hentsche  (1001) hentsche  (1001) 17416423 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/doctrees/reference.doctree
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.813467 ms3-1.2.8/docs/build/html/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/.buildinfo
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2023-03-18 10:45:36.000000 ms3-1.2.8/docs/build/html/.nojekyll
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15846 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/README.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.816800 ms3-1.2.8/docs/build/html/_modules/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15440 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/index.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.826800 ms3-1.2.8/docs/build/html/_modules/ms3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   121982 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/annotations.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   562760 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/bs4_parser.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   585871 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/corpus.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   119721 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/expand_dcml.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   299877 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/parse.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   337630 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/piece.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   326103 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/score.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   264338 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/transformations.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   930043 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/utils.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   139939 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/ms3/view.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    63215 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_modules/re.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.826800 ms3-1.2.8/docs/build/html/_sources/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_sources/README.md.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/html/_sources/authors.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.8/docs/build/html/_sources/install.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/build/html/_sources/license.rst.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.830133 ms3-1.2.8/docs/build/html/_sources/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/manual/index.md.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.830133 ms3-1.2.8/docs/build/html/_sources/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/old_src/quick_old.rst.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_sources/quick.md.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-05-01 12:14:08.000000 ms3-1.2.8/docs/build/html/_sources/reference.rst.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.836800 ms3-1.2.8/docs/build/html/_static/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4418 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14621 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/_static/basic.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4472 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/doctools.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      439 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      286 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/file.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   288580 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    89501 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/jquery.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/jupyter-sphinx.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4758 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/language_data.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/minus.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    39364 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/plus.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14668 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/pygments.css
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.836800 ms3-1.2.8/docs/build/html/_static/scripts/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    86398 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5229 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18215 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/searchtools.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4712 2023-01-21 10:04:25.000000 ms3-1.2.8/docs/build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.840133 ms3-1.2.8/docs/build/html/_static/styles/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   144661 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    58614 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      106 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/styles/theme.css
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    68420 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19530 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/underscore.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/docs/build/html/_static/vendor/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.840133 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7427 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.840133 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   101709 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.843467 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   181264 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   105112 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60236 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24028 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   389948 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154840 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10084 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4776 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1845 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16465 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/authors.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    69269 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/changelog.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79722 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/genindex.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    31724 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19975 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/install.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    53099 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/license.html
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.843467 ms3-1.2.8/docs/build/html/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   338361 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/manual/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7352 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/objects.inv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.846800 ms3-1.2.8/docs/build/html/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60388 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/old_src/quick_old.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17021 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/py-modindex.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    47347 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/quick.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1763633 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/reference.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15656 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/search.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130526 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/html/searchindex.js
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.846800 ms3-1.2.8/docs/build/jupyter_execute/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.846800 ms3-1.2.8/docs/build/jupyter_execute/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   346220 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/jupyter_execute/manual/index.ipynb
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    49220 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/build/jupyter_execute/quick.ipynb
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/changelog.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      135 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/columns.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10588 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/conf.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   137117 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/cujus.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.850133 ms3-1.2.8/docs/examples/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      134 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/access_score_info.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       47 2021-10-16 12:40:03.000000 ms3-1.2.8/docs/examples/parse_directory.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       64 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_directory_mscx.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       58 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_directory_xml.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      199 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_key.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      173 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_other_directory.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-01-02 20:31:46.000000 ms3-1.2.8/docs/examples/parse_single_score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       71 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/index.html
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/index.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.8/docs/install.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/license.rst
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.850133 ms3-1.2.8/docs/manual/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      715 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/corpus_after
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      174 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/corpus_before
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/index.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      488 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/manual/out
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9940 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/ms3_architecture.drawio
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   218314 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/ms3_architecture.png
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96827 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/o_quam.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.850133 ms3-1.2.8/docs/old_src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15949 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/old_src/quick_old.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/old_src/quick_old.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   163542 2020-11-02 16:20:48.000000 ms3-1.2.8/docs/quae.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-05-02 08:27:28.000000 ms3-1.2.8/docs/quick.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-05-01 12:14:08.000000 ms3-1.2.8/docs/reference.rst
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       86 2023-03-23 18:04:34.000000 ms3-1.2.8/docs/requirements.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   115684 2021-10-20 14:43:53.000000 ms3-1.2.8/docs/stabat.mscx
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.853467 ms3-1.2.8/new_tests/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7378 2023-05-02 08:27:28.000000 ms3-1.2.8/new_tests/conftest.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.700133 ms3-1.2.8/new_tests/inferred_labels/
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.856800 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19047 2022-12-15 11:35:36.000000 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   332296 2022-12-15 11:35:36.000000 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317949 2022-12-15 11:35:36.000000 ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      466 2023-05-01 13:23:04.000000 ms3-1.2.8/new_tests/parse_script.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-05-02 08:27:28.000000 ms3-1.2.8/new_tests/test_cli.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      403 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_docs_examples.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    12424 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_extract.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6352 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3744 2023-01-02 20:31:46.000000 ms3-1.2.8/new_tests/test_score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      823 2023-01-17 21:52:55.000000 ms3-1.2.8/new_tests/test_transformations.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.873467 ms3-1.2.8/old_tests/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   388689 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/05_symph_fant_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      959 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/05_symph_fant_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   100539 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/05_symph_fant_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   488895 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7268 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2636 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   155973 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/76CASM34A33UM_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4361 2023-01-02 20:31:46.000000 ms3-1.2.8/old_tests/ALL_WARNINGS
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   256806 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/BWV_0815_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/BWV_0815_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/BWV_0815_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16417 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/D973deutscher01_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/D973deutscher01_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/D973deutscher01_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1490215 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      330 2023-01-02 20:31:46.000000 ms3-1.2.8/old_tests/IGNORED_WARNINGS
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   431522 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14480 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4560 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96112 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/K281-3_notes.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.883467 ms3-1.2.8/old_tests/MS3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1041665 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/05_symph_fant.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1034028 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/76CASM34A33UM.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   787637 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/BWV_0815.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    54002 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/D973deutscher01.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   701525 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   807371 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/MS3/K281-3.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   259369 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/MS3/stabat_03_coloured.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      624 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/README.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      224 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/conftest.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.886800 ms3-1.2.8/old_tests/harmonies/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9855 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    21459 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3905 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/harmonies/stabat_03_coloured.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.886800 ms3-1.2.8/old_tests/measures/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      889 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/05_symph_fant.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6504 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/BWV_0815.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      684 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/D973deutscher01.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2706 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4411 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/measures/stabat_03_coloured.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5885 2023-05-02 08:27:28.000000 ms3-1.2.8/old_tests/metadata.tsv
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.890133 ms3-1.2.8/old_tests/notes/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    74055 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/05_symph_fant.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   112389 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/76CASM34A33UM.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   102317 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/BWV_0815.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6173 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/D973deutscher01.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   230316 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    70952 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/K281-3.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/notes/stabat_03_coloured.tsv
--rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)       45 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/parse_original.sh
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      750 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/paths1.json
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      844 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/paths2.json
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.893467 ms3-1.2.8/old_tests/repeat_dummies/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6909 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/repeat_dummies/repeats0.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6493 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/repeat_dummies/repeats1.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7376 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/repeat_dummies/repeats2.mscx
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   135170 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_events.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4822 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/stabat_03_coloured_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2207 2023-02-18 19:40:30.000000 ms3-1.2.8/old_tests/test_parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      712 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_repeats.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.900134 ms3-1.2.8/old_tests/test_results/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      921 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/05_symph_fant_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    98388 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/05_symph_fant_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7089 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/76CASM34A33UM_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2536 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/76CASM34A33UM_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   152525 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/76CASM34A33UM_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/BWV_0815_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/BWV_0815_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/D973deutscher01_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/D973deutscher01_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14099 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/K281-3_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4391 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/K281-3_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    94030 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/K281-3_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4731 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/stabat_03_coloured_labels.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      758 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/stabat_03_coloured_measures.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24478 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_results/stabat_03_coloured_notes.tsv
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4777 2022-12-15 11:35:36.000000 ms3-1.2.8/old_tests/test_score.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.900134 ms3-1.2.8/paper/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17950 2023-05-01 12:14:08.000000 ms3-1.2.8/paper/paper.bib
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4605 2023-05-01 12:14:08.000000 ms3-1.2.8/paper/paper.md
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   200690 2023-01-28 14:33:36.000000 ms3-1.2.8/paper/paper.pdf
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1364 2023-05-02 15:36:47.910134 ms3-1.2.8/setup.cfg
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      567 2020-05-03 17:52:04.000000 ms3-1.2.8/setup.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.900134 ms3-1.2.8/src/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:27:59.000000 ms3-1.2.8/src/__init__.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.906800 ms3-1.2.8/src/ms3/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1006 2023-02-18 19:40:30.000000 ms3-1.2.8/src/ms3/__init__.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2402 2023-02-18 19:40:30.000000 ms3-1.2.8/src/ms3/_typing.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24943 2023-01-12 10:36:52.000000 ms3-1.2.8/src/ms3/annotations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41608 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/bs4_measures.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130482 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/bs4_parser.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41211 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/cli.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   151740 2023-05-02 15:30:05.000000 ms3-1.2.8/src/ms3/corpus.py
--rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)    26692 2023-01-02 20:31:46.000000 ms3-1.2.8/src/ms3/expand_dcml.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8416 2023-01-02 20:31:46.000000 ms3-1.2.8/src/ms3/ferocious_names.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18415 2023-03-18 08:04:35.000000 ms3-1.2.8/src/ms3/logger.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15652 2023-05-02 15:30:05.000000 ms3-1.2.8/src/ms3/operations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    83765 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/parse.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    82901 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/piece.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97681 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/score.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    67393 2023-05-02 08:27:28.000000 ms3-1.2.8/src/ms3/transformations.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)   219679 2023-05-02 15:33:29.000000 ms3-1.2.8/src/ms3/utils.py
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)    29890 2023-05-02 15:30:05.000000 ms3-1.2.8/src/ms3/view.py
-drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-02 15:36:47.910134 ms3-1.2.8/src/ms3.egg-info/
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/PKG-INFO
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9420 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/SOURCES.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/dependency_links.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)       36 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/entry_points.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-28 13:53:29.000000 ms3-1.2.8/src/ms3.egg-info/not-zip-safe
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/requires.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)        4 2023-05-02 15:36:47.000000 ms3-1.2.8/src/ms3.egg-info/top_level.txt
--rw-r--r--   0 hentsche  (1001) hentsche  (1001)      318 2020-05-03 17:52:04.000000 ms3-1.2.8/tox.ini
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.183729 ms3-1.2.9/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      586 2020-05-03 17:52:04.000000 ms3-1.2.9/.coveragerc
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.083728 ms3-1.2.9/.github/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.090395 ms3-1.2.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      752 2023-05-02 08:27:28.000000 ms3-1.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      599 2023-05-02 08:27:28.000000 ms3-1.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.090395 ms3-1.2.9/.github/workflows/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      669 2023-01-28 14:33:36.000000 ms3-1.2.9/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      541 2023-05-02 08:27:28.000000 ms3-1.2.9/.gitignore
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2020-07-06 00:26:02.000000 ms3-1.2.9/AUTHORS.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    23601 2023-05-11 15:34:43.000000 ms3-1.2.9/CHANGELOG.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    34500 2020-05-07 11:55:51.000000 ms3-1.2.9/LICENSE.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-05-11 15:37:56.183729 ms3-1.2.9/PKG-INFO
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4026 2023-05-11 14:47:37.000000 ms3-1.2.9/README.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2094 2022-12-15 11:35:36.000000 ms3-1.2.9/codemeta.json
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.093728 ms3-1.2.9/docs/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/.nojekyll
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7593 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/Makefile
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-01-28 14:33:36.000000 ms3-1.2.9/docs/README.md
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.093728 ms3-1.2.9/docs/_intersphinx/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      646 2021-10-20 14:43:53.000000 ms3-1.2.9/docs/_intersphinx/bs4_objects.inv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1799 2021-10-20 14:43:53.000000 ms3-1.2.9/docs/_intersphinx/bs4_objects.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.093728 ms3-1.2.9/docs/_static/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       18 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/_static/.gitignore
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/authors.rst
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.093728 ms3-1.2.9/docs/build/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.buildinfo
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.103728 ms3-1.2.9/docs/build/.doctrees/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.103728 ms3-1.2.9/docs/build/.doctrees/api/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2579 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/api/modules.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   619252 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/api/ms3.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3406 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/authors.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6354 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/changelog.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 10423401 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14745 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/index.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7547 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/install.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4679 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/intro.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96686 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/license.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35413 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/manual.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4590 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.doctrees/quick.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/.nojekyll
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.117062 ms3-1.2.9/docs/build/doctrees/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4366 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/doctrees/README.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3594 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/doctrees/authors.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154262 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/doctrees/changelog.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 13487965 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    35248 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/doctrees/index.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7812 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/doctrees/install.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97335 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/doctrees/license.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.130395 ms3-1.2.9/docs/build/doctrees/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 14283956 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/doctrees/manual/index.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.140395 ms3-1.2.9/docs/build/doctrees/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79212 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/doctrees/old_src/quick_old.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    78946 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/doctrees/quick.doctree
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001) 17416423 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/doctrees/reference.doctree
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.143729 ms3-1.2.9/docs/build/html/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      230 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/.buildinfo
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2023-03-18 10:45:36.000000 ms3-1.2.9/docs/build/html/.nojekyll
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15846 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/README.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.143729 ms3-1.2.9/docs/build/html/_modules/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15440 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/index.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.147062 ms3-1.2.9/docs/build/html/_modules/ms3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   121982 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/annotations.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   562760 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/bs4_parser.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   585871 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/corpus.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   119721 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/expand_dcml.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   299877 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/parse.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   337630 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/piece.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   326103 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/score.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   264338 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/transformations.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   930043 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/utils.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   139939 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/ms3/view.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    63215 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_modules/re.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.150395 ms3-1.2.9/docs/build/html/_sources/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      201 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_sources/README.md.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       41 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/html/_sources/authors.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.9/docs/build/html/_sources/install.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/build/html/_sources/license.rst.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.150395 ms3-1.2.9/docs/build/html/_sources/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/html/_sources/manual/index.md.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.150395 ms3-1.2.9/docs/build/html/_sources/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/html/_sources/old_src/quick_old.rst.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/html/_sources/quick.md.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/_sources/reference.rst.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.153729 ms3-1.2.9/docs/build/html/_static/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4418 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14621 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/build/html/_static/basic.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4472 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/doctools.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      439 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      286 2023-01-21 10:04:25.000000 ms3-1.2.9/docs/build/html/_static/file.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   288580 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    89501 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/jquery.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/jupyter-sphinx.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4758 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/language_data.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.9/docs/build/html/_static/minus.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    39364 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       90 2023-01-21 10:04:25.000000 ms3-1.2.9/docs/build/html/_static/plus.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14668 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/pygments.css
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.153729 ms3-1.2.9/docs/build/html/_static/scripts/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    86398 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5229 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18215 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4712 2023-01-21 10:04:25.000000 ms3-1.2.9/docs/build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.153729 ms3-1.2.9/docs/build/html/_static/styles/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   144661 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    58614 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      106 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    68420 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19530 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/underscore.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.087061 ms3-1.2.9/docs/build/html/_static/vendor/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.087061 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.153729 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7427 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.153729 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   101709 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.153729 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   181264 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   105112 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60236 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24028 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   389948 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   154840 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10084 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4776 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1845 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16465 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/authors.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    69269 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/changelog.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    79722 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/genindex.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    31724 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19975 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/install.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    53099 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/license.html
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.153729 ms3-1.2.9/docs/build/html/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   338361 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/manual/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7352 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/objects.inv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.157062 ms3-1.2.9/docs/build/html/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    60388 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/old_src/quick_old.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17021 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/py-modindex.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    47347 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/quick.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1763633 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/reference.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15656 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/search.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130526 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/html/searchindex.js
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.157062 ms3-1.2.9/docs/build/jupyter_execute/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.157062 ms3-1.2.9/docs/build/jupyter_execute/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   346220 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/jupyter_execute/manual/index.ipynb
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    49220 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/build/jupyter_execute/quick.ipynb
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       43 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/changelog.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      135 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/columns.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    10588 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/conf.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   137117 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/cujus.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.157062 ms3-1.2.9/docs/examples/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      134 2023-01-02 20:31:46.000000 ms3-1.2.9/docs/examples/access_score_info.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       47 2021-10-16 12:40:03.000000 ms3-1.2.9/docs/examples/parse_directory.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       64 2023-01-02 20:31:46.000000 ms3-1.2.9/docs/examples/parse_directory_mscx.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       58 2023-01-02 20:31:46.000000 ms3-1.2.9/docs/examples/parse_directory_xml.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      199 2023-01-02 20:31:46.000000 ms3-1.2.9/docs/examples/parse_key.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      173 2023-01-02 20:31:46.000000 ms3-1.2.9/docs/examples/parse_other_directory.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-01-02 20:31:46.000000 ms3-1.2.9/docs/examples/parse_single_score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       71 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/index.html
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1356 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/index.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1256 2023-01-28 14:33:36.000000 ms3-1.2.9/docs/install.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       67 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/license.rst
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.157062 ms3-1.2.9/docs/manual/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      715 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/manual/corpus_after
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      174 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/manual/corpus_before
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    76626 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/manual/index.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      488 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/manual/out
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9940 2021-10-20 14:43:53.000000 ms3-1.2.9/docs/ms3_architecture.drawio
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   218314 2021-10-20 14:43:53.000000 ms3-1.2.9/docs/ms3_architecture.png
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96827 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/o_quam.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.157062 ms3-1.2.9/docs/old_src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15949 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/old_src/quick_old.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17232 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/old_src/quick_old.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   163542 2020-11-02 16:20:48.000000 ms3-1.2.9/docs/quae.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2619 2023-05-02 08:27:28.000000 ms3-1.2.9/docs/quick.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7126 2023-05-11 14:47:37.000000 ms3-1.2.9/docs/reference.rst
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       86 2023-03-23 18:04:34.000000 ms3-1.2.9/docs/requirements.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   115684 2021-10-20 14:43:53.000000 ms3-1.2.9/docs/stabat.mscx
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.160395 ms3-1.2.9/new_tests/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7378 2023-05-09 15:03:19.000000 ms3-1.2.9/new_tests/conftest.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.087061 ms3-1.2.9/new_tests/inferred_labels/
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.160395 ms3-1.2.9/new_tests/inferred_labels/sweelinck_keyboard/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    19047 2022-12-15 11:35:36.000000 ms3-1.2.9/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   332296 2022-12-15 11:35:36.000000 ms3-1.2.9/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317949 2022-12-15 11:35:36.000000 ms3-1.2.9/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      466 2023-05-11 14:44:13.000000 ms3-1.2.9/new_tests/parse_script.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3019 2023-05-11 14:47:13.000000 ms3-1.2.9/new_tests/test_cli.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      403 2023-01-02 20:31:46.000000 ms3-1.2.9/new_tests/test_docs_examples.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    12424 2023-01-02 20:31:46.000000 ms3-1.2.9/new_tests/test_extract.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6352 2023-01-02 20:31:46.000000 ms3-1.2.9/new_tests/test_parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3744 2023-01-02 20:31:46.000000 ms3-1.2.9/new_tests/test_score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      823 2023-01-17 21:52:55.000000 ms3-1.2.9/new_tests/test_transformations.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.167062 ms3-1.2.9/old_tests/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   388689 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/05_symph_fant_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      959 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/05_symph_fant_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   100539 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/05_symph_fant_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   488895 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/76CASM34A33UM_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7268 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/76CASM34A33UM_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2636 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/76CASM34A33UM_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   155973 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/76CASM34A33UM_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4361 2023-01-02 20:31:46.000000 ms3-1.2.9/old_tests/ALL_WARNINGS
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   256806 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/BWV_0815_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/BWV_0815_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/BWV_0815_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    16417 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/D973deutscher01_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/D973deutscher01_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/D973deutscher01_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1490215 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      330 2023-01-02 20:31:46.000000 ms3-1.2.9/old_tests/IGNORED_WARNINGS
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   431522 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/K281-3_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14480 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/K281-3_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4560 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/K281-3_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    96112 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/K281-3_notes.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.170395 ms3-1.2.9/old_tests/MS3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1041665 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/MS3/05_symph_fant.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)  1034028 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/MS3/76CASM34A33UM.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   787637 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/MS3/BWV_0815.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    54002 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/MS3/D973deutscher01.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   701525 2023-05-02 08:27:28.000000 ms3-1.2.9/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   807371 2023-05-02 08:27:28.000000 ms3-1.2.9/old_tests/MS3/K281-3.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   259369 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/MS3/stabat_03_coloured.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      624 2023-05-02 08:27:28.000000 ms3-1.2.9/old_tests/README.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      224 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/conftest.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.173729 ms3-1.2.9/old_tests/harmonies/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/harmonies/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9855 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    21459 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/harmonies/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3905 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/harmonies/stabat_03_coloured.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.173729 ms3-1.2.9/old_tests/measures/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      889 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/measures/05_symph_fant.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2524 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/measures/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6504 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/measures/BWV_0815.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      684 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/measures/D973deutscher01.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2706 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4411 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/measures/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/measures/stabat_03_coloured.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     5885 2023-05-02 08:27:28.000000 ms3-1.2.9/old_tests/metadata.tsv
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.173729 ms3-1.2.9/old_tests/notes/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    74055 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/notes/05_symph_fant.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   112389 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/notes/76CASM34A33UM.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   102317 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/notes/BWV_0815.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6173 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/notes/D973deutscher01.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   230316 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    70952 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/notes/K281-3.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/notes/stabat_03_coloured.tsv
+-rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)       45 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/parse_original.sh
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      750 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/paths1.json
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      844 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/paths2.json
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.177062 ms3-1.2.9/old_tests/repeat_dummies/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6909 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/repeat_dummies/repeats0.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6493 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/repeat_dummies/repeats1.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7376 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/repeat_dummies/repeats2.mscx
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   135170 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/stabat_03_coloured_events.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4822 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/stabat_03_coloured_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      790 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/stabat_03_coloured_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    25080 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/stabat_03_coloured_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2207 2023-02-18 19:40:30.000000 ms3-1.2.9/old_tests/test_parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      712 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_repeats.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.177062 ms3-1.2.9/old_tests/test_results/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      921 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/05_symph_fant_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    98388 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/05_symph_fant_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7089 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/76CASM34A33UM_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2536 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/76CASM34A33UM_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   152525 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/76CASM34A33UM_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     6833 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/BWV_0815_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   136433 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/BWV_0815_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      697 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/D973deutscher01_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8271 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/D973deutscher01_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     7264 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     3305 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   317634 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    14099 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/K281-3_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4391 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/K281-3_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    94030 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/K281-3_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4731 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/stabat_03_coloured_labels.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      758 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/stabat_03_coloured_measures.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24478 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_results/stabat_03_coloured_notes.tsv
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4777 2022-12-15 11:35:36.000000 ms3-1.2.9/old_tests/test_score.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.177062 ms3-1.2.9/paper/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    17950 2023-05-11 14:47:37.000000 ms3-1.2.9/paper/paper.bib
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4605 2023-05-11 14:47:37.000000 ms3-1.2.9/paper/paper.md
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   200690 2023-01-28 14:33:36.000000 ms3-1.2.9/paper/paper.pdf
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1364 2023-05-11 15:37:56.183729 ms3-1.2.9/setup.cfg
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      567 2020-05-03 17:52:04.000000 ms3-1.2.9/setup.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.180396 ms3-1.2.9/src/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        0 2020-11-02 16:27:59.000000 ms3-1.2.9/src/__init__.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.180396 ms3-1.2.9/src/ms3/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     1006 2023-02-18 19:40:30.000000 ms3-1.2.9/src/ms3/__init__.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     2402 2023-02-18 19:40:30.000000 ms3-1.2.9/src/ms3/_typing.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    24943 2023-01-12 10:36:52.000000 ms3-1.2.9/src/ms3/annotations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41608 2023-05-02 08:27:28.000000 ms3-1.2.9/src/ms3/bs4_measures.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   130482 2023-05-09 15:03:19.000000 ms3-1.2.9/src/ms3/bs4_parser.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    41211 2023-05-09 15:03:19.000000 ms3-1.2.9/src/ms3/cli.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   151740 2023-05-11 14:47:37.000000 ms3-1.2.9/src/ms3/corpus.py
+-rwxr-xr-x   0 hentsche  (1001) hentsche  (1001)    26692 2023-01-02 20:31:46.000000 ms3-1.2.9/src/ms3/expand_dcml.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     8416 2023-01-02 20:31:46.000000 ms3-1.2.9/src/ms3/ferocious_names.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    18703 2023-05-11 15:34:43.000000 ms3-1.2.9/src/ms3/logger.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    15782 2023-05-11 15:34:43.000000 ms3-1.2.9/src/ms3/operations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    83815 2023-05-11 15:34:43.000000 ms3-1.2.9/src/ms3/parse.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    82901 2023-05-02 08:27:28.000000 ms3-1.2.9/src/ms3/piece.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    97681 2023-05-02 08:27:28.000000 ms3-1.2.9/src/ms3/score.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    67393 2023-05-02 08:27:28.000000 ms3-1.2.9/src/ms3/transformations.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)   219771 2023-05-11 15:34:43.000000 ms3-1.2.9/src/ms3/utils.py
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)    29890 2023-05-11 15:34:43.000000 ms3-1.2.9/src/ms3/view.py
+drwxr-xr-x   0 hentsche  (1001) hentsche  (1001)        0 2023-05-11 15:37:56.183729 ms3-1.2.9/src/ms3.egg-info/
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     4564 2023-05-11 15:37:55.000000 ms3-1.2.9/src/ms3.egg-info/PKG-INFO
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)     9420 2023-05-11 15:37:56.000000 ms3-1.2.9/src/ms3.egg-info/SOURCES.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-05-11 15:37:55.000000 ms3-1.2.9/src/ms3.egg-info/dependency_links.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)       36 2023-05-11 15:37:55.000000 ms3-1.2.9/src/ms3.egg-info/entry_points.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        1 2023-04-28 13:53:29.000000 ms3-1.2.9/src/ms3.egg-info/not-zip-safe
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      120 2023-05-11 15:37:55.000000 ms3-1.2.9/src/ms3.egg-info/requires.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)        4 2023-05-11 15:37:55.000000 ms3-1.2.9/src/ms3.egg-info/top_level.txt
+-rw-r--r--   0 hentsche  (1001) hentsche  (1001)      318 2020-05-03 17:52:04.000000 ms3-1.2.9/tox.ini
```

### Comparing `ms3-1.2.8/.coveragerc` & `ms3-1.2.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `ms3-1.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/.github/ISSUE_TEMPLATE/feature_request.md` & `ms3-1.2.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/.github/workflows/draft-pdf.yml` & `ms3-1.2.9/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/.gitignore` & `ms3-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/CHANGELOG.rst` & `ms3-1.2.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
 Changelog
 =========
 
+Version 1.2.9
+=============
+
+* when updating ``README.md``:
+
+  * make 2nd-level heading ``## Overview`` (instead of first-level)
+  * don't output ms3 version (to avoid merge conflicts)
+
+* small bugfixes in ``ms3 review`` command
+
 Version 1.2.8
 =============
 
 * operations.insert_labels_into_score() filters pieces exactly one facet to be inserted (e.g. ``labels``),
   not a fuzzy regex (e.g., which would include ``form_labels`` in the filter)
 
 Version 1.2.7
```

### Comparing `ms3-1.2.8/LICENSE.txt` & `ms3-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/PKG-INFO` & `ms3-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms3
-Version: 1.2.8
+Version: 1.2.9
 Summary: A parser for annotated MuseScore 3 files.
 Home-page: https://github.com/johentsch/ms3
 Author: Johannes Hentschel
 Author-email: johannes.hentschel@epfl.ch
 License: gpl3
 Project-URL: Documentation, https://johentsch.github.io/ms3/
 Platform: any
```

### Comparing `ms3-1.2.8/README.rst` & `ms3-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/codemeta.json` & `ms3-1.2.9/codemeta.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/Makefile` & `ms3-1.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/_intersphinx/bs4_objects.inv` & `ms3-1.2.9/docs/_intersphinx/bs4_objects.inv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/_intersphinx/bs4_objects.txt` & `ms3-1.2.9/docs/_intersphinx/bs4_objects.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/api/modules.doctree` & `ms3-1.2.9/docs/build/.doctrees/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/api/ms3.doctree` & `ms3-1.2.9/docs/build/.doctrees/api/ms3.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/authors.doctree` & `ms3-1.2.9/docs/build/.doctrees/authors.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/changelog.doctree` & `ms3-1.2.9/docs/build/.doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/environment.pickle` & `ms3-1.2.9/docs/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/index.doctree` & `ms3-1.2.9/docs/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/install.doctree` & `ms3-1.2.9/docs/build/.doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/intro.doctree` & `ms3-1.2.9/docs/build/.doctrees/intro.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/license.doctree` & `ms3-1.2.9/docs/build/.doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/manual.doctree` & `ms3-1.2.9/docs/build/.doctrees/manual.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/.doctrees/quick.doctree` & `ms3-1.2.9/docs/build/.doctrees/quick.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/README.doctree` & `ms3-1.2.9/docs/build/doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/authors.doctree` & `ms3-1.2.9/docs/build/doctrees/authors.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/changelog.doctree` & `ms3-1.2.9/docs/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/environment.pickle` & `ms3-1.2.9/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/index.doctree` & `ms3-1.2.9/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/install.doctree` & `ms3-1.2.9/docs/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/license.doctree` & `ms3-1.2.9/docs/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/manual/index.doctree` & `ms3-1.2.9/docs/build/doctrees/manual/index.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/old_src/quick_old.doctree` & `ms3-1.2.9/docs/build/doctrees/old_src/quick_old.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/quick.doctree` & `ms3-1.2.9/docs/build/doctrees/quick.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/doctrees/reference.doctree` & `ms3-1.2.9/docs/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/README.html` & `ms3-1.2.9/docs/build/html/README.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/index.html` & `ms3-1.2.9/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/annotations.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/annotations.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/bs4_parser.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/bs4_parser.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/corpus.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/corpus.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/expand_dcml.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/expand_dcml.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/parse.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/parse.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/piece.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/piece.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/score.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/score.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/transformations.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/transformations.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/utils.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/utils.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/ms3/view.html` & `ms3-1.2.9/docs/build/html/_modules/ms3/view.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_modules/re.html` & `ms3-1.2.9/docs/build/html/_modules/re.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_sources/index.rst.txt` & `ms3-1.2.9/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_sources/install.rst.txt` & `ms3-1.2.9/docs/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_sources/manual/index.md.txt` & `ms3-1.2.9/docs/build/html/_sources/manual/index.md.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_sources/old_src/quick_old.rst.txt` & `ms3-1.2.9/docs/build/html/_sources/old_src/quick_old.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_sources/quick.md.txt` & `ms3-1.2.9/docs/build/html/_sources/quick.md.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_sources/reference.rst.txt` & `ms3-1.2.9/docs/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `ms3-1.2.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/basic.css` & `ms3-1.2.9/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/doctools.js` & `ms3-1.2.9/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/jquery-3.6.0.js` & `ms3-1.2.9/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/jquery.js` & `ms3-1.2.9/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/jupyter-sphinx.css` & `ms3-1.2.9/docs/build/html/_static/jupyter-sphinx.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/language_data.js` & `ms3-1.2.9/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `ms3-1.2.9/docs/build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/pygments.css` & `ms3-1.2.9/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/scripts/bootstrap.js` & `ms3-1.2.9/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `ms3-1.2.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/searchtools.js` & `ms3-1.2.9/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/sphinx_highlight.js` & `ms3-1.2.9/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/styles/bootstrap.css` & `ms3-1.2.9/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `ms3-1.2.9/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/underscore-1.13.1.js` & `ms3-1.2.9/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/underscore.js` & `ms3-1.2.9/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `ms3-1.2.9/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/_static/webpack-macros.html` & `ms3-1.2.9/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/authors.html` & `ms3-1.2.9/docs/build/html/authors.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/changelog.html` & `ms3-1.2.9/docs/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/genindex.html` & `ms3-1.2.9/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/index.html` & `ms3-1.2.9/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/install.html` & `ms3-1.2.9/docs/build/html/install.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/license.html` & `ms3-1.2.9/docs/build/html/license.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/manual/index.html` & `ms3-1.2.9/docs/build/html/manual/index.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/objects.inv` & `ms3-1.2.9/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/old_src/quick_old.html` & `ms3-1.2.9/docs/build/html/old_src/quick_old.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/py-modindex.html` & `ms3-1.2.9/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/quick.html` & `ms3-1.2.9/docs/build/html/quick.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/reference.html` & `ms3-1.2.9/docs/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/search.html` & `ms3-1.2.9/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/html/searchindex.js` & `ms3-1.2.9/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/jupyter_execute/manual/index.ipynb` & `ms3-1.2.9/docs/build/jupyter_execute/manual/index.ipynb`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/build/jupyter_execute/quick.ipynb` & `ms3-1.2.9/docs/build/jupyter_execute/quick.ipynb`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/conf.py` & `ms3-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/cujus.mscx` & `ms3-1.2.9/docs/cujus.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/index.rst` & `ms3-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/install.rst` & `ms3-1.2.9/docs/install.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/manual/corpus_after` & `ms3-1.2.9/docs/manual/corpus_after`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/manual/index.md` & `ms3-1.2.9/docs/manual/index.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/ms3_architecture.drawio` & `ms3-1.2.9/docs/ms3_architecture.drawio`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/ms3_architecture.png` & `ms3-1.2.9/docs/ms3_architecture.png`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/o_quam.mscx` & `ms3-1.2.9/docs/o_quam.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/old_src/quick_old.md` & `ms3-1.2.9/docs/old_src/quick_old.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/old_src/quick_old.rst` & `ms3-1.2.9/docs/old_src/quick_old.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/quae.mscx` & `ms3-1.2.9/docs/quae.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/quick.md` & `ms3-1.2.9/docs/quick.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/reference.rst` & `ms3-1.2.9/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/docs/stabat.mscx` & `ms3-1.2.9/docs/stabat.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/conftest.py` & `ms3-1.2.9/new_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv` & `ms3-1.2.9/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv` & `ms3-1.2.9/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv` & `ms3-1.2.9/new_tests/inferred_labels/sweelinck_keyboard/SwWV258_fantasia_cromatica_results_midi.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/test_cli.py` & `ms3-1.2.9/new_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/test_extract.py` & `ms3-1.2.9/new_tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/test_parse.py` & `ms3-1.2.9/new_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/test_score.py` & `ms3-1.2.9/new_tests/test_score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/new_tests/test_transformations.py` & `ms3-1.2.9/new_tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/05_symph_fant_events.tsv` & `ms3-1.2.9/old_tests/05_symph_fant_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/05_symph_fant_measures.tsv` & `ms3-1.2.9/old_tests/05_symph_fant_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/05_symph_fant_notes.tsv` & `ms3-1.2.9/old_tests/05_symph_fant_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/76CASM34A33UM_events.tsv` & `ms3-1.2.9/old_tests/76CASM34A33UM_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/76CASM34A33UM_labels.tsv` & `ms3-1.2.9/old_tests/76CASM34A33UM_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/76CASM34A33UM_measures.tsv` & `ms3-1.2.9/old_tests/76CASM34A33UM_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/76CASM34A33UM_notes.tsv` & `ms3-1.2.9/old_tests/76CASM34A33UM_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/ALL_WARNINGS` & `ms3-1.2.9/old_tests/ALL_WARNINGS`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/BWV_0815_events.tsv` & `ms3-1.2.9/old_tests/BWV_0815_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/BWV_0815_measures.tsv` & `ms3-1.2.9/old_tests/BWV_0815_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/BWV_0815_notes.tsv` & `ms3-1.2.9/old_tests/BWV_0815_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/D973deutscher01_events.tsv` & `ms3-1.2.9/old_tests/D973deutscher01_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/D973deutscher01_measures.tsv` & `ms3-1.2.9/old_tests/D973deutscher01_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/D973deutscher01_notes.tsv` & `ms3-1.2.9/old_tests/D973deutscher01_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv` & `ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv` & `ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv` & `ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv` & `ms3-1.2.9/old_tests/Did03M-Son_regina-1762-Sarti_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/K281-3_events.tsv` & `ms3-1.2.9/old_tests/K281-3_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/K281-3_labels.tsv` & `ms3-1.2.9/old_tests/K281-3_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/K281-3_measures.tsv` & `ms3-1.2.9/old_tests/K281-3_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/K281-3_notes.tsv` & `ms3-1.2.9/old_tests/K281-3_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/MS3/05_symph_fant.mscx` & `ms3-1.2.9/old_tests/MS3/05_symph_fant.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/MS3/76CASM34A33UM.mscx` & `ms3-1.2.9/old_tests/MS3/76CASM34A33UM.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/MS3/BWV_0815.mscx` & `ms3-1.2.9/old_tests/MS3/BWV_0815.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/MS3/D973deutscher01.mscx` & `ms3-1.2.9/old_tests/MS3/D973deutscher01.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx` & `ms3-1.2.9/old_tests/MS3/Did03M-Son_regina-1762-Sarti.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/MS3/K281-3.mscx` & `ms3-1.2.9/old_tests/MS3/K281-3.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/MS3/stabat_03_coloured.mscx` & `ms3-1.2.9/old_tests/MS3/stabat_03_coloured.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/README.md` & `ms3-1.2.9/old_tests/README.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/harmonies/76CASM34A33UM.tsv` & `ms3-1.2.9/old_tests/harmonies/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.9/old_tests/harmonies/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/harmonies/K281-3.tsv` & `ms3-1.2.9/old_tests/harmonies/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/harmonies/stabat_03_coloured.tsv` & `ms3-1.2.9/old_tests/harmonies/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/measures/05_symph_fant.tsv` & `ms3-1.2.9/old_tests/measures/05_symph_fant.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/measures/76CASM34A33UM.tsv` & `ms3-1.2.9/old_tests/measures/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/measures/BWV_0815.tsv` & `ms3-1.2.9/old_tests/measures/BWV_0815.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/measures/D973deutscher01.tsv` & `ms3-1.2.9/old_tests/measures/D973deutscher01.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.9/old_tests/measures/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/measures/K281-3.tsv` & `ms3-1.2.9/old_tests/measures/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/measures/stabat_03_coloured.tsv` & `ms3-1.2.9/old_tests/measures/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/metadata.tsv` & `ms3-1.2.9/old_tests/metadata.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/notes/05_symph_fant.tsv` & `ms3-1.2.9/old_tests/notes/05_symph_fant.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/notes/76CASM34A33UM.tsv` & `ms3-1.2.9/old_tests/notes/76CASM34A33UM.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/notes/BWV_0815.tsv` & `ms3-1.2.9/old_tests/notes/BWV_0815.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/notes/D973deutscher01.tsv` & `ms3-1.2.9/old_tests/notes/D973deutscher01.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv` & `ms3-1.2.9/old_tests/notes/Did03M-Son_regina-1762-Sarti.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/notes/K281-3.tsv` & `ms3-1.2.9/old_tests/notes/K281-3.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/notes/stabat_03_coloured.tsv` & `ms3-1.2.9/old_tests/notes/stabat_03_coloured.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/paths1.json` & `ms3-1.2.9/old_tests/paths1.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/paths2.json` & `ms3-1.2.9/old_tests/paths2.json`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/repeat_dummies/repeats0.mscx` & `ms3-1.2.9/old_tests/repeat_dummies/repeats0.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/repeat_dummies/repeats1.mscx` & `ms3-1.2.9/old_tests/repeat_dummies/repeats1.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/repeat_dummies/repeats2.mscx` & `ms3-1.2.9/old_tests/repeat_dummies/repeats2.mscx`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/stabat_03_coloured_events.tsv` & `ms3-1.2.9/old_tests/stabat_03_coloured_events.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/stabat_03_coloured_labels.tsv` & `ms3-1.2.9/old_tests/stabat_03_coloured_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/stabat_03_coloured_measures.tsv` & `ms3-1.2.9/old_tests/stabat_03_coloured_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/stabat_03_coloured_notes.tsv` & `ms3-1.2.9/old_tests/stabat_03_coloured_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_parse.py` & `ms3-1.2.9/old_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_repeats.py` & `ms3-1.2.9/old_tests/test_repeats.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/05_symph_fant_measures.tsv` & `ms3-1.2.9/old_tests/test_results/05_symph_fant_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/05_symph_fant_notes.tsv` & `ms3-1.2.9/old_tests/test_results/05_symph_fant_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/76CASM34A33UM_labels.tsv` & `ms3-1.2.9/old_tests/test_results/76CASM34A33UM_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/76CASM34A33UM_measures.tsv` & `ms3-1.2.9/old_tests/test_results/76CASM34A33UM_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/76CASM34A33UM_notes.tsv` & `ms3-1.2.9/old_tests/test_results/76CASM34A33UM_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/BWV_0815_measures.tsv` & `ms3-1.2.9/old_tests/test_results/BWV_0815_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/BWV_0815_notes.tsv` & `ms3-1.2.9/old_tests/test_results/BWV_0815_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/D973deutscher01_measures.tsv` & `ms3-1.2.9/old_tests/test_results/D973deutscher01_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/D973deutscher01_notes.tsv` & `ms3-1.2.9/old_tests/test_results/D973deutscher01_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv` & `ms3-1.2.9/old_tests/test_results/Did03M-Son_regina-1762-Sarti_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv` & `ms3-1.2.9/old_tests/test_results/Did03M-Son_regina-1762-Sarti_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv` & `ms3-1.2.9/old_tests/test_results/Did03M-Son_regina-1762-Sarti_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/K281-3_labels.tsv` & `ms3-1.2.9/old_tests/test_results/K281-3_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/K281-3_measures.tsv` & `ms3-1.2.9/old_tests/test_results/K281-3_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/K281-3_notes.tsv` & `ms3-1.2.9/old_tests/test_results/K281-3_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/stabat_03_coloured_labels.tsv` & `ms3-1.2.9/old_tests/test_results/stabat_03_coloured_labels.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/stabat_03_coloured_measures.tsv` & `ms3-1.2.9/old_tests/test_results/stabat_03_coloured_measures.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_results/stabat_03_coloured_notes.tsv` & `ms3-1.2.9/old_tests/test_results/stabat_03_coloured_notes.tsv`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/old_tests/test_score.py` & `ms3-1.2.9/old_tests/test_score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/paper/paper.bib` & `ms3-1.2.9/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/paper/paper.md` & `ms3-1.2.9/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/paper/paper.pdf` & `ms3-1.2.9/paper/paper.pdf`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/setup.cfg` & `ms3-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/setup.py` & `ms3-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/__init__.py` & `ms3-1.2.9/src/ms3/__init__.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/_typing.py` & `ms3-1.2.9/src/ms3/_typing.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/annotations.py` & `ms3-1.2.9/src/ms3/annotations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/bs4_measures.py` & `ms3-1.2.9/src/ms3/bs4_measures.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/bs4_parser.py` & `ms3-1.2.9/src/ms3/bs4_parser.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/cli.py` & `ms3-1.2.9/src/ms3/cli.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/corpus.py` & `ms3-1.2.9/src/ms3/corpus.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/expand_dcml.py` & `ms3-1.2.9/src/ms3/expand_dcml.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/ferocious_names.txt` & `ms3-1.2.9/src/ms3/ferocious_names.txt`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/logger.py` & `ms3-1.2.9/src/ms3/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging, sys, os
 from contextlib import contextmanager
 from functools import wraps
 from enum import Enum, unique
 from inspect import stack
-from typing import Iterable, Tuple, List
+from typing import Iterable, Tuple, List, Set
 
 LEVELS = {
     'DEBUG': logging.DEBUG,
     'INFO': logging.INFO,
     'WARNING': logging.WARNING,
     'ERROR': logging.ERROR,
     'CRITICAL': logging.CRITICAL,
@@ -447,8 +447,15 @@
             components.remove(remove)
         except ValueError:
             pass
     for extension in ('tsv', 'mscx', 'mscz', 'cap', 'capx', 'midi', 'mid', 'musicxml', 'mxl', 'xml'):
         if components[-1] == extension:
             components = components[:-1]
             break
-    return '.'.join(components)
+    return '.'.join(components)
+
+def get_ignored_warning_ids(logger: logging.Logger) -> Set[tuple]:
+    try:
+        existing_filter = next(filter for filter in logger.filters if isinstance(filter, WarningFilter))
+        return set(existing_filter.ignored_warnings)
+    except StopIteration:
+        return set()
```

### Comparing `ms3-1.2.8/src/ms3/operations.py` & `ms3-1.2.9/src/ms3/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from typing import Literal, Optional, Tuple, Dict, List, Union
 
 from ms3 import Parse, Corpus
 from ms3._typing import AnnotationsFacet
 from ms3.utils import capture_parse_logs, LATEST_MUSESCORE_VERSION, pretty_dict, check_argument_against_literal_type, compute_path_from_file, write_tsv, fifths2sd, scale_degree2name
-from ms3.logger import get_logger, temporarily_suppress_warnings, function_logger
+from ms3.logger import get_logger, temporarily_suppress_warnings, function_logger, get_ignored_warning_ids
+
 
 def insert_labels_into_score(ms3_object: Union[Parse, Corpus],
                              facet: AnnotationsFacet,
                              ask_for_input: bool = True,
                              replace: bool = True,
                              staff: int = None,
                              voice: Optional[Literal[1, 2, 3, 4]] = None,
@@ -258,32 +259,33 @@
     Returns:
         False if at least one label went beyond the threshold, True otherwise.
     """
     review_reports = parse_obj.color_non_chord_tones()
     test_passes = True
     for (corpus_name, fname), file_df_pairs in review_reports.items():
         piece_logger = get_logger(parse_obj[corpus_name].logger_names[fname])
+        ignored_warning_ids = get_ignored_warning_ids(piece_logger)
         is_first = True
         for file, report in file_df_pairs:
             report_path = compute_path_from_file(file, root_dir=out_dir, folder='reviewed')
             os.makedirs(report_path, exist_ok=True)
             report_file = os.path.join(report_path, file.fname + '_reviewed.tsv')
             if not is_first and os.path.isfile(report_file):
                 get_logger('ms3.review').warning(f"This coloring report has been overwritten because several scores have the same fname:\n{report_file}")
             write_tsv(report, report_file)
             is_first = False
             warning_selection = (report.count_ratio > threshold) & report.chord_tones.notna()
-            if warning_selection.sum() > 0:
-                test_passes = False
-            else:
-                continue
             for t in report[warning_selection].itertuples():
+                message_id = (19, t.mc, str(t.mc_onset), t.label)
+                if message_id in ignored_warning_ids:
+                    continue
+                test_passes = False
                 if len(t.added_tones) > 0:
                     added = f" plus the added {(fifths2sd(t.added_tones, t.localkey_is_minor))} [{scale_degree2name(t.added_tones, t.localkey, t.globalkey)}]"
                 else:
                     added = ""
                 msg = f"""The label '{t.label}' in m. {t.mn}, onset {t.mn_onset} (MC {t.mc}, onset {t.mc_onset}) seems not to correspond well to the score (which does not necessarily mean it is wrong).
 In the context of {t.globalkey}.{t.localkey}, it expresses the scale degrees {(fifths2sd(t.chord_tones, t.localkey_is_minor))} [{scale_degree2name(t.chord_tones, t.localkey, t.globalkey)}]{added}.
 The corresponding score segment has {t.n_untouched} within-label and {t.n_colored} out-of-label note onsets, a ratio of {t.count_ratio} > {threshold} (the current, arbitrary, threshold).
 If it turns out the label is correct, please add the header of this warning to the IGNORED_WARNINGS, ideally followed by a free-text comment in subsequent lines starting with a space or tab."""
-                piece_logger.warning(msg, extra={'message_id': (19, t.mc, str(t.mc_onset), t.label)})
+                piece_logger.warning(msg, extra={'message_id': message_id})
     return test_passes
```

### Comparing `ms3-1.2.8/src/ms3/parse.py` & `ms3-1.2.9/src/ms3/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
                             **corpus_config)
             return
 
         # new corpus/corpora to be added
         subdir_corpora = sorted(get_first_level_corpora(directory, logger=self.logger))
         n_corpora = len(subdir_corpora)
         if n_corpora == 0:
-            self.logger.debug(f"Treating {directory} as corpus.")
+            self.logger.debug(f"Treating {directory} as corpus because none of its children seems to be a corpus.")
             self.add_corpus(directory,
                             **corpus_config)
         else:
             self.logger.debug(f"{n_corpora} individual corpora detected in {directory}.")
             for corpus_path in subdir_corpora:
                 self.add_corpus(corpus_path,
                                 **corpus_config)
```

### Comparing `ms3-1.2.8/src/ms3/piece.py` & `ms3-1.2.9/src/ms3/piece.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/score.py` & `ms3-1.2.9/src/ms3/score.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/transformations.py` & `ms3-1.2.9/src/ms3/transformations.py`

 * *Files identical despite different names*

### Comparing `ms3-1.2.8/src/ms3/utils.py` & `ms3-1.2.9/src/ms3/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 00000420: 7064 6174 655f 6366 672c 204c 6f67 4361  pdate_cfg, LogCa
 00000430: 7074 7572 6572 0a66 726f 6d20 2e5f 7479  pturer.from ._ty
 00000440: 7069 6e67 2069 6d70 6f72 7420 4669 6c65  ping import File
 00000450: 4469 6374 2c20 4661 6365 742c 2056 6965  Dict, Facet, Vie
 00000460: 7744 6963 742c 2046 696c 6544 6174 6166  wDict, FileDataf
 00000470: 7261 6d65 5475 706c 654d 6179 6265 0a0a  rameTupleMaybe..
 00000480: 4d53 335f 5645 5253 494f 4e20 3d20 2731  MS3_VERSION = '1
-00000490: 2e32 2e38 270a 4c41 5445 5354 5f4d 5553  .2.8'.LATEST_MUS
+00000490: 2e32 2e39 270a 4c41 5445 5354 5f4d 5553  .2.9'.LATEST_MUS
 000004a0: 4553 434f 5245 5f56 4552 5349 4f4e 203d  ESCORE_VERSION =
 000004b0: 2027 332e 362e 3227 0a43 4f4d 5055 5445   '3.6.2'.COMPUTE
 000004c0: 445f 4d45 5441 4441 5441 5f43 4f4c 554d  D_METADATA_COLUM
 000004d0: 4e53 203d 205b 2754 696d 6553 6967 272c  NS = ['TimeSig',
 000004e0: 2027 4b65 7953 6967 272c 2027 6c61 7374   'KeySig', 'last
 000004f0: 5f6d 6327 2c20 276c 6173 745f 6d6e 272c  _mc', 'last_mn',
 00000500: 2027 6c65 6e67 7468 5f71 6227 2c20 276c   'length_qb', 'l
@@ -9302,4429 +9302,4435 @@
 00024550: 6472 6f70 3d64 726f 705f 696e 6465 7829  drop=drop_index)
 00024560: 5b6c 6973 7428 7265 6e61 6d65 346d 6172  [list(rename4mar
 00024570: 6b64 6f77 6e2e 6b65 7973 2829 295d 2e66  kdown.keys())].f
 00024580: 696c 6c6e 6128 2727 290a 2020 2020 6d64  illna('').    md
 00024590: 203d 206d 642e 7265 6e61 6d65 2863 6f6c   = md.rename(col
 000245a0: 756d 6e73 3d72 656e 616d 6534 6d61 726b  umns=rename4mark
 000245b0: 646f 776e 290a 2020 2020 6d64 5f74 6162  down).    md_tab
-000245c0: 6c65 203d 2073 7472 2864 6632 6d64 286d  le = str(df2md(m
-000245d0: 6429 290a 2020 2020 6d64 5f74 6162 6c65  d)).    md_table
-000245e0: 202b 3d20 6622 5c6e 5c6e 2a4f 7665 7276   += f"\n\n*Overv
-000245f0: 6965 7720 7461 626c 6520 7570 6461 7465  iew table update
-00024600: 6420 7573 696e 6720 5b6d 7333 5d28 6874  d using [ms3](ht
-00024610: 7470 733a 2f2f 6a6f 6865 6e74 7363 682e  tps://johentsch.
-00024620: 6769 7468 7562 2e69 6f2f 6d73 332f 2920  github.io/ms3/) 
-00024630: 7b4d 5333 5f56 4552 5349 4f4e 7d2e 2a5c  {MS3_VERSION}.*\
-00024640: 6e22 0a0a 2020 2020 6966 206f 732e 7061  n"..    if os.pa
-00024650: 7468 2e69 7366 696c 6528 6669 6c65 5f70  th.isfile(file_p
-00024660: 6174 6829 3a0a 2020 2020 2020 2020 6d73  ath):.        ms
-00024670: 6720 3d20 2755 7064 6174 6564 270a 2020  g = 'Updated'.  
-00024680: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00024690: 6669 6c65 5f70 6174 682c 2027 7227 2c20  file_path, 'r', 
-000246a0: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
-000246b0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-000246c0: 2020 2020 6c69 6e65 7320 3d20 662e 7265      lines = f.re
-000246d0: 6164 6c69 6e65 7328 290a 2020 2020 656c  adlines().    el
-000246e0: 7365 3a0a 2020 2020 2020 2020 6d73 6720  se:.        msg 
-000246f0: 3d20 2743 7265 6174 6564 270a 2020 2020  = 'Created'.    
-00024700: 2020 2020 6c69 6e65 7320 3d20 5b5d 0a20      lines = []. 
-00024710: 2020 2023 2069 6e20 6361 7365 2074 6865     # in case the
-00024720: 2052 4541 444d 452e 6d64 2065 7869 7374   README.md exist
-00024730: 732c 2065 7665 7279 7468 696e 6720 6672  s, everything fr
-00024740: 6f6d 2074 6865 206c 696e 6520 696e 636c  om the line incl
-00024750: 7564 696e 6720 2723 204f 7665 7276 6965  uding '# Overvie
-00024760: 7727 2028 6f72 206c 6173 7420 6c69 6e65  w' (or last line
-00024770: 206f 7468 6572 7769 7365 2920 6973 206f   otherwise) is o
-00024780: 7665 7277 7269 7474 656e 0a20 2020 2077  verwritten.    w
-00024790: 6974 6820 6f70 656e 2866 696c 655f 7061  ith open(file_pa
-000247a0: 7468 2c20 2777 272c 2065 6e63 6f64 696e  th, 'w', encodin
-000247b0: 673d 2775 7466 2d38 2729 2061 7320 663a  g='utf-8') as f:
-000247c0: 0a20 2020 2020 2020 2066 6f72 206c 696e  .        for lin
-000247d0: 6520 696e 206c 696e 6573 3a0a 2020 2020  e in lines:.    
-000247e0: 2020 2020 2020 2020 6966 2027 2320 4f76          if '# Ov
-000247f0: 6572 7669 6577 2720 696e 206c 696e 653a  erview' in line:
-00024800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024810: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-00024820: 2020 2066 2e77 7269 7465 286c 696e 6529     f.write(line)
-00024830: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00024840: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
-00024850: 7465 2827 5c6e 5c6e 2729 0a20 2020 2020  te('\n\n').     
-00024860: 2020 2066 2e77 7269 7465 286d 645f 7461     f.write(md_ta
-00024870: 626c 6529 0a20 2020 206c 6f67 6765 722e  ble).    logger.
-00024880: 696e 666f 2866 227b 6d73 677d 207b 6669  info(f"{msg} {fi
-00024890: 6c65 5f70 6174 687d 2229 0a0a 0a64 6566  le_path}")...def
-000248a0: 2070 7265 7061 7265 5f6d 6574 6164 6174   prepare_metadat
-000248b0: 615f 666f 725f 7772 6974 696e 6728 6d65  a_for_writing(me
-000248c0: 7461 6461 7461 5f64 6629 3a0a 2020 2020  tadata_df):.    
-000248d0: 2320 636f 6e76 6572 745f 746f 5f73 7472  # convert_to_str
-000248e0: 203d 207b 633a 2027 7374 7269 6e67 2720   = {c: 'string' 
-000248f0: 666f 7220 6320 696e 2028 276c 656e 6774  for c in ('lengt
-00024900: 685f 7162 272c 2027 6c65 6e67 7468 5f71  h_qb', 'length_q
-00024910: 625f 756e 666f 6c64 6564 272c 2027 616c  b_unfolded', 'al
-00024920: 6c5f 6e6f 7465 735f 7162 2729 2069 6620  l_notes_qb') if 
-00024930: 6320 696e 206d 6574 6164 6174 615f 6466  c in metadata_df
-00024940: 7d0a 2020 2020 2320 6966 206c 656e 2863  }.    # if len(c
-00024950: 6f6e 7665 7274 5f74 6f5f 7374 7229 203e  onvert_to_str) >
-00024960: 2030 3a0a 2020 2020 2320 2020 2020 6d65   0:.    #     me
-00024970: 7461 6461 7461 5f64 6620 3d20 6d65 7461  tadata_df = meta
-00024980: 6461 7461 5f64 662e 6173 7479 7065 2863  data_df.astype(c
-00024990: 6f6e 7665 7274 5f74 6f5f 7374 722c 2065  onvert_to_str, e
-000249a0: 7272 6f72 733d 2769 676e 6f72 6527 290a  rrors='ignore').
-000249b0: 2020 2020 6d65 7461 6461 7461 5f64 6620      metadata_df 
-000249c0: 3d20 6d65 7461 6461 7461 5f64 662e 6173  = metadata_df.as
-000249d0: 7479 7065 2827 7374 7269 6e67 272c 2065  type('string', e
-000249e0: 7272 6f72 733d 2769 676e 6f72 6527 290a  rrors='ignore').
-000249f0: 2020 2020 6d65 7461 6461 7461 5f64 662e      metadata_df.
-00024a00: 736f 7274 5f69 6e64 6578 2869 6e70 6c61  sort_index(inpla
-00024a10: 6365 3d54 7275 6529 0a20 2020 206d 6574  ce=True).    met
-00024a20: 6164 6174 615f 6466 203d 2063 6f6c 756d  adata_df = colum
-00024a30: 6e5f 6f72 6465 7228 6d65 7461 6461 7461  n_order(metadata
-00024a40: 5f64 662c 204d 4554 4144 4154 415f 434f  _df, METADATA_CO
-00024a50: 4c55 4d4e 5f4f 5244 4552 2c20 736f 7274  LUMN_ORDER, sort
-00024a60: 3d46 616c 7365 290a 2020 2020 2320 6f6e  =False).    # on
-00024a70: 2057 696e 646f 7773 2c20 6d61 6b65 2073   Windows, make s
-00024a80: 7572 6520 7468 6520 7061 7468 7320 6172  ure the paths ar
-00024a90: 6520 7772 6974 7465 6e20 7769 7468 202f  e written with /
-00024aa0: 2073 6570 6172 6174 6f72 730a 2020 2020   separators.    
-00024ab0: 7061 7468 5f63 6f6c 7320 3d20 5b63 6f6c  path_cols = [col
-00024ac0: 2066 6f72 2063 6f6c 2069 6e20 2827 7375   for col in ('su
-00024ad0: 6264 6972 272c 2027 7265 6c5f 7061 7468  bdir', 'rel_path
-00024ae0: 2729 2069 6620 636f 6c20 696e 206d 6574  ') if col in met
-00024af0: 6164 6174 615f 6466 2e63 6f6c 756d 6e73  adata_df.columns
-00024b00: 5d0a 2020 2020 666f 7220 636f 6c20 696e  ].    for col in
-00024b10: 2070 6174 685f 636f 6c73 3a0a 2020 2020   path_cols:.    
-00024b20: 2020 2020 7769 7468 2077 6172 6e69 6e67      with warning
-00024b30: 732e 6361 7463 685f 7761 726e 696e 6773  s.catch_warnings
-00024b40: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00024b50: 2320 5365 7474 696e 6720 7661 6c75 6573  # Setting values
-00024b60: 2069 6e2d 706c 6163 6520 6973 2066 696e   in-place is fin
-00024b70: 652c 2069 676e 6f72 6520 7468 6520 7761  e, ignore the wa
-00024b80: 726e 696e 6720 696e 2050 616e 6461 7320  rning in Pandas 
-00024b90: 3e3d 2031 2e35 2e30 0a20 2020 2020 2020  >= 1.5.0.       
-00024ba0: 2020 2020 2023 2054 6869 7320 6361 6e20       # This can 
-00024bb0: 6265 2072 656d 6f76 6564 2c20 6966 2050  be removed, if P
-00024bc0: 616e 6461 7320 312e 352e 3020 646f 6573  andas 1.5.0 does
-00024bd0: 206e 6f74 206e 6565 6420 746f 2062 6520   not need to be 
-00024be0: 7375 7070 6f72 7465 6420 616e 7920 6c6f  supported any lo
-00024bf0: 6e67 6572 2e0a 2020 2020 2020 2020 2020  nger..          
-00024c00: 2020 2320 5365 6520 616c 736f 3a20 6874    # See also: ht
-00024c10: 7470 733a 2f2f 7374 6163 6b6f 7665 7266  tps://stackoverf
-00024c20: 6c6f 772e 636f 6d2f 712f 3734 3035 3733  low.com/q/740573
-00024c30: 3637 2f38 3539 3539 310a 2020 2020 2020  67/859591.      
-00024c40: 2020 2020 2020 7761 726e 696e 6773 2e66        warnings.f
-00024c50: 696c 7465 7277 6172 6e69 6e67 7328 0a20  ilterwarnings(. 
-00024c60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00024c70: 6967 6e6f 7265 222c 0a20 2020 2020 2020  ignore",.       
-00024c80: 2020 2020 2020 2020 2063 6174 6567 6f72           categor
-00024c90: 793d 4675 7475 7265 5761 726e 696e 672c  y=FutureWarning,
-00024ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024cb0: 206d 6573 7361 6765 3d28 0a20 2020 2020   message=(.     
-00024cc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00024cd0: 2e2a 7769 6c6c 2061 7474 656d 7074 2074  .*will attempt t
-00024ce0: 6f20 7365 7420 7468 6520 7661 6c75 6573  o set the values
-00024cf0: 2069 6e70 6c61 6365 2069 6e73 7465 6164   inplace instead
-00024d00: 206f 6620 616c 7761 7973 2073 6574 7469   of always setti
-00024d10: 6e67 2061 206e 6577 2061 7272 6179 2e20  ng a new array. 
-00024d20: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00024d30: 2020 2020 2020 2254 6f20 7265 7461 696e        "To retain
-00024d40: 2074 6865 206f 6c64 2062 6568 6176 696f   the old behavio
-00024d50: 722c 2075 7365 2065 6974 6865 722e 2a22  r, use either.*"
-00024d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024d70: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00024d80: 290a 2020 2020 2020 2020 2020 2020 6d65  ).            me
-00024d90: 7461 6461 7461 5f64 662e 6c6f 635b 3a2c  tadata_df.loc[:,
-00024da0: 2063 6f6c 5d20 3d20 6d65 7461 6461 7461   col] = metadata
-00024db0: 5f64 665b 636f 6c5d 2e73 7472 2e72 6570  _df[col].str.rep
-00024dc0: 6c61 6365 286f 732e 7365 702c 2027 2f27  lace(os.sep, '/'
-00024dd0: 290a 2020 2020 7374 6166 665f 636f 6c73  ).    staff_cols
-00024de0: 2c20 6f74 6865 725f 636f 6c73 203d 205b  , other_cols = [
-00024df0: 5d2c 205b 5d0a 2020 2020 666f 7220 636f  ], [].    for co
-00024e00: 6c20 696e 206d 6574 6164 6174 615f 6466  l in metadata_df
-00024e10: 2e63 6f6c 756d 6e73 3a0a 2020 2020 2020  .columns:.      
-00024e20: 2020 6966 2072 652e 6d61 7463 6828 7222    if re.match(r"
-00024e30: 5e73 7461 6666 5f28 5c64 2b29 222c 2063  ^staff_(\d+)", c
-00024e40: 6f6c 293a 0a20 2020 2020 2020 2020 2020  ol):.           
-00024e50: 2073 7461 6666 5f63 6f6c 732e 6170 7065   staff_cols.appe
-00024e60: 6e64 2863 6f6c 290a 2020 2020 2020 2020  nd(col).        
-00024e70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00024e80: 2020 6f74 6865 725f 636f 6c73 2e61 7070    other_cols.app
-00024e90: 656e 6428 636f 6c29 0a20 2020 2073 7461  end(col).    sta
-00024ea0: 6666 5f63 6f6c 7320 3d20 736f 7274 6564  ff_cols = sorted
-00024eb0: 2873 7461 6666 5f63 6f6c 732c 206b 6579  (staff_cols, key
-00024ec0: 3d6c 616d 6264 6120 733a 2069 6e74 2872  =lambda s: int(r
-00024ed0: 652e 6d61 7463 6828 7222 5e73 7461 6666  e.match(r"^staff
-00024ee0: 5f28 5c64 2b29 222c 2073 295b 315d 2929  _(\d+)", s)[1]))
-00024ef0: 0a20 2020 206d 6574 6164 6174 615f 6466  .    metadata_df
-00024f00: 203d 206d 6574 6164 6174 615f 6466 5b6f   = metadata_df[o
-00024f10: 7468 6572 5f63 6f6c 7320 2b20 7374 6166  ther_cols + staf
-00024f20: 665f 636f 6c73 5d0a 2020 2020 6966 206e  f_cols].    if n
-00024f30: 6f74 2069 7369 6e73 7461 6e63 6528 6d65  ot isinstance(me
-00024f40: 7461 6461 7461 5f64 662e 696e 6465 782c  tadata_df.index,
-00024f50: 2070 642e 5261 6e67 6549 6e64 6578 293a   pd.RangeIndex):
-00024f60: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-00024f70: 615f 6466 203d 206d 6574 6164 6174 615f  a_df = metadata_
-00024f80: 6466 2e72 6573 6574 5f69 6e64 6578 2829  df.reset_index()
-00024f90: 0a20 2020 2072 6574 7572 6e20 6d65 7461  .    return meta
-00024fa0: 6461 7461 5f64 660a 0a0a 4066 756e 6374  data_df...@funct
-00024fb0: 696f 6e5f 6c6f 6767 6572 0a64 6566 2077  ion_logger.def w
-00024fc0: 7269 7465 5f74 7376 2864 662c 2066 696c  rite_tsv(df, fil
-00024fd0: 655f 7061 7468 2c20 7072 655f 7072 6f63  e_path, pre_proc
-00024fe0: 6573 733d 5472 7565 2c20 2a2a 6b77 6172  ess=True, **kwar
-00024ff0: 6773 293a 0a20 2020 2022 2222 2057 7269  gs):.    """ Wri
-00025000: 7465 2061 2044 6174 6146 7261 6d65 2074  te a DataFrame t
-00025010: 6f20 6120 5453 5620 6f72 2043 5356 2066  o a TSV or CSV f
-00025020: 696c 6520 6261 7365 6420 6f6e 2074 6865  ile based on the
-00025030: 2065 7874 656e 7369 6f6e 206f 6620 2766   extension of 'f
-00025040: 696c 655f 7061 7468 272e 0a20 2020 2055  ile_path'..    U
-00025050: 7365 733a 203a 7079 3a66 756e 633a 606e  ses: :py:func:`n
-00025060: 6f5f 636f 6c6c 6563 7469 6f6e 735f 6e6f  o_collections_no
-00025070: 5f62 6f6f 6c65 616e 7360 0a0a 2020 2020  _booleans`..    
-00025080: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00025090: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6466  ---------.    df
-000250a0: 203a 203a 6f62 6a3a 6070 616e 6461 732e   : :obj:`pandas.
-000250b0: 4461 7461 4672 616d 6560 0a20 2020 2020  DataFrame`.     
-000250c0: 2020 2044 6174 6146 7261 6d65 2074 6f20     DataFrame to 
-000250d0: 7772 6974 652e 0a20 2020 2066 696c 655f  write..    file_
-000250e0: 7061 7468 203a 203a 6f62 6a3a 6073 7472  path : :obj:`str
-000250f0: 600a 2020 2020 2020 2020 4669 6c65 2074  `.        File t
-00025100: 6f20 6372 6561 7465 206f 7220 6f76 6572  o create or over
-00025110: 7772 6974 652e 2049 6620 7468 6520 6578  write. If the ex
-00025120: 7465 6e73 696f 6e20 6973 202e 7473 762c  tension is .tsv,
-00025130: 2074 6865 2061 7267 756d 656e 7420 2773   the argument 's
-00025140: 6570 2720 7769 6c6c 2062 6520 7365 7420  ep' will be set 
-00025150: 746f 2027 5c74 272c 206f 7468 6572 7769  to '\t', otherwi
-00025160: 7365 2074 6865 0a20 2020 2020 2020 2065  se the.        e
-00025170: 7874 656e 7369 6f6e 2069 7320 6578 7065  xtension is expe
-00025180: 6374 6564 2074 6f20 6265 202e 6373 7620  cted to be .csv 
-00025190: 616e 6420 7468 6520 6465 6661 756c 7420  and the default 
-000251a0: 7365 7061 7261 746f 7220 272c 2720 7769  separator ',' wi
-000251b0: 6c6c 2062 6520 7573 6564 2e0a 2020 2020  ll be used..    
-000251c0: 7072 655f 7072 6f63 6573 7320 3a20 3a6f  pre_process : :o
-000251d0: 626a 3a60 626f 6f6c 602c 206f 7074 696f  bj:`bool`, optio
-000251e0: 6e61 6c0a 2020 2020 2020 2020 4279 2064  nal.        By d
-000251f0: 6566 6175 6c74 2c20 4461 7461 4672 616d  efault, DataFram
-00025200: 6520 6365 6c6c 7320 636f 6e74 6169 6e69  e cells containi
-00025210: 6e67 206c 6973 7473 2061 6e64 2074 7570  ng lists and tup
-00025220: 6c65 7320 7769 6c6c 2062 6520 7472 616e  les will be tran
-00025230: 7366 6f72 6d65 6420 746f 2073 7472 696e  sformed to strin
-00025240: 6773 2061 6e64 2042 6f6f 6c65 616e 7320  gs and Booleans 
-00025250: 7769 6c6c 2062 650a 2020 2020 2020 2020  will be.        
-00025260: 636f 6e76 6572 7465 6420 746f 2030 2061  converted to 0 a
-00025270: 6e64 2031 2028 6f74 6865 7277 6973 6520  nd 1 (otherwise 
-00025280: 7468 6579 2077 696c 6c20 6265 2077 7269  they will be wri
-00025290: 7474 656e 206f 7574 2061 7320 5472 7565  tten out as True
-000252a0: 2061 6e64 2046 616c 7365 292e 2050 6173   and False). Pas
-000252b0: 7320 4661 6c73 6520 746f 2070 7265 7665  s False to preve
-000252c0: 6e74 2e0a 2020 2020 6b77 6172 6773 203a  nt..    kwargs :
-000252d0: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
-000252e0: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
-000252f0: 6d65 6e74 7320 7769 6c6c 2062 6520 7061  ments will be pa
-00025300: 7373 6564 206f 6e20 746f 203a 7079 3a6d  ssed on to :py:m
-00025310: 6574 683a 6070 616e 6461 732e 4461 7461  eth:`pandas.Data
-00025320: 4672 616d 652e 746f 5f63 7376 602e 0a20  Frame.to_csv`.. 
-00025330: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-00025340: 6172 6775 6d65 6e74 7320 6172 6520 6060  arguments are ``
-00025350: 696e 6465 783d 4661 6c73 6560 6020 616e  index=False`` an
-00025360: 6420 6060 7365 703d 275c 7427 6060 2028  d ``sep='\t'`` (
-00025370: 6173 7375 6d69 6e67 2065 7874 656e 7369  assuming extensi
-00025380: 6f6e 2027 2e74 7376 272c 2073 6565 2061  on '.tsv', see a
-00025390: 626f 7665 292e 0a0a 2020 2020 5265 7475  bove)...    Retu
-000253a0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-000253b0: 2020 2020 4e6f 6e65 0a20 2020 2022 2222      None.    """
-000253c0: 0a20 2020 2070 6174 682c 2066 696c 6520  .    path, file 
-000253d0: 3d20 6f73 2e70 6174 682e 7370 6c69 7428  = os.path.split(
-000253e0: 6669 6c65 5f70 6174 6829 0a20 2020 2070  file_path).    p
-000253f0: 6174 6820 3d20 7265 736f 6c76 655f 6469  ath = resolve_di
-00025400: 7228 7061 7468 290a 2020 2020 6f73 2e70  r(path).    os.p
-00025410: 6174 682e 6a6f 696e 2870 6174 682c 2066  ath.join(path, f
-00025420: 696c 6529 0a20 2020 2066 6e61 6d65 2c20  ile).    fname, 
-00025430: 6578 7420 3d20 6f73 2e70 6174 682e 7370  ext = os.path.sp
-00025440: 6c69 7465 7874 2866 696c 6529 0a20 2020  litext(file).   
-00025450: 2069 6620 6578 742e 6c6f 7765 7228 2920   if ext.lower() 
-00025460: 6e6f 7420 696e 2028 272e 7473 7627 2c20  not in ('.tsv', 
-00025470: 272e 6373 7627 293a 0a20 2020 2020 2020  '.csv'):.       
-00025480: 206c 6f67 6765 722e 6572 726f 7228 6622   logger.error(f"
-00025490: 5468 6973 2066 756e 6374 696f 6e20 6578  This function ex
-000254a0: 7065 6374 7320 6669 6c65 5f70 6174 6820  pects file_path 
-000254b0: 746f 2069 6e63 6c75 6465 2074 6865 2066  to include the f
-000254c0: 696c 6520 6e61 6d65 2065 6e64 696e 6720  ile name ending 
-000254d0: 6f6e 202e 6373 7620 6f72 202e 7473 762c  on .csv or .tsv,
-000254e0: 206e 6f74 2027 7b65 7874 7d27 2e22 290a   not '{ext}'.").
-000254f0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00025500: 2020 206f 732e 6d61 6b65 6469 7273 2870     os.makedirs(p
-00025510: 6174 682c 2065 7869 7374 5f6f 6b3d 5472  ath, exist_ok=Tr
-00025520: 7565 290a 2020 2020 6966 2065 7874 2e6c  ue).    if ext.l
-00025530: 6f77 6572 2829 203d 3d20 272e 7473 7627  ower() == '.tsv'
-00025540: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
-00025550: 2e75 7064 6174 6528 6469 6374 2873 6570  .update(dict(sep
-00025560: 3d27 5c74 2729 290a 2020 2020 6966 2027  ='\t')).    if '
-00025570: 696e 6465 7827 206e 6f74 2069 6e20 6b77  index' not in kw
-00025580: 6172 6773 3a0a 2020 2020 2020 2020 6b77  args:.        kw
-00025590: 6172 6773 5b27 696e 6465 7827 5d20 3d20  args['index'] = 
-000255a0: 4661 6c73 650a 2020 2020 6966 2070 7265  False.    if pre
-000255b0: 5f70 726f 6365 7373 3a0a 2020 2020 2020  _process:.      
-000255c0: 2020 6466 203d 206e 6f5f 636f 6c6c 6563    df = no_collec
-000255d0: 7469 6f6e 735f 6e6f 5f62 6f6f 6c65 616e  tions_no_boolean
-000255e0: 7328 6466 2c20 6c6f 6767 6572 3d6c 6f67  s(df, logger=log
-000255f0: 6765 7229 0a20 2020 2064 662e 746f 5f63  ger).    df.to_c
-00025600: 7376 2866 696c 655f 7061 7468 2c20 2a2a  sv(file_path, **
-00025610: 6b77 6172 6773 290a 2020 2020 6c6f 6767  kwargs).    logg
-00025620: 6572 2e64 6562 7567 2866 227b 6669 6c65  er.debug(f"{file
-00025630: 5f70 6174 687d 2077 7269 7474 656e 2077  _path} written w
-00025640: 6974 6820 7061 7261 6d65 7465 7273 207b  ith parameters {
-00025650: 6b77 6172 6773 7d2e 2229 0a20 2020 2072  kwargs}.").    r
-00025660: 6574 7572 6e0a 0a0a 4066 756e 6374 696f  eturn...@functio
-00025670: 6e5f 6c6f 6767 6572 0a64 6566 2061 6273  n_logger.def abs
-00025680: 3272 656c 5f6b 6579 2861 6273 6f6c 7574  2rel_key(absolut
-00025690: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
-000256a0: 2020 2020 2020 2020 6c6f 6361 6c6b 6579          localkey
-000256b0: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
-000256c0: 2020 2020 2020 2067 6c6f 6261 6c5f 6d69         global_mi
-000256d0: 6e6f 723a 2062 6f6f 6c20 3d20 4661 6c73  nor: bool = Fals
-000256e0: 6529 202d 3e20 7374 723a 0a20 2020 2022  e) -> str:.    "
-000256f0: 2222 0a20 2020 2045 7870 7265 7373 6573  "".    Expresses
-00025700: 2061 2052 6f6d 616e 206e 756d 6572 616c   a Roman numeral
-00025710: 2061 7320 7363 616c 6520 6465 6772 6565   as scale degree
-00025720: 2072 656c 6174 6976 6520 746f 2061 2067   relative to a g
-00025730: 6976 656e 206c 6f63 616c 6b65 792e 0a20  iven localkey.. 
-00025740: 2020 2054 6865 2072 6573 756c 7420 6368     The result ch
-00025750: 616e 6765 7320 6465 7065 6e64 696e 6720  anges depending 
-00025760: 6f6e 2077 6865 7468 6572 2052 6f6d 616e  on whether Roman
-00025770: 206e 756d 6572 616c 2061 6e64 206c 6f63   numeral and loc
-00025780: 616c 6b65 7920 6172 650a 2020 2020 696e  alkey are.    in
-00025790: 7465 7270 7265 7465 6420 7769 7468 696e  terpreted within
-000257a0: 2061 2067 6c6f 6261 6c20 6d61 6a6f 7220   a global major 
-000257b0: 6f72 206d 696e 6f72 206b 6579 2e0a 0a20  or minor key... 
-000257c0: 2020 2055 7365 733a 203a 7079 3a66 756e     Uses: :py:fun
-000257d0: 633a 6073 706c 6974 5f73 6361 6c65 5f64  c:`split_scale_d
-000257e0: 6567 7265 6560 0a0a 0a20 2020 2041 7267  egree`...    Arg
-000257f0: 733a 0a20 2020 2020 2061 6273 6f6c 7574  s:.      absolut
-00025800: 653a 2041 6273 6f6c 7574 6520 6b65 7920  e: Absolute key 
-00025810: 6578 7072 6573 7365 6420 6173 2052 6f6d  expressed as Rom
-00025820: 616e 2073 6361 6c65 2064 6567 7265 6520  an scale degree 
-00025830: 6f66 2074 6865 206c 6f63 616c 206b 6579  of the local key
-00025840: 2e0a 2020 2020 2020 6c6f 6361 6c6b 6579  ..      localkey
-00025850: 3a20 5468 6520 6c6f 6361 6c20 6b65 7920  : The local key 
-00025860: 696e 2074 6572 6d73 206f 6620 7768 6963  in terms of whic
-00025870: 6820 6060 6162 736f 6c75 7465 6060 2077  h ``absolute`` w
-00025880: 696c 6c20 6265 2065 7870 7265 7373 6564  ill be expressed
-00025890: 2e0a 2020 2020 2020 676c 6f62 616c 5f6d  ..      global_m
-000258a0: 696e 6f72 3a20 4861 7320 746f 2062 6520  inor: Has to be 
-000258b0: 7365 7420 746f 2054 7275 6520 6966 2060  set to True if `
-000258c0: 6162 736f 6c75 7465 6020 616e 6420 606c  absolute` and `l
-000258d0: 6f63 616c 6b65 7960 2061 7265 2073 6361  ocalkey` are sca
-000258e0: 6c65 2064 6567 7265 6573 206f 6620 6120  le degrees of a 
-000258f0: 676c 6f62 616c 206d 696e 6f72 206b 6579  global minor key
-00025900: 2e0a 0a20 2020 2045 7861 6d70 6c65 733a  ...    Examples:
-00025910: 0a20 2020 2020 2049 6e20 6120 6d69 6e6f  .      In a mino
-00025920: 7220 636f 6e74 6578 742c 2074 6865 206b  r context, the k
-00025930: 6579 206f 6620 4949 2077 6f75 6c64 2061  ey of II would a
-00025940: 7070 6561 7220 7769 7468 696e 2074 6865  ppear within the
-00025950: 206b 6579 206f 6620 7669 6920 6173 2023   key of vii as #
-00025960: 4949 492e 0a0a 2020 2020 2020 2020 2020  III...          
-00025970: 3e3e 3e20 6162 7332 7265 6c5f 6b65 7928  >>> abs2rel_key(
-00025980: 2769 7627 2c20 2756 4927 2c20 676c 6f62  'iv', 'VI', glob
-00025990: 616c 5f6d 696e 6f72 3d46 616c 7365 290a  al_minor=False).
-000259a0: 2020 2020 2020 2020 2020 2762 7669 2720            'bvi' 
-000259b0: 2020 2020 2020 2320 4620 6d69 6e6f 7220        # F minor 
-000259c0: 6578 7072 6573 7365 6420 7769 7468 2072  expressed with r
-000259d0: 6573 7065 6374 2074 6f20 4120 6d61 6a6f  espect to A majo
-000259e0: 720a 2020 2020 2020 2020 2020 3e3e 3e20  r.          >>> 
-000259f0: 6162 7332 7265 6c5f 6b65 7928 2769 7627  abs2rel_key('iv'
-00025a00: 2c20 2776 6927 2c20 676c 6f62 616c 5f6d  , 'vi', global_m
-00025a10: 696e 6f72 3d46 616c 7365 290a 2020 2020  inor=False).    
-00025a20: 2020 2020 2020 2776 6927 2020 2020 2020        'vi'      
-00025a30: 2320 4620 6d69 6e6f 7220 6578 7072 6573  # F minor expres
-00025a40: 7365 6420 7769 7468 2072 6573 7065 6374  sed with respect
-00025a50: 2074 6f20 4120 6d69 6e6f 720a 2020 2020   to A minor.    
-00025a60: 2020 2020 2020 3e3e 3e20 6162 7332 7265        >>> abs2re
-00025a70: 6c5f 6b65 7928 2769 7627 2c20 2756 4927  l_key('iv', 'VI'
-00025a80: 2c20 676c 6f62 616c 5f6d 696e 6f72 3d54  , global_minor=T
-00025a90: 7275 6529 0a20 2020 2020 2020 2020 2027  rue).          '
-00025aa0: 7669 2720 2020 2020 2023 2046 206d 696e  vi'      # F min
-00025ab0: 6f72 2065 7870 7265 7373 6564 2077 6974  or expressed wit
-00025ac0: 6820 7265 7370 6563 7420 746f 2041 6220  h respect to Ab 
-00025ad0: 6d61 6a6f 720a 2020 2020 2020 2020 2020  major.          
-00025ae0: 3e3e 3e20 6162 7332 7265 6c5f 6b65 7928  >>> abs2rel_key(
-00025af0: 2769 7627 2c20 2776 6927 2c20 676c 6f62  'iv', 'vi', glob
-00025b00: 616c 5f6d 696e 6f72 3d54 7275 6529 0a20  al_minor=True). 
-00025b10: 2020 2020 2020 2020 2027 2376 6927 2020           '#vi'  
-00025b20: 2020 2020 2023 2046 206d 696e 6f72 2065       # F minor e
-00025b30: 7870 7265 7373 6564 2077 6974 6820 7265  xpressed with re
-00025b40: 7370 6563 7420 746f 2041 6220 6d69 6e6f  spect to Ab mino
-00025b50: 720a 0a20 2020 2020 2020 2020 203e 3e3e  r..          >>>
-00025b60: 2061 6273 3272 656c 5f6b 6579 2827 5649   abs2rel_key('VI
-00025b70: 272c 2027 4956 272c 2067 6c6f 6261 6c5f  ', 'IV', global_
-00025b80: 6d69 6e6f 723d 4661 6c73 6529 0a20 2020  minor=False).   
-00025b90: 2020 2020 2020 2027 4949 4927 2020 2020         'III'    
-00025ba0: 2020 2023 2041 206d 616a 6f72 2065 7870     # A major exp
-00025bb0: 7265 7373 6564 2077 6974 6820 7265 7370  ressed with resp
-00025bc0: 6563 7420 746f 2046 206d 616a 6f72 0a20  ect to F major. 
-00025bd0: 2020 2020 2020 2020 203e 3e3e 2061 6273           >>> abs
-00025be0: 3272 656c 5f6b 6579 2827 5649 272c 2027  2rel_key('VI', '
-00025bf0: 6976 272c 2067 6c6f 6261 6c5f 6d69 6e6f  iv', global_mino
-00025c00: 723d 4661 6c73 6529 0a20 2020 2020 2020  r=False).       
-00025c10: 2020 2027 2349 4949 2720 2020 2020 2020     '#III'       
-00025c20: 2320 4120 6d61 6a6f 7220 6578 7072 6573  # A major expres
-00025c30: 7365 6420 7769 7468 2072 6573 7065 6374  sed with respect
-00025c40: 2074 6f20 4620 6d69 6e6f 720a 2020 2020   to F minor.    
-00025c50: 2020 2020 2020 3e3e 3e20 6162 7332 7265        >>> abs2re
-00025c60: 6c5f 6b65 7928 2756 4927 2c20 2749 5627  l_key('VI', 'IV'
-00025c70: 2c20 676c 6f62 616c 5f6d 696e 6f72 3d54  , global_minor=T
-00025c80: 7275 6529 0a20 2020 2020 2020 2020 2027  rue).          '
-00025c90: 6249 4949 2720 2020 2020 2020 2320 4162  bIII'       # Ab
-00025ca0: 206d 616a 6f72 2065 7870 7265 7373 6564   major expressed
-00025cb0: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
-00025cc0: 2046 206d 616a 6f72 0a20 2020 2020 2020   F major.       
-00025cd0: 2020 203e 3e3e 2061 6273 3272 656c 5f6b     >>> abs2rel_k
-00025ce0: 6579 2827 5649 272c 2027 6976 272c 2067  ey('VI', 'iv', g
-00025cf0: 6c6f 6261 6c5f 6d69 6e6f 723d 4661 6c73  lobal_minor=Fals
-00025d00: 6529 0a20 2020 2020 2020 2020 2027 4949  e).          'II
-00025d10: 4927 2020 2020 2020 2023 2041 6220 6d61  I'       # Ab ma
-00025d20: 6a6f 7220 6578 7072 6573 7365 6420 7769  jor expressed wi
-00025d30: 7468 2072 6573 7065 6374 2074 6f20 4620  th respect to F 
-00025d40: 6d69 6e6f 720a 2020 2020 2222 220a 2020  minor.    """.  
-00025d50: 2020 6966 2070 642e 6973 6e75 6c6c 2861    if pd.isnull(a
-00025d60: 6273 6f6c 7574 6529 206f 7220 7064 2e69  bsolute) or pd.i
-00025d70: 736e 756c 6c28 6c6f 6361 6c6b 6579 293a  snull(localkey):
-00025d80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00025d90: 6162 736f 6c75 7465 0a20 2020 2061 6273  absolute.    abs
-00025da0: 6f6c 7574 6520 3d20 7265 736f 6c76 655f  olute = resolve_
-00025db0: 7265 6c61 7469 7665 5f6b 6579 7328 6162  relative_keys(ab
-00025dc0: 736f 6c75 7465 290a 2020 2020 6c6f 6361  solute).    loca
-00025dd0: 6c6b 6579 203d 2072 6573 6f6c 7665 5f72  lkey = resolve_r
-00025de0: 656c 6174 6976 655f 6b65 7973 286c 6f63  elative_keys(loc
-00025df0: 616c 6b65 7929 0a20 2020 206d 616a 5f72  alkey).    maj_r
-00025e00: 6e20 3d20 5b27 4927 2c20 2749 4927 2c20  n = ['I', 'II', 
-00025e10: 2749 4949 272c 2027 4956 272c 2027 5627  'III', 'IV', 'V'
-00025e20: 2c20 2756 4927 2c20 2756 4949 275d 0a20  , 'VI', 'VII']. 
-00025e30: 2020 206d 696e 5f72 6e20 3d20 5b27 6927     min_rn = ['i'
-00025e40: 2c20 2769 6927 2c20 2769 6969 272c 2027  , 'ii', 'iii', '
-00025e50: 6976 272c 2027 7627 2c20 2776 6927 2c20  iv', 'v', 'vi', 
-00025e60: 2776 6969 275d 0a20 2020 2077 6869 7465  'vii'].    white
-00025e70: 5f6b 6579 5f6d 616a 6f72 5f61 6363 6964  _key_major_accid
-00025e80: 656e 7461 6c73 203d 206e 702e 6172 7261  entals = np.arra
-00025e90: 7928 5b5b 302c 2030 2c20 302c 2030 2c20  y([[0, 0, 0, 0, 
-00025ea0: 302c 2030 2c20 305d 2c0a 2020 2020 2020  0, 0, 0],.      
-00025eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ed0: 2020 2020 2020 5b30 2c20 302c 2031 2c20        [0, 0, 1, 
-00025ee0: 302c 2030 2c20 302c 2031 5d2c 0a20 2020  0, 0, 0, 1],.   
-00025ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000245c0: 6c65 203d 2022 2322 202b 2073 7472 2864  le = "#" + str(d
+000245d0: 6632 6d64 286d 6429 2920 2320 636f 6d65  f2md(md)) # come
+000245e0: 7320 7769 7468 2061 2066 6972 7374 2d6c  s with a first-l
+000245f0: 6576 656c 2068 6561 6469 6e67 2077 6869  evel heading whi
+00024600: 6368 2077 6520 7475 726e 2069 6e74 6f20  ch we turn into 
+00024610: 7365 636f 6e64 2d6c 6576 656c 0a20 2020  second-level.   
+00024620: 206d 645f 7461 626c 6520 2b3d 2066 225c   md_table += f"\
+00024630: 6e5c 6e2a 4f76 6572 7669 6577 2074 6162  n\n*Overview tab
+00024640: 6c65 2061 7574 6f6d 6174 6963 616c 6c79  le automatically
+00024650: 2075 7064 6174 6564 2075 7369 6e67 205b   updated using [
+00024660: 6d73 335d 2868 7474 7073 3a2f 2f6a 6f68  ms3](https://joh
+00024670: 656e 7473 6368 2e67 6974 6875 622e 696f  entsch.github.io
+00024680: 2f6d 7333 2f29 2e2a 5c6e 220a 0a20 2020  /ms3/).*\n"..   
+00024690: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+000246a0: 6c65 2866 696c 655f 7061 7468 293a 0a20  le(file_path):. 
+000246b0: 2020 2020 2020 206d 7367 203d 2027 5570         msg = 'Up
+000246c0: 6461 7465 6427 0a20 2020 2020 2020 2077  dated'.        w
+000246d0: 6974 6820 6f70 656e 2866 696c 655f 7061  ith open(file_pa
+000246e0: 7468 2c20 2772 272c 2065 6e63 6f64 696e  th, 'r', encodin
+000246f0: 673d 2775 7466 2d38 2729 2061 7320 663a  g='utf-8') as f:
+00024700: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
+00024710: 6573 203d 2066 2e72 6561 646c 696e 6573  es = f.readlines
+00024720: 2829 0a20 2020 2065 6c73 653a 0a20 2020  ().    else:.   
+00024730: 2020 2020 206d 7367 203d 2027 4372 6561       msg = 'Crea
+00024740: 7465 6427 0a20 2020 2020 2020 206c 696e  ted'.        lin
+00024750: 6573 203d 205b 5d0a 2020 2020 2320 696e  es = [].    # in
+00024760: 2063 6173 6520 7468 6520 5245 4144 4d45   case the README
+00024770: 2e6d 6420 6578 6973 7473 2c20 6576 6572  .md exists, ever
+00024780: 7974 6869 6e67 2066 726f 6d20 7468 6520  ything from the 
+00024790: 6c69 6e65 2069 6e63 6c75 6469 6e67 2027  line including '
+000247a0: 2320 4f76 6572 7669 6577 2720 286f 7220  # Overview' (or 
+000247b0: 6c61 7374 206c 696e 6520 6f74 6865 7277  last line otherw
+000247c0: 6973 6529 2069 7320 6f76 6572 7772 6974  ise) is overwrit
+000247d0: 7465 6e0a 2020 2020 7769 7468 206f 7065  ten.    with ope
+000247e0: 6e28 6669 6c65 5f70 6174 682c 2027 7727  n(file_path, 'w'
+000247f0: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
+00024800: 3827 2920 6173 2066 3a0a 2020 2020 2020  8') as f:.      
+00024810: 2020 666f 7220 6c69 6e65 2069 6e20 6c69    for line in li
+00024820: 6e65 733a 0a20 2020 2020 2020 2020 2020  nes:.           
+00024830: 2069 6620 2723 204f 7665 7276 6965 7727   if '# Overview'
+00024840: 2069 6e20 6c69 6e65 3a0a 2020 2020 2020   in line:.      
+00024850: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00024860: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00024870: 6974 6528 6c69 6e65 290a 2020 2020 2020  ite(line).      
+00024880: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00024890: 2020 2020 662e 7772 6974 6528 275c 6e5c      f.write('\n\
+000248a0: 6e27 290a 2020 2020 2020 2020 662e 7772  n').        f.wr
+000248b0: 6974 6528 6d64 5f74 6162 6c65 290a 2020  ite(md_table).  
+000248c0: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
+000248d0: 7b6d 7367 7d20 7b66 696c 655f 7061 7468  {msg} {file_path
+000248e0: 7d22 290a 0a0a 6465 6620 7072 6570 6172  }")...def prepar
+000248f0: 655f 6d65 7461 6461 7461 5f66 6f72 5f77  e_metadata_for_w
+00024900: 7269 7469 6e67 286d 6574 6164 6174 615f  riting(metadata_
+00024910: 6466 293a 0a20 2020 2023 2063 6f6e 7665  df):.    # conve
+00024920: 7274 5f74 6f5f 7374 7220 3d20 7b63 3a20  rt_to_str = {c: 
+00024930: 2773 7472 696e 6727 2066 6f72 2063 2069  'string' for c i
+00024940: 6e20 2827 6c65 6e67 7468 5f71 6227 2c20  n ('length_qb', 
+00024950: 276c 656e 6774 685f 7162 5f75 6e66 6f6c  'length_qb_unfol
+00024960: 6465 6427 2c20 2761 6c6c 5f6e 6f74 6573  ded', 'all_notes
+00024970: 5f71 6227 2920 6966 2063 2069 6e20 6d65  _qb') if c in me
+00024980: 7461 6461 7461 5f64 667d 0a20 2020 2023  tadata_df}.    #
+00024990: 2069 6620 6c65 6e28 636f 6e76 6572 745f   if len(convert_
+000249a0: 746f 5f73 7472 2920 3e20 303a 0a20 2020  to_str) > 0:.   
+000249b0: 2023 2020 2020 206d 6574 6164 6174 615f   #     metadata_
+000249c0: 6466 203d 206d 6574 6164 6174 615f 6466  df = metadata_df
+000249d0: 2e61 7374 7970 6528 636f 6e76 6572 745f  .astype(convert_
+000249e0: 746f 5f73 7472 2c20 6572 726f 7273 3d27  to_str, errors='
+000249f0: 6967 6e6f 7265 2729 0a20 2020 206d 6574  ignore').    met
+00024a00: 6164 6174 615f 6466 203d 206d 6574 6164  adata_df = metad
+00024a10: 6174 615f 6466 2e61 7374 7970 6528 2773  ata_df.astype('s
+00024a20: 7472 696e 6727 2c20 6572 726f 7273 3d27  tring', errors='
+00024a30: 6967 6e6f 7265 2729 0a20 2020 206d 6574  ignore').    met
+00024a40: 6164 6174 615f 6466 2e73 6f72 745f 696e  adata_df.sort_in
+00024a50: 6465 7828 696e 706c 6163 653d 5472 7565  dex(inplace=True
+00024a60: 290a 2020 2020 6d65 7461 6461 7461 5f64  ).    metadata_d
+00024a70: 6620 3d20 636f 6c75 6d6e 5f6f 7264 6572  f = column_order
+00024a80: 286d 6574 6164 6174 615f 6466 2c20 4d45  (metadata_df, ME
+00024a90: 5441 4441 5441 5f43 4f4c 554d 4e5f 4f52  TADATA_COLUMN_OR
+00024aa0: 4445 522c 2073 6f72 743d 4661 6c73 6529  DER, sort=False)
+00024ab0: 0a20 2020 2023 206f 6e20 5769 6e64 6f77  .    # on Window
+00024ac0: 732c 206d 616b 6520 7375 7265 2074 6865  s, make sure the
+00024ad0: 2070 6174 6873 2061 7265 2077 7269 7474   paths are writt
+00024ae0: 656e 2077 6974 6820 2f20 7365 7061 7261  en with / separa
+00024af0: 746f 7273 0a20 2020 2070 6174 685f 636f  tors.    path_co
+00024b00: 6c73 203d 205b 636f 6c20 666f 7220 636f  ls = [col for co
+00024b10: 6c20 696e 2028 2773 7562 6469 7227 2c20  l in ('subdir', 
+00024b20: 2772 656c 5f70 6174 6827 2920 6966 2063  'rel_path') if c
+00024b30: 6f6c 2069 6e20 6d65 7461 6461 7461 5f64  ol in metadata_d
+00024b40: 662e 636f 6c75 6d6e 735d 0a20 2020 2066  f.columns].    f
+00024b50: 6f72 2063 6f6c 2069 6e20 7061 7468 5f63  or col in path_c
+00024b60: 6f6c 733a 0a20 2020 2020 2020 2077 6974  ols:.        wit
+00024b70: 6820 7761 726e 696e 6773 2e63 6174 6368  h warnings.catch
+00024b80: 5f77 6172 6e69 6e67 7328 293a 0a20 2020  _warnings():.   
+00024b90: 2020 2020 2020 2020 2023 2053 6574 7469           # Setti
+00024ba0: 6e67 2076 616c 7565 7320 696e 2d70 6c61  ng values in-pla
+00024bb0: 6365 2069 7320 6669 6e65 2c20 6967 6e6f  ce is fine, igno
+00024bc0: 7265 2074 6865 2077 6172 6e69 6e67 2069  re the warning i
+00024bd0: 6e20 5061 6e64 6173 203e 3d20 312e 352e  n Pandas >= 1.5.
+00024be0: 300a 2020 2020 2020 2020 2020 2020 2320  0.            # 
+00024bf0: 5468 6973 2063 616e 2062 6520 7265 6d6f  This can be remo
+00024c00: 7665 642c 2069 6620 5061 6e64 6173 2031  ved, if Pandas 1
+00024c10: 2e35 2e30 2064 6f65 7320 6e6f 7420 6e65  .5.0 does not ne
+00024c20: 6564 2074 6f20 6265 2073 7570 706f 7274  ed to be support
+00024c30: 6564 2061 6e79 206c 6f6e 6765 722e 0a20  ed any longer.. 
+00024c40: 2020 2020 2020 2020 2020 2023 2053 6565             # See
+00024c50: 2061 6c73 6f3a 2068 7474 7073 3a2f 2f73   also: https://s
+00024c60: 7461 636b 6f76 6572 666c 6f77 2e63 6f6d  tackoverflow.com
+00024c70: 2f71 2f37 3430 3537 3336 372f 3835 3935  /q/74057367/8595
+00024c80: 3931 0a20 2020 2020 2020 2020 2020 2077  91.            w
+00024c90: 6172 6e69 6e67 732e 6669 6c74 6572 7761  arnings.filterwa
+00024ca0: 726e 696e 6773 280a 2020 2020 2020 2020  rnings(.        
+00024cb0: 2020 2020 2020 2020 2269 676e 6f72 6522          "ignore"
+00024cc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00024cd0: 2020 6361 7465 676f 7279 3d46 7574 7572    category=Futur
+00024ce0: 6557 6172 6e69 6e67 2c0a 2020 2020 2020  eWarning,.      
+00024cf0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00024d00: 653d 280a 2020 2020 2020 2020 2020 2020  e=(.            
+00024d10: 2020 2020 2020 2020 222e 2a77 696c 6c20          ".*will 
+00024d20: 6174 7465 6d70 7420 746f 2073 6574 2074  attempt to set t
+00024d30: 6865 2076 616c 7565 7320 696e 706c 6163  he values inplac
+00024d40: 6520 696e 7374 6561 6420 6f66 2061 6c77  e instead of alw
+00024d50: 6179 7320 7365 7474 696e 6720 6120 6e65  ays setting a ne
+00024d60: 7720 6172 7261 792e 2022 0a20 2020 2020  w array. ".     
+00024d70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00024d80: 546f 2072 6574 6169 6e20 7468 6520 6f6c  To retain the ol
+00024d90: 6420 6265 6861 7669 6f72 2c20 7573 6520  d behavior, use 
+00024da0: 6569 7468 6572 2e2a 220a 2020 2020 2020  either.*".      
+00024db0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00024dc0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00024dd0: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
+00024de0: 6466 2e6c 6f63 5b3a 2c20 636f 6c5d 203d  df.loc[:, col] =
+00024df0: 206d 6574 6164 6174 615f 6466 5b63 6f6c   metadata_df[col
+00024e00: 5d2e 7374 722e 7265 706c 6163 6528 6f73  ].str.replace(os
+00024e10: 2e73 6570 2c20 272f 2729 0a20 2020 2073  .sep, '/').    s
+00024e20: 7461 6666 5f63 6f6c 732c 206f 7468 6572  taff_cols, other
+00024e30: 5f63 6f6c 7320 3d20 5b5d 2c20 5b5d 0a20  _cols = [], []. 
+00024e40: 2020 2066 6f72 2063 6f6c 2069 6e20 6d65     for col in me
+00024e50: 7461 6461 7461 5f64 662e 636f 6c75 6d6e  tadata_df.column
+00024e60: 733a 0a20 2020 2020 2020 2069 6620 7265  s:.        if re
+00024e70: 2e6d 6174 6368 2872 225e 7374 6166 665f  .match(r"^staff_
+00024e80: 285c 642b 2922 2c20 636f 6c29 3a0a 2020  (\d+)", col):.  
+00024e90: 2020 2020 2020 2020 2020 7374 6166 665f            staff_
+00024ea0: 636f 6c73 2e61 7070 656e 6428 636f 6c29  cols.append(col)
+00024eb0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00024ec0: 2020 2020 2020 2020 2020 206f 7468 6572             other
+00024ed0: 5f63 6f6c 732e 6170 7065 6e64 2863 6f6c  _cols.append(col
+00024ee0: 290a 2020 2020 7374 6166 665f 636f 6c73  ).    staff_cols
+00024ef0: 203d 2073 6f72 7465 6428 7374 6166 665f   = sorted(staff_
+00024f00: 636f 6c73 2c20 6b65 793d 6c61 6d62 6461  cols, key=lambda
+00024f10: 2073 3a20 696e 7428 7265 2e6d 6174 6368   s: int(re.match
+00024f20: 2872 225e 7374 6166 665f 285c 642b 2922  (r"^staff_(\d+)"
+00024f30: 2c20 7329 5b31 5d29 290a 2020 2020 6d65  , s)[1])).    me
+00024f40: 7461 6461 7461 5f64 6620 3d20 6d65 7461  tadata_df = meta
+00024f50: 6461 7461 5f64 665b 6f74 6865 725f 636f  data_df[other_co
+00024f60: 6c73 202b 2073 7461 6666 5f63 6f6c 735d  ls + staff_cols]
+00024f70: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
+00024f80: 7374 616e 6365 286d 6574 6164 6174 615f  stance(metadata_
+00024f90: 6466 2e69 6e64 6578 2c20 7064 2e52 616e  df.index, pd.Ran
+00024fa0: 6765 496e 6465 7829 3a0a 2020 2020 2020  geIndex):.      
+00024fb0: 2020 6d65 7461 6461 7461 5f64 6620 3d20    metadata_df = 
+00024fc0: 6d65 7461 6461 7461 5f64 662e 7265 7365  metadata_df.rese
+00024fd0: 745f 696e 6465 7828 290a 2020 2020 7265  t_index().    re
+00024fe0: 7475 726e 206d 6574 6164 6174 615f 6466  turn metadata_df
+00024ff0: 0a0a 0a40 6675 6e63 7469 6f6e 5f6c 6f67  ...@function_log
+00025000: 6765 720a 6465 6620 7772 6974 655f 7473  ger.def write_ts
+00025010: 7628 6466 2c20 6669 6c65 5f70 6174 682c  v(df, file_path,
+00025020: 2070 7265 5f70 726f 6365 7373 3d54 7275   pre_process=Tru
+00025030: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
+00025040: 2020 2222 2220 5772 6974 6520 6120 4461    """ Write a Da
+00025050: 7461 4672 616d 6520 746f 2061 2054 5356  taFrame to a TSV
+00025060: 206f 7220 4353 5620 6669 6c65 2062 6173   or CSV file bas
+00025070: 6564 206f 6e20 7468 6520 6578 7465 6e73  ed on the extens
+00025080: 696f 6e20 6f66 2027 6669 6c65 5f70 6174  ion of 'file_pat
+00025090: 6827 2e0a 2020 2020 5573 6573 3a20 3a70  h'..    Uses: :p
+000250a0: 793a 6675 6e63 3a60 6e6f 5f63 6f6c 6c65  y:func:`no_colle
+000250b0: 6374 696f 6e73 5f6e 6f5f 626f 6f6c 6561  ctions_no_boolea
+000250c0: 6e73 600a 0a20 2020 2050 6172 616d 6574  ns`..    Paramet
+000250d0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000250e0: 2d2d 0a20 2020 2064 6620 3a20 3a6f 626a  --.    df : :obj
+000250f0: 3a60 7061 6e64 6173 2e44 6174 6146 7261  :`pandas.DataFra
+00025100: 6d65 600a 2020 2020 2020 2020 4461 7461  me`.        Data
+00025110: 4672 616d 6520 746f 2077 7269 7465 2e0a  Frame to write..
+00025120: 2020 2020 6669 6c65 5f70 6174 6820 3a20      file_path : 
+00025130: 3a6f 626a 3a60 7374 7260 0a20 2020 2020  :obj:`str`.     
+00025140: 2020 2046 696c 6520 746f 2063 7265 6174     File to creat
+00025150: 6520 6f72 206f 7665 7277 7269 7465 2e20  e or overwrite. 
+00025160: 4966 2074 6865 2065 7874 656e 7369 6f6e  If the extension
+00025170: 2069 7320 2e74 7376 2c20 7468 6520 6172   is .tsv, the ar
+00025180: 6775 6d65 6e74 2027 7365 7027 2077 696c  gument 'sep' wil
+00025190: 6c20 6265 2073 6574 2074 6f20 275c 7427  l be set to '\t'
+000251a0: 2c20 6f74 6865 7277 6973 6520 7468 650a  , otherwise the.
+000251b0: 2020 2020 2020 2020 6578 7465 6e73 696f          extensio
+000251c0: 6e20 6973 2065 7870 6563 7465 6420 746f  n is expected to
+000251d0: 2062 6520 2e63 7376 2061 6e64 2074 6865   be .csv and the
+000251e0: 2064 6566 6175 6c74 2073 6570 6172 6174   default separat
+000251f0: 6f72 2027 2c27 2077 696c 6c20 6265 2075  or ',' will be u
+00025200: 7365 642e 0a20 2020 2070 7265 5f70 726f  sed..    pre_pro
+00025210: 6365 7373 203a 203a 6f62 6a3a 6062 6f6f  cess : :obj:`boo
+00025220: 6c60 2c20 6f70 7469 6f6e 616c 0a20 2020  l`, optional.   
+00025230: 2020 2020 2042 7920 6465 6661 756c 742c       By default,
+00025240: 2044 6174 6146 7261 6d65 2063 656c 6c73   DataFrame cells
+00025250: 2063 6f6e 7461 696e 696e 6720 6c69 7374   containing list
+00025260: 7320 616e 6420 7475 706c 6573 2077 696c  s and tuples wil
+00025270: 6c20 6265 2074 7261 6e73 666f 726d 6564  l be transformed
+00025280: 2074 6f20 7374 7269 6e67 7320 616e 6420   to strings and 
+00025290: 426f 6f6c 6561 6e73 2077 696c 6c20 6265  Booleans will be
+000252a0: 0a20 2020 2020 2020 2063 6f6e 7665 7274  .        convert
+000252b0: 6564 2074 6f20 3020 616e 6420 3120 286f  ed to 0 and 1 (o
+000252c0: 7468 6572 7769 7365 2074 6865 7920 7769  therwise they wi
+000252d0: 6c6c 2062 6520 7772 6974 7465 6e20 6f75  ll be written ou
+000252e0: 7420 6173 2054 7275 6520 616e 6420 4661  t as True and Fa
+000252f0: 6c73 6529 2e20 5061 7373 2046 616c 7365  lse). Pass False
+00025300: 2074 6f20 7072 6576 656e 742e 0a20 2020   to prevent..   
+00025310: 206b 7761 7267 7320 3a0a 2020 2020 2020   kwargs :.      
+00025320: 2020 4164 6469 7469 6f6e 616c 206b 6579    Additional key
+00025330: 776f 7264 2061 7267 756d 656e 7473 2077  word arguments w
+00025340: 696c 6c20 6265 2070 6173 7365 6420 6f6e  ill be passed on
+00025350: 2074 6f20 3a70 793a 6d65 7468 3a60 7061   to :py:meth:`pa
+00025360: 6e64 6173 2e44 6174 6146 7261 6d65 2e74  ndas.DataFrame.t
+00025370: 6f5f 6373 7660 2e0a 2020 2020 2020 2020  o_csv`..        
+00025380: 4465 6661 756c 7473 2061 7267 756d 656e  Defaults argumen
+00025390: 7473 2061 7265 2060 6069 6e64 6578 3d46  ts are ``index=F
+000253a0: 616c 7365 6060 2061 6e64 2060 6073 6570  alse`` and ``sep
+000253b0: 3d27 5c74 2760 6020 2861 7373 756d 696e  ='\t'`` (assumin
+000253c0: 6720 6578 7465 6e73 696f 6e20 272e 7473  g extension '.ts
+000253d0: 7627 2c20 7365 6520 6162 6f76 6529 2e0a  v', see above)..
+000253e0: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+000253f0: 202d 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e   -------.    Non
+00025400: 650a 2020 2020 2222 220a 2020 2020 7061  e.    """.    pa
+00025410: 7468 2c20 6669 6c65 203d 206f 732e 7061  th, file = os.pa
+00025420: 7468 2e73 706c 6974 2866 696c 655f 7061  th.split(file_pa
+00025430: 7468 290a 2020 2020 7061 7468 203d 2072  th).    path = r
+00025440: 6573 6f6c 7665 5f64 6972 2870 6174 6829  esolve_dir(path)
+00025450: 0a20 2020 206f 732e 7061 7468 2e6a 6f69  .    os.path.joi
+00025460: 6e28 7061 7468 2c20 6669 6c65 290a 2020  n(path, file).  
+00025470: 2020 666e 616d 652c 2065 7874 203d 206f    fname, ext = o
+00025480: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
+00025490: 6669 6c65 290a 2020 2020 6966 2065 7874  file).    if ext
+000254a0: 2e6c 6f77 6572 2829 206e 6f74 2069 6e20  .lower() not in 
+000254b0: 2827 2e74 7376 272c 2027 2e63 7376 2729  ('.tsv', '.csv')
+000254c0: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
+000254d0: 2e65 7272 6f72 2866 2254 6869 7320 6675  .error(f"This fu
+000254e0: 6e63 7469 6f6e 2065 7870 6563 7473 2066  nction expects f
+000254f0: 696c 655f 7061 7468 2074 6f20 696e 636c  ile_path to incl
+00025500: 7564 6520 7468 6520 6669 6c65 206e 616d  ude the file nam
+00025510: 6520 656e 6469 6e67 206f 6e20 2e63 7376  e ending on .csv
+00025520: 206f 7220 2e74 7376 2c20 6e6f 7420 277b   or .tsv, not '{
+00025530: 6578 747d 272e 2229 0a20 2020 2020 2020  ext}'.").       
+00025540: 2072 6574 7572 6e0a 2020 2020 6f73 2e6d   return.    os.m
+00025550: 616b 6564 6972 7328 7061 7468 2c20 6578  akedirs(path, ex
+00025560: 6973 745f 6f6b 3d54 7275 6529 0a20 2020  ist_ok=True).   
+00025570: 2069 6620 6578 742e 6c6f 7765 7228 2920   if ext.lower() 
+00025580: 3d3d 2027 2e74 7376 273a 0a20 2020 2020  == '.tsv':.     
+00025590: 2020 206b 7761 7267 732e 7570 6461 7465     kwargs.update
+000255a0: 2864 6963 7428 7365 703d 275c 7427 2929  (dict(sep='\t'))
+000255b0: 0a20 2020 2069 6620 2769 6e64 6578 2720  .    if 'index' 
+000255c0: 6e6f 7420 696e 206b 7761 7267 733a 0a20  not in kwargs:. 
+000255d0: 2020 2020 2020 206b 7761 7267 735b 2769         kwargs['i
+000255e0: 6e64 6578 275d 203d 2046 616c 7365 0a20  ndex'] = False. 
+000255f0: 2020 2069 6620 7072 655f 7072 6f63 6573     if pre_proces
+00025600: 733a 0a20 2020 2020 2020 2064 6620 3d20  s:.        df = 
+00025610: 6e6f 5f63 6f6c 6c65 6374 696f 6e73 5f6e  no_collections_n
+00025620: 6f5f 626f 6f6c 6561 6e73 2864 662c 206c  o_booleans(df, l
+00025630: 6f67 6765 723d 6c6f 6767 6572 290a 2020  ogger=logger).  
+00025640: 2020 6466 2e74 6f5f 6373 7628 6669 6c65    df.to_csv(file
+00025650: 5f70 6174 682c 202a 2a6b 7761 7267 7329  _path, **kwargs)
+00025660: 0a20 2020 206c 6f67 6765 722e 6465 6275  .    logger.debu
+00025670: 6728 6622 7b66 696c 655f 7061 7468 7d20  g(f"{file_path} 
+00025680: 7772 6974 7465 6e20 7769 7468 2070 6172  written with par
+00025690: 616d 6574 6572 7320 7b6b 7761 7267 737d  ameters {kwargs}
+000256a0: 2e22 290a 2020 2020 7265 7475 726e 0a0a  .").    return..
+000256b0: 0a40 6675 6e63 7469 6f6e 5f6c 6f67 6765  .@function_logge
+000256c0: 720a 6465 6620 6162 7332 7265 6c5f 6b65  r.def abs2rel_ke
+000256d0: 7928 6162 736f 6c75 7465 3a20 7374 722c  y(absolute: str,
+000256e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000256f0: 206c 6f63 616c 6b65 793a 2073 7472 2c0a   localkey: str,.
+00025700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025710: 676c 6f62 616c 5f6d 696e 6f72 3a20 626f  global_minor: bo
+00025720: 6f6c 203d 2046 616c 7365 2920 2d3e 2073  ol = False) -> s
+00025730: 7472 3a0a 2020 2020 2222 220a 2020 2020  tr:.    """.    
+00025740: 4578 7072 6573 7365 7320 6120 526f 6d61  Expresses a Roma
+00025750: 6e20 6e75 6d65 7261 6c20 6173 2073 6361  n numeral as sca
+00025760: 6c65 2064 6567 7265 6520 7265 6c61 7469  le degree relati
+00025770: 7665 2074 6f20 6120 6769 7665 6e20 6c6f  ve to a given lo
+00025780: 6361 6c6b 6579 2e0a 2020 2020 5468 6520  calkey..    The 
+00025790: 7265 7375 6c74 2063 6861 6e67 6573 2064  result changes d
+000257a0: 6570 656e 6469 6e67 206f 6e20 7768 6574  epending on whet
+000257b0: 6865 7220 526f 6d61 6e20 6e75 6d65 7261  her Roman numera
+000257c0: 6c20 616e 6420 6c6f 6361 6c6b 6579 2061  l and localkey a
+000257d0: 7265 0a20 2020 2069 6e74 6572 7072 6574  re.    interpret
+000257e0: 6564 2077 6974 6869 6e20 6120 676c 6f62  ed within a glob
+000257f0: 616c 206d 616a 6f72 206f 7220 6d69 6e6f  al major or mino
+00025800: 7220 6b65 792e 0a0a 2020 2020 5573 6573  r key...    Uses
+00025810: 3a20 3a70 793a 6675 6e63 3a60 7370 6c69  : :py:func:`spli
+00025820: 745f 7363 616c 655f 6465 6772 6565 600a  t_scale_degree`.
+00025830: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00025840: 2020 6162 736f 6c75 7465 3a20 4162 736f    absolute: Abso
+00025850: 6c75 7465 206b 6579 2065 7870 7265 7373  lute key express
+00025860: 6564 2061 7320 526f 6d61 6e20 7363 616c  ed as Roman scal
+00025870: 6520 6465 6772 6565 206f 6620 7468 6520  e degree of the 
+00025880: 6c6f 6361 6c20 6b65 792e 0a20 2020 2020  local key..     
+00025890: 206c 6f63 616c 6b65 793a 2054 6865 206c   localkey: The l
+000258a0: 6f63 616c 206b 6579 2069 6e20 7465 726d  ocal key in term
+000258b0: 7320 6f66 2077 6869 6368 2060 6061 6273  s of which ``abs
+000258c0: 6f6c 7574 6560 6020 7769 6c6c 2062 6520  olute`` will be 
+000258d0: 6578 7072 6573 7365 642e 0a20 2020 2020  expressed..     
+000258e0: 2067 6c6f 6261 6c5f 6d69 6e6f 723a 2048   global_minor: H
+000258f0: 6173 2074 6f20 6265 2073 6574 2074 6f20  as to be set to 
+00025900: 5472 7565 2069 6620 6061 6273 6f6c 7574  True if `absolut
+00025910: 6560 2061 6e64 2060 6c6f 6361 6c6b 6579  e` and `localkey
+00025920: 6020 6172 6520 7363 616c 6520 6465 6772  ` are scale degr
+00025930: 6565 7320 6f66 2061 2067 6c6f 6261 6c20  ees of a global 
+00025940: 6d69 6e6f 7220 6b65 792e 0a0a 2020 2020  minor key...    
+00025950: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+00025960: 496e 2061 206d 696e 6f72 2063 6f6e 7465  In a minor conte
+00025970: 7874 2c20 7468 6520 6b65 7920 6f66 2049  xt, the key of I
+00025980: 4920 776f 756c 6420 6170 7065 6172 2077  I would appear w
+00025990: 6974 6869 6e20 7468 6520 6b65 7920 6f66  ithin the key of
+000259a0: 2076 6969 2061 7320 2349 4949 2e0a 0a20   vii as #III... 
+000259b0: 2020 2020 2020 2020 203e 3e3e 2061 6273           >>> abs
+000259c0: 3272 656c 5f6b 6579 2827 6976 272c 2027  2rel_key('iv', '
+000259d0: 5649 272c 2067 6c6f 6261 6c5f 6d69 6e6f  VI', global_mino
+000259e0: 723d 4661 6c73 6529 0a20 2020 2020 2020  r=False).       
+000259f0: 2020 2027 6276 6927 2020 2020 2020 2023     'bvi'       #
+00025a00: 2046 206d 696e 6f72 2065 7870 7265 7373   F minor express
+00025a10: 6564 2077 6974 6820 7265 7370 6563 7420  ed with respect 
+00025a20: 746f 2041 206d 616a 6f72 0a20 2020 2020  to A major.     
+00025a30: 2020 2020 203e 3e3e 2061 6273 3272 656c       >>> abs2rel
+00025a40: 5f6b 6579 2827 6976 272c 2027 7669 272c  _key('iv', 'vi',
+00025a50: 2067 6c6f 6261 6c5f 6d69 6e6f 723d 4661   global_minor=Fa
+00025a60: 6c73 6529 0a20 2020 2020 2020 2020 2027  lse).          '
+00025a70: 7669 2720 2020 2020 2023 2046 206d 696e  vi'      # F min
+00025a80: 6f72 2065 7870 7265 7373 6564 2077 6974  or expressed wit
+00025a90: 6820 7265 7370 6563 7420 746f 2041 206d  h respect to A m
+00025aa0: 696e 6f72 0a20 2020 2020 2020 2020 203e  inor.          >
+00025ab0: 3e3e 2061 6273 3272 656c 5f6b 6579 2827  >> abs2rel_key('
+00025ac0: 6976 272c 2027 5649 272c 2067 6c6f 6261  iv', 'VI', globa
+00025ad0: 6c5f 6d69 6e6f 723d 5472 7565 290a 2020  l_minor=True).  
+00025ae0: 2020 2020 2020 2020 2776 6927 2020 2020          'vi'    
+00025af0: 2020 2320 4620 6d69 6e6f 7220 6578 7072    # F minor expr
+00025b00: 6573 7365 6420 7769 7468 2072 6573 7065  essed with respe
+00025b10: 6374 2074 6f20 4162 206d 616a 6f72 0a20  ct to Ab major. 
+00025b20: 2020 2020 2020 2020 203e 3e3e 2061 6273           >>> abs
+00025b30: 3272 656c 5f6b 6579 2827 6976 272c 2027  2rel_key('iv', '
+00025b40: 7669 272c 2067 6c6f 6261 6c5f 6d69 6e6f  vi', global_mino
+00025b50: 723d 5472 7565 290a 2020 2020 2020 2020  r=True).        
+00025b60: 2020 2723 7669 2720 2020 2020 2020 2320    '#vi'       # 
+00025b70: 4620 6d69 6e6f 7220 6578 7072 6573 7365  F minor expresse
+00025b80: 6420 7769 7468 2072 6573 7065 6374 2074  d with respect t
+00025b90: 6f20 4162 206d 696e 6f72 0a0a 2020 2020  o Ab minor..    
+00025ba0: 2020 2020 2020 3e3e 3e20 6162 7332 7265        >>> abs2re
+00025bb0: 6c5f 6b65 7928 2756 4927 2c20 2749 5627  l_key('VI', 'IV'
+00025bc0: 2c20 676c 6f62 616c 5f6d 696e 6f72 3d46  , global_minor=F
+00025bd0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00025be0: 2749 4949 2720 2020 2020 2020 2320 4120  'III'       # A 
+00025bf0: 6d61 6a6f 7220 6578 7072 6573 7365 6420  major expressed 
+00025c00: 7769 7468 2072 6573 7065 6374 2074 6f20  with respect to 
+00025c10: 4620 6d61 6a6f 720a 2020 2020 2020 2020  F major.        
+00025c20: 2020 3e3e 3e20 6162 7332 7265 6c5f 6b65    >>> abs2rel_ke
+00025c30: 7928 2756 4927 2c20 2769 7627 2c20 676c  y('VI', 'iv', gl
+00025c40: 6f62 616c 5f6d 696e 6f72 3d46 616c 7365  obal_minor=False
+00025c50: 290a 2020 2020 2020 2020 2020 2723 4949  ).          '#II
+00025c60: 4927 2020 2020 2020 2023 2041 206d 616a  I'       # A maj
+00025c70: 6f72 2065 7870 7265 7373 6564 2077 6974  or expressed wit
+00025c80: 6820 7265 7370 6563 7420 746f 2046 206d  h respect to F m
+00025c90: 696e 6f72 0a20 2020 2020 2020 2020 203e  inor.          >
+00025ca0: 3e3e 2061 6273 3272 656c 5f6b 6579 2827  >> abs2rel_key('
+00025cb0: 5649 272c 2027 4956 272c 2067 6c6f 6261  VI', 'IV', globa
+00025cc0: 6c5f 6d69 6e6f 723d 5472 7565 290a 2020  l_minor=True).  
+00025cd0: 2020 2020 2020 2020 2762 4949 4927 2020          'bIII'  
+00025ce0: 2020 2020 2023 2041 6220 6d61 6a6f 7220       # Ab major 
+00025cf0: 6578 7072 6573 7365 6420 7769 7468 2072  expressed with r
+00025d00: 6573 7065 6374 2074 6f20 4620 6d61 6a6f  espect to F majo
+00025d10: 720a 2020 2020 2020 2020 2020 3e3e 3e20  r.          >>> 
+00025d20: 6162 7332 7265 6c5f 6b65 7928 2756 4927  abs2rel_key('VI'
+00025d30: 2c20 2769 7627 2c20 676c 6f62 616c 5f6d  , 'iv', global_m
+00025d40: 696e 6f72 3d46 616c 7365 290a 2020 2020  inor=False).    
+00025d50: 2020 2020 2020 2749 4949 2720 2020 2020        'III'     
+00025d60: 2020 2320 4162 206d 616a 6f72 2065 7870    # Ab major exp
+00025d70: 7265 7373 6564 2077 6974 6820 7265 7370  ressed with resp
+00025d80: 6563 7420 746f 2046 206d 696e 6f72 0a20  ect to F minor. 
+00025d90: 2020 2022 2222 0a20 2020 2069 6620 7064     """.    if pd
+00025da0: 2e69 736e 756c 6c28 6162 736f 6c75 7465  .isnull(absolute
+00025db0: 2920 6f72 2070 642e 6973 6e75 6c6c 286c  ) or pd.isnull(l
+00025dc0: 6f63 616c 6b65 7929 3a0a 2020 2020 2020  ocalkey):.      
+00025dd0: 2020 7265 7475 726e 2061 6273 6f6c 7574    return absolut
+00025de0: 650a 2020 2020 6162 736f 6c75 7465 203d  e.    absolute =
+00025df0: 2072 6573 6f6c 7665 5f72 656c 6174 6976   resolve_relativ
+00025e00: 655f 6b65 7973 2861 6273 6f6c 7574 6529  e_keys(absolute)
+00025e10: 0a20 2020 206c 6f63 616c 6b65 7920 3d20  .    localkey = 
+00025e20: 7265 736f 6c76 655f 7265 6c61 7469 7665  resolve_relative
+00025e30: 5f6b 6579 7328 6c6f 6361 6c6b 6579 290a  _keys(localkey).
+00025e40: 2020 2020 6d61 6a5f 726e 203d 205b 2749      maj_rn = ['I
+00025e50: 272c 2027 4949 272c 2027 4949 4927 2c20  ', 'II', 'III', 
+00025e60: 2749 5627 2c20 2756 272c 2027 5649 272c  'IV', 'V', 'VI',
+00025e70: 2027 5649 4927 5d0a 2020 2020 6d69 6e5f   'VII'].    min_
+00025e80: 726e 203d 205b 2769 272c 2027 6969 272c  rn = ['i', 'ii',
+00025e90: 2027 6969 6927 2c20 2769 7627 2c20 2776   'iii', 'iv', 'v
+00025ea0: 272c 2027 7669 272c 2027 7669 6927 5d0a  ', 'vi', 'vii'].
+00025eb0: 2020 2020 7768 6974 655f 6b65 795f 6d61      white_key_ma
+00025ec0: 6a6f 725f 6163 6369 6465 6e74 616c 7320  jor_accidentals 
+00025ed0: 3d20 6e70 2e61 7272 6179 285b 5b30 2c20  = np.array([[0, 
+00025ee0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00025ef0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
 00025f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f10: 2020 2020 2020 2020 205b 302c 2031 2c20           [0, 1, 
-00025f20: 312c 2030 2c20 302c 2031 2c20 315d 2c0a  1, 0, 0, 1, 1],.
-00025f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f10: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00025f20: 302c 2030 2c20 312c 2030 2c20 302c 2030  0, 0, 1, 0, 0, 0
+00025f30: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
 00025f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f50: 2020 2020 2020 2020 2020 2020 5b30 2c20              [0, 
-00025f60: 302c 2030 2c20 2d31 2c20 302c 2030 2c20  0, 0, -1, 0, 0, 
-00025f70: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00025f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f60: 2020 5b30 2c20 312c 2031 2c20 302c 2030    [0, 1, 1, 0, 0
+00025f70: 2c20 312c 2031 5d2c 0a20 2020 2020 2020  , 1, 1],.       
 00025f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00025f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025fa0: 5b30 2c20 302c 2030 2c20 302c 2030 2c20  [0, 0, 0, 0, 0, 
-00025fb0: 302c 2031 5d2c 0a20 2020 2020 2020 2020  0, 1],.         
+00025fa0: 2020 2020 205b 302c 2030 2c20 302c 202d       [0, 0, 0, -
+00025fb0: 312c 2030 2c20 302c 2030 5d2c 0a20 2020  1, 0, 0, 0],.   
 00025fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00025fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025fe0: 2020 205b 302c 2030 2c20 312c 2030 2c20     [0, 0, 1, 0, 
-00025ff0: 302c 2031 2c20 315d 2c0a 2020 2020 2020  0, 1, 1],.      
+00025fe0: 2020 2020 2020 2020 205b 302c 2030 2c20           [0, 0, 
+00025ff0: 302c 2030 2c20 302c 2030 2c20 315d 2c0a  0, 0, 0, 0, 1],.
 00026000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00026010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026020: 2020 2020 2020 5b30 2c20 312c 2031 2c20        [0, 1, 1, 
-00026030: 302c 2031 2c20 312c 2031 5d5d 290a 2020  0, 1, 1, 1]]).  
-00026040: 2020 6162 735f 6163 6369 6465 6e74 616c    abs_accidental
-00026050: 732c 2061 6273 6f6c 7574 6520 3d20 7370  s, absolute = sp
-00026060: 6c69 745f 7363 616c 655f 6465 6772 6565  lit_scale_degree
-00026070: 2861 6273 6f6c 7574 652c 2063 6f75 6e74  (absolute, count
-00026080: 3d54 7275 652c 206c 6f67 6765 723d 6c6f  =True, logger=lo
-00026090: 6767 6572 290a 2020 2020 6c6f 6361 6c6b  gger).    localk
-000260a0: 6579 5f61 6363 6964 656e 7461 6c73 2c20  ey_accidentals, 
-000260b0: 6c6f 6361 6c6b 6579 203d 2073 706c 6974  localkey = split
-000260c0: 5f73 6361 6c65 5f64 6567 7265 6528 6c6f  _scale_degree(lo
-000260d0: 6361 6c6b 6579 2c20 636f 756e 743d 5472  calkey, count=Tr
-000260e0: 7565 2c20 6c6f 6767 6572 3d6c 6f67 6765  ue, logger=logge
-000260f0: 7229 0a20 2020 2072 6573 756c 7469 6e67  r).    resulting
-00026100: 5f61 6363 6964 656e 7461 6c73 203d 2061  _accidentals = a
-00026110: 6273 5f61 6363 6964 656e 7461 6c73 202d  bs_accidentals -
-00026120: 206c 6f63 616c 6b65 795f 6163 6369 6465   localkey_accide
-00026130: 6e74 616c 730a 2020 2020 6e75 6d65 7261  ntals.    numera
-00026140: 6c73 203d 206d 616a 5f72 6e20 6966 2061  ls = maj_rn if a
-00026150: 6273 6f6c 7574 652e 6973 7570 7065 7228  bsolute.isupper(
-00026160: 2920 656c 7365 206d 696e 5f72 6e0a 2020  ) else min_rn.  
-00026170: 2020 6c6f 6361 6c6b 6579 5f69 6e64 6578    localkey_index
-00026180: 203d 206d 616a 5f72 6e2e 696e 6465 7828   = maj_rn.index(
-00026190: 6c6f 6361 6c6b 6579 2e75 7070 6572 2829  localkey.upper()
-000261a0: 290a 2020 2020 7265 7375 6c74 5f69 6e64  ).    result_ind
-000261b0: 6578 203d 2028 6e75 6d65 7261 6c73 2e69  ex = (numerals.i
-000261c0: 6e64 6578 2861 6273 6f6c 7574 6529 202d  ndex(absolute) -
-000261d0: 206c 6f63 616c 6b65 795f 696e 6465 7829   localkey_index)
-000261e0: 2025 2037 0a20 2020 2072 6573 756c 745f   % 7.    result_
-000261f0: 6e75 6d65 7261 6c20 3d20 6e75 6d65 7261  numeral = numera
-00026200: 6c73 5b72 6573 756c 745f 696e 6465 785d  ls[result_index]
-00026210: 0a20 2020 2069 6620 6c6f 6361 6c6b 6579  .    if localkey
-00026220: 2e69 736c 6f77 6572 2829 2061 6e64 2072  .islower() and r
-00026230: 6573 756c 745f 696e 6465 7820 696e 205b  esult_index in [
-00026240: 322c 2035 2c20 365d 3a0a 2020 2020 2020  2, 5, 6]:.      
-00026250: 2020 7265 7375 6c74 696e 675f 6163 6369    resulting_acci
-00026260: 6465 6e74 616c 7320 2b3d 2031 0a20 2020  dentals += 1.   
-00026270: 2069 6620 676c 6f62 616c 5f6d 696e 6f72   if global_minor
-00026280: 3a0a 2020 2020 2020 2020 6c6f 6361 6c6b  :.        localk
-00026290: 6579 5f69 6e64 6578 203d 2028 6c6f 6361  ey_index = (loca
-000262a0: 6c6b 6579 5f69 6e64 6578 202d 2032 2920  lkey_index - 2) 
-000262b0: 2520 370a 2020 2020 7265 7375 6c74 696e  % 7.    resultin
-000262c0: 675f 6163 6369 6465 6e74 616c 7320 2d3d  g_accidentals -=
-000262d0: 2077 6869 7465 5f6b 6579 5f6d 616a 6f72   white_key_major
-000262e0: 5f61 6363 6964 656e 7461 6c73 5b6c 6f63  _accidentals[loc
-000262f0: 616c 6b65 795f 696e 6465 785d 5b72 6573  alkey_index][res
-00026300: 756c 745f 696e 6465 785d 0a20 2020 2061  ult_index].    a
-00026310: 6363 203d 2072 6573 756c 7469 6e67 5f61  cc = resulting_a
-00026320: 6363 6964 656e 7461 6c73 202a 2027 2327  ccidentals * '#'
-00026330: 2069 6620 7265 7375 6c74 696e 675f 6163   if resulting_ac
-00026340: 6369 6465 6e74 616c 7320 3e20 3020 656c  cidentals > 0 el
-00026350: 7365 202d 7265 7375 6c74 696e 675f 6163  se -resulting_ac
-00026360: 6369 6465 6e74 616c 7320 2a20 2762 270a  cidentals * 'b'.
-00026370: 2020 2020 7265 7475 726e 2061 6363 202b      return acc +
-00026380: 2072 6573 756c 745f 6e75 6d65 7261 6c0a   result_numeral.
-00026390: 0a0a 4066 756e 6374 696f 6e5f 6c6f 6767  ..@function_logg
-000263a0: 6572 0a64 6566 2072 656c 3261 6273 5f6b  er.def rel2abs_k
-000263b0: 6579 2872 656c 6174 6976 653a 2073 7472  ey(relative: str
-000263c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000263d0: 2020 6c6f 6361 6c6b 6579 3a20 7374 722c    localkey: str,
-000263e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000263f0: 2067 6c6f 6261 6c5f 6d69 6e6f 723a 2062   global_minor: b
-00026400: 6f6f 6c20 3d20 4661 6c73 6529 3a0a 2020  ool = False):.  
-00026410: 2020 2222 2245 7870 7265 7373 6573 2061    """Expresses a
-00026420: 2052 6f6d 616e 206e 756d 6572 616c 2074   Roman numeral t
-00026430: 6861 7420 6973 2065 7870 7265 7373 6564  hat is expressed
-00026440: 2072 656c 6174 6976 6520 746f 2061 206c   relative to a l
-00026450: 6f63 616c 6b65 790a 2020 2020 6173 2073  ocalkey.    as s
-00026460: 6361 6c65 2064 6567 7265 6520 6f66 2074  cale degree of t
-00026470: 6865 2067 6c6f 6261 6c20 6b65 792e 2046  he global key. F
-00026480: 6f72 206c 6f63 616c 206b 6579 7320 7b49  or local keys {I
-00026490: 4949 2c20 6969 692c 2056 492c 2076 692c  II, iii, VI, vi,
-000264a0: 2056 4949 2c20 7669 697d 0a20 2020 2074   VII, vii}.    t
-000264b0: 6865 2072 6573 756c 7420 6368 616e 6765  he result change
-000264c0: 7320 6465 7065 6e64 696e 6720 6f6e 2077  s depending on w
-000264d0: 6865 7468 6572 2074 6865 2067 6c6f 6261  hether the globa
-000264e0: 6c20 6b65 7920 6973 206d 616a 6f72 206f  l key is major o
-000264f0: 7220 6d69 6e6f 722e 0a0a 2020 2020 5573  r minor...    Us
-00026500: 6573 3a20 3a70 793a 6675 6e63 3a60 7370  es: :py:func:`sp
-00026510: 6c69 745f 7363 616c 655f 6465 6772 6565  lit_scale_degree
-00026520: 600a 0a0a 2020 2020 4172 6773 3a0a 2020  `...    Args:.  
-00026530: 2020 2020 7265 6c61 7469 7665 3a20 5265      relative: Re
-00026540: 6c61 7469 7665 206b 6579 206f 7220 6368  lative key or ch
-00026550: 6f72 6420 6578 7072 6573 7365 6420 6173  ord expressed as
-00026560: 2052 6f6d 616e 2073 6361 6c65 2064 6567   Roman scale deg
-00026570: 7265 6520 6f66 2074 6865 206c 6f63 616c  ree of the local
-00026580: 206b 6579 2e0a 2020 2020 2020 6c6f 6361   key..      loca
-00026590: 6c6b 6579 3a20 5468 6520 6c6f 6361 6c20  lkey: The local 
-000265a0: 6b65 7920 746f 2077 6869 6368 2060 7265  key to which `re
-000265b0: 6c60 2069 7320 7265 6c61 7469 7665 2e0a  l` is relative..
-000265c0: 2020 2020 2020 676c 6f62 616c 5f6d 696e        global_min
-000265d0: 6f72 3a20 4861 7320 746f 2062 6520 7365  or: Has to be se
-000265e0: 7420 746f 2054 7275 6520 6966 2060 6c6f  t to True if `lo
-000265f0: 6361 6c6b 6579 6020 6973 2061 2073 6361  calkey` is a sca
-00026600: 6c65 2064 6567 7265 6520 6f66 2061 2067  le degree of a g
-00026610: 6c6f 6261 6c20 6d69 6e6f 7220 6b65 792e  lobal minor key.
-00026620: 0a0a 2020 2020 4578 616d 706c 6573 3a0a  ..    Examples:.
-00026630: 2020 2020 2020 4966 2074 6865 206c 6162        If the lab
-00026640: 656c 2076 6969 6f36 2f56 4920 6170 7065  el viio6/VI appe
-00026650: 6172 7320 696e 2074 6865 2063 6f6e 7465  ars in the conte
-00026660: 7874 206f 6620 7468 6520 6c6f 6361 6c20  xt of the local 
-00026670: 6b65 7920 5649 206f 7220 7669 2c0a 2020  key VI or vi,.  
-00026680: 2020 2020 7468 6520 6162 736f 6c75 7465      the absolute
-00026690: 206b 6579 2074 6f20 7768 6963 6820 7669   key to which vi
-000266a0: 696f 3620 6170 706c 6965 7320 6465 7065  io6 applies depe
-000266b0: 6e64 7320 6f6e 2074 6865 2067 6c6f 6261  nds on the globa
-000266c0: 6c20 6b65 792e 0a20 2020 2020 2054 6865  l key..      The
-000266d0: 2063 6f6d 6d65 6e74 7320 6578 7072 6573   comments expres
-000266e0: 7320 7468 6520 6578 616d 706c 6573 2069  s the examples i
-000266f0: 6e20 7265 6c61 7469 6f6e 2074 6f20 676c  n relation to gl
-00026700: 6f62 616c 2043 206d 616a 6f72 206f 7220  obal C major or 
-00026710: 4320 6d69 6e6f 722e 0a0a 2020 2020 2020  C minor...      
-00026720: 2020 2020 3e3e 3e20 7265 6c32 6162 735f      >>> rel2abs_
-00026730: 6b65 7928 2776 6927 2c20 2756 4927 2c20  key('vi', 'VI', 
-00026740: 676c 6f62 616c 5f6d 696e 6f72 3d46 616c  global_minor=Fal
-00026750: 7365 290a 2020 2020 2020 2020 2020 2723  se).          '#
-00026760: 6976 2720 2020 2020 2020 2320 7669 206f  iv'       # vi o
-00026770: 6620 4120 6d61 6a6f 7220 3d20 4623 206d  f A major = F# m
-00026780: 696e 6f72 0a20 2020 2020 2020 2020 203e  inor.          >
-00026790: 3e3e 2072 656c 3261 6273 5f6b 6579 2827  >> rel2abs_key('
-000267a0: 7669 272c 2027 7669 272c 2067 6c6f 6261  vi', 'vi', globa
-000267b0: 6c5f 6d69 6e6f 723d 4661 6c73 6529 0a20  l_minor=False). 
-000267c0: 2020 2020 2020 2020 2027 6976 2720 2020           'iv'   
-000267d0: 2020 2023 2076 6920 6f66 2041 206d 696e     # vi of A min
-000267e0: 6f72 203d 2046 206d 696e 6f72 0a20 2020  or = F minor.   
-000267f0: 2020 2020 2020 203e 3e3e 2072 656c 3261         >>> rel2a
-00026800: 6273 5f6b 6579 2827 7669 272c 2027 5649  bs_key('vi', 'VI
-00026810: 272c 2067 6c6f 6261 6c5f 6d69 6e6f 723d  ', global_minor=
-00026820: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00026830: 2769 7627 2020 2020 2020 2320 7669 206f  'iv'      # vi o
-00026840: 6620 4162 206d 616a 6f72 203d 2046 206d  f Ab major = F m
-00026850: 696e 6f72 0a20 2020 2020 2020 2020 203e  inor.          >
-00026860: 3e3e 2072 656c 3261 6273 5f6b 6579 2827  >> rel2abs_key('
-00026870: 7669 272c 2027 7669 272c 2067 6c6f 6261  vi', 'vi', globa
-00026880: 6c5f 6d69 6e6f 723d 5472 7565 290a 2020  l_minor=True).  
-00026890: 2020 2020 2020 2020 2762 6976 2720 2020          'biv'   
-000268a0: 2020 2020 2320 7669 206f 6620 4162 206d      # vi of Ab m
-000268b0: 696e 6f72 203d 2046 6220 6d69 6e6f 720a  inor = Fb minor.
-000268c0: 0a20 2020 2020 2054 6865 2073 616d 6520  .      The same 
-000268d0: 6578 616d 706c 6573 2068 6f6c 6420 6966  examples hold if
-000268e0: 2079 6f75 2772 6520 6578 7072 6573 7369   you're expressi
-000268f0: 6e67 2069 6e20 7465 726d 7320 6f66 2074  ng in terms of t
-00026900: 6865 2067 6c6f 6261 6c20 6b65 790a 2020  he global key.  
-00026910: 2020 2020 7468 6520 726f 6f74 206f 6620      the root of 
-00026920: 6120 5649 2d63 686f 7264 2077 6974 6869  a VI-chord withi
-00026930: 6e20 7468 6520 6c6f 6361 6c20 6b65 7973  n the local keys
-00026940: 2056 4920 6f72 2076 692e 0a20 2020 2022   VI or vi..    "
-00026950: 2222 0a20 2020 2069 6620 7064 2e69 736e  "".    if pd.isn
-00026960: 756c 6c28 7265 6c61 7469 7665 2920 6f72  ull(relative) or
-00026970: 2070 642e 6973 6e75 6c6c 286c 6f63 616c   pd.isnull(local
-00026980: 6b65 7929 3a0a 2020 2020 2020 2020 7265  key):.        re
-00026990: 7475 726e 2072 656c 6174 6976 650a 2020  turn relative.  
-000269a0: 2020 7265 6c61 7469 7665 203d 2072 6573    relative = res
-000269b0: 6f6c 7665 5f72 656c 6174 6976 655f 6b65  olve_relative_ke
-000269c0: 7973 2872 656c 6174 6976 6529 0a20 2020  ys(relative).   
-000269d0: 206c 6f63 616c 6b65 7920 3d20 7265 736f   localkey = reso
-000269e0: 6c76 655f 7265 6c61 7469 7665 5f6b 6579  lve_relative_key
-000269f0: 7328 6c6f 6361 6c6b 6579 290a 2020 2020  s(localkey).    
-00026a00: 6d61 6a5f 726e 203d 205b 2749 272c 2027  maj_rn = ['I', '
-00026a10: 4949 272c 2027 4949 4927 2c20 2749 5627  II', 'III', 'IV'
-00026a20: 2c20 2756 272c 2027 5649 272c 2027 5649  , 'V', 'VI', 'VI
-00026a30: 4927 5d0a 2020 2020 6d69 6e5f 726e 203d  I'].    min_rn =
-00026a40: 205b 2769 272c 2027 6969 272c 2027 6969   ['i', 'ii', 'ii
-00026a50: 6927 2c20 2769 7627 2c20 2776 272c 2027  i', 'iv', 'v', '
-00026a60: 7669 272c 2027 7669 6927 5d0a 2020 2020  vi', 'vii'].    
-00026a70: 7768 6974 655f 6b65 795f 6d61 6a6f 725f  white_key_major_
-00026a80: 6163 6369 6465 6e74 616c 7320 3d20 6e70  accidentals = np
-00026a90: 2e61 7272 6179 285b 5b30 2c20 302c 2030  .array([[0, 0, 0
-00026aa0: 2c20 302c 2030 2c20 302c 2030 5d2c 0a20  , 0, 0, 0, 0],. 
-00026ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026ad0: 2020 2020 2020 2020 2020 2020 5b30 2c20              [0, 
-00026ae0: 302c 2031 2c20 302c 2030 2c20 302c 2031  0, 1, 0, 0, 0, 1
-00026af0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00026020: 2020 2020 2020 2020 2020 2020 5b30 2c20              [0, 
+00026030: 302c 2031 2c20 302c 2030 2c20 312c 2031  0, 1, 0, 0, 1, 1
+00026040: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00026050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026060: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00026070: 302c 2031 2c20 312c 2030 2c20 312c 2031  0, 1, 1, 0, 1, 1
+00026080: 2c20 315d 5d29 0a20 2020 2061 6273 5f61  , 1]]).    abs_a
+00026090: 6363 6964 656e 7461 6c73 2c20 6162 736f  ccidentals, abso
+000260a0: 6c75 7465 203d 2073 706c 6974 5f73 6361  lute = split_sca
+000260b0: 6c65 5f64 6567 7265 6528 6162 736f 6c75  le_degree(absolu
+000260c0: 7465 2c20 636f 756e 743d 5472 7565 2c20  te, count=True, 
+000260d0: 6c6f 6767 6572 3d6c 6f67 6765 7229 0a20  logger=logger). 
+000260e0: 2020 206c 6f63 616c 6b65 795f 6163 6369     localkey_acci
+000260f0: 6465 6e74 616c 732c 206c 6f63 616c 6b65  dentals, localke
+00026100: 7920 3d20 7370 6c69 745f 7363 616c 655f  y = split_scale_
+00026110: 6465 6772 6565 286c 6f63 616c 6b65 792c  degree(localkey,
+00026120: 2063 6f75 6e74 3d54 7275 652c 206c 6f67   count=True, log
+00026130: 6765 723d 6c6f 6767 6572 290a 2020 2020  ger=logger).    
+00026140: 7265 7375 6c74 696e 675f 6163 6369 6465  resulting_accide
+00026150: 6e74 616c 7320 3d20 6162 735f 6163 6369  ntals = abs_acci
+00026160: 6465 6e74 616c 7320 2d20 6c6f 6361 6c6b  dentals - localk
+00026170: 6579 5f61 6363 6964 656e 7461 6c73 0a20  ey_accidentals. 
+00026180: 2020 206e 756d 6572 616c 7320 3d20 6d61     numerals = ma
+00026190: 6a5f 726e 2069 6620 6162 736f 6c75 7465  j_rn if absolute
+000261a0: 2e69 7375 7070 6572 2829 2065 6c73 6520  .isupper() else 
+000261b0: 6d69 6e5f 726e 0a20 2020 206c 6f63 616c  min_rn.    local
+000261c0: 6b65 795f 696e 6465 7820 3d20 6d61 6a5f  key_index = maj_
+000261d0: 726e 2e69 6e64 6578 286c 6f63 616c 6b65  rn.index(localke
+000261e0: 792e 7570 7065 7228 2929 0a20 2020 2072  y.upper()).    r
+000261f0: 6573 756c 745f 696e 6465 7820 3d20 286e  esult_index = (n
+00026200: 756d 6572 616c 732e 696e 6465 7828 6162  umerals.index(ab
+00026210: 736f 6c75 7465 2920 2d20 6c6f 6361 6c6b  solute) - localk
+00026220: 6579 5f69 6e64 6578 2920 2520 370a 2020  ey_index) % 7.  
+00026230: 2020 7265 7375 6c74 5f6e 756d 6572 616c    result_numeral
+00026240: 203d 206e 756d 6572 616c 735b 7265 7375   = numerals[resu
+00026250: 6c74 5f69 6e64 6578 5d0a 2020 2020 6966  lt_index].    if
+00026260: 206c 6f63 616c 6b65 792e 6973 6c6f 7765   localkey.islowe
+00026270: 7228 2920 616e 6420 7265 7375 6c74 5f69  r() and result_i
+00026280: 6e64 6578 2069 6e20 5b32 2c20 352c 2036  ndex in [2, 5, 6
+00026290: 5d3a 0a20 2020 2020 2020 2072 6573 756c  ]:.        resul
+000262a0: 7469 6e67 5f61 6363 6964 656e 7461 6c73  ting_accidentals
+000262b0: 202b 3d20 310a 2020 2020 6966 2067 6c6f   += 1.    if glo
+000262c0: 6261 6c5f 6d69 6e6f 723a 0a20 2020 2020  bal_minor:.     
+000262d0: 2020 206c 6f63 616c 6b65 795f 696e 6465     localkey_inde
+000262e0: 7820 3d20 286c 6f63 616c 6b65 795f 696e  x = (localkey_in
+000262f0: 6465 7820 2d20 3229 2025 2037 0a20 2020  dex - 2) % 7.   
+00026300: 2072 6573 756c 7469 6e67 5f61 6363 6964   resulting_accid
+00026310: 656e 7461 6c73 202d 3d20 7768 6974 655f  entals -= white_
+00026320: 6b65 795f 6d61 6a6f 725f 6163 6369 6465  key_major_accide
+00026330: 6e74 616c 735b 6c6f 6361 6c6b 6579 5f69  ntals[localkey_i
+00026340: 6e64 6578 5d5b 7265 7375 6c74 5f69 6e64  ndex][result_ind
+00026350: 6578 5d0a 2020 2020 6163 6320 3d20 7265  ex].    acc = re
+00026360: 7375 6c74 696e 675f 6163 6369 6465 6e74  sulting_accident
+00026370: 616c 7320 2a20 2723 2720 6966 2072 6573  als * '#' if res
+00026380: 756c 7469 6e67 5f61 6363 6964 656e 7461  ulting_accidenta
+00026390: 6c73 203e 2030 2065 6c73 6520 2d72 6573  ls > 0 else -res
+000263a0: 756c 7469 6e67 5f61 6363 6964 656e 7461  ulting_accidenta
+000263b0: 6c73 202a 2027 6227 0a20 2020 2072 6574  ls * 'b'.    ret
+000263c0: 7572 6e20 6163 6320 2b20 7265 7375 6c74  urn acc + result
+000263d0: 5f6e 756d 6572 616c 0a0a 0a40 6675 6e63  _numeral...@func
+000263e0: 7469 6f6e 5f6c 6f67 6765 720a 6465 6620  tion_logger.def 
+000263f0: 7265 6c32 6162 735f 6b65 7928 7265 6c61  rel2abs_key(rela
+00026400: 7469 7665 3a20 7374 722c 0a20 2020 2020  tive: str,.     
+00026410: 2020 2020 2020 2020 2020 206c 6f63 616c             local
+00026420: 6b65 793a 2073 7472 2c0a 2020 2020 2020  key: str,.      
+00026430: 2020 2020 2020 2020 2020 676c 6f62 616c            global
+00026440: 5f6d 696e 6f72 3a20 626f 6f6c 203d 2046  _minor: bool = F
+00026450: 616c 7365 293a 0a20 2020 2022 2222 4578  alse):.    """Ex
+00026460: 7072 6573 7365 7320 6120 526f 6d61 6e20  presses a Roman 
+00026470: 6e75 6d65 7261 6c20 7468 6174 2069 7320  numeral that is 
+00026480: 6578 7072 6573 7365 6420 7265 6c61 7469  expressed relati
+00026490: 7665 2074 6f20 6120 6c6f 6361 6c6b 6579  ve to a localkey
+000264a0: 0a20 2020 2061 7320 7363 616c 6520 6465  .    as scale de
+000264b0: 6772 6565 206f 6620 7468 6520 676c 6f62  gree of the glob
+000264c0: 616c 206b 6579 2e20 466f 7220 6c6f 6361  al key. For loca
+000264d0: 6c20 6b65 7973 207b 4949 492c 2069 6969  l keys {III, iii
+000264e0: 2c20 5649 2c20 7669 2c20 5649 492c 2076  , VI, vi, VII, v
+000264f0: 6969 7d0a 2020 2020 7468 6520 7265 7375  ii}.    the resu
+00026500: 6c74 2063 6861 6e67 6573 2064 6570 656e  lt changes depen
+00026510: 6469 6e67 206f 6e20 7768 6574 6865 7220  ding on whether 
+00026520: 7468 6520 676c 6f62 616c 206b 6579 2069  the global key i
+00026530: 7320 6d61 6a6f 7220 6f72 206d 696e 6f72  s major or minor
+00026540: 2e0a 0a20 2020 2055 7365 733a 203a 7079  ...    Uses: :py
+00026550: 3a66 756e 633a 6073 706c 6974 5f73 6361  :func:`split_sca
+00026560: 6c65 5f64 6567 7265 6560 0a0a 0a20 2020  le_degree`...   
+00026570: 2041 7267 733a 0a20 2020 2020 2072 656c   Args:.      rel
+00026580: 6174 6976 653a 2052 656c 6174 6976 6520  ative: Relative 
+00026590: 6b65 7920 6f72 2063 686f 7264 2065 7870  key or chord exp
+000265a0: 7265 7373 6564 2061 7320 526f 6d61 6e20  ressed as Roman 
+000265b0: 7363 616c 6520 6465 6772 6565 206f 6620  scale degree of 
+000265c0: 7468 6520 6c6f 6361 6c20 6b65 792e 0a20  the local key.. 
+000265d0: 2020 2020 206c 6f63 616c 6b65 793a 2054       localkey: T
+000265e0: 6865 206c 6f63 616c 206b 6579 2074 6f20  he local key to 
+000265f0: 7768 6963 6820 6072 656c 6020 6973 2072  which `rel` is r
+00026600: 656c 6174 6976 652e 0a20 2020 2020 2067  elative..      g
+00026610: 6c6f 6261 6c5f 6d69 6e6f 723a 2048 6173  lobal_minor: Has
+00026620: 2074 6f20 6265 2073 6574 2074 6f20 5472   to be set to Tr
+00026630: 7565 2069 6620 606c 6f63 616c 6b65 7960  ue if `localkey`
+00026640: 2069 7320 6120 7363 616c 6520 6465 6772   is a scale degr
+00026650: 6565 206f 6620 6120 676c 6f62 616c 206d  ee of a global m
+00026660: 696e 6f72 206b 6579 2e0a 0a20 2020 2045  inor key...    E
+00026670: 7861 6d70 6c65 733a 0a20 2020 2020 2049  xamples:.      I
+00026680: 6620 7468 6520 6c61 6265 6c20 7669 696f  f the label viio
+00026690: 362f 5649 2061 7070 6561 7273 2069 6e20  6/VI appears in 
+000266a0: 7468 6520 636f 6e74 6578 7420 6f66 2074  the context of t
+000266b0: 6865 206c 6f63 616c 206b 6579 2056 4920  he local key VI 
+000266c0: 6f72 2076 692c 0a20 2020 2020 2074 6865  or vi,.      the
+000266d0: 2061 6273 6f6c 7574 6520 6b65 7920 746f   absolute key to
+000266e0: 2077 6869 6368 2076 6969 6f36 2061 7070   which viio6 app
+000266f0: 6c69 6573 2064 6570 656e 6473 206f 6e20  lies depends on 
+00026700: 7468 6520 676c 6f62 616c 206b 6579 2e0a  the global key..
+00026710: 2020 2020 2020 5468 6520 636f 6d6d 656e        The commen
+00026720: 7473 2065 7870 7265 7373 2074 6865 2065  ts express the e
+00026730: 7861 6d70 6c65 7320 696e 2072 656c 6174  xamples in relat
+00026740: 696f 6e20 746f 2067 6c6f 6261 6c20 4320  ion to global C 
+00026750: 6d61 6a6f 7220 6f72 2043 206d 696e 6f72  major or C minor
+00026760: 2e0a 0a20 2020 2020 2020 2020 203e 3e3e  ...          >>>
+00026770: 2072 656c 3261 6273 5f6b 6579 2827 7669   rel2abs_key('vi
+00026780: 272c 2027 5649 272c 2067 6c6f 6261 6c5f  ', 'VI', global_
+00026790: 6d69 6e6f 723d 4661 6c73 6529 0a20 2020  minor=False).   
+000267a0: 2020 2020 2020 2027 2369 7627 2020 2020         '#iv'    
+000267b0: 2020 2023 2076 6920 6f66 2041 206d 616a     # vi of A maj
+000267c0: 6f72 203d 2046 2320 6d69 6e6f 720a 2020  or = F# minor.  
+000267d0: 2020 2020 2020 2020 3e3e 3e20 7265 6c32          >>> rel2
+000267e0: 6162 735f 6b65 7928 2776 6927 2c20 2776  abs_key('vi', 'v
+000267f0: 6927 2c20 676c 6f62 616c 5f6d 696e 6f72  i', global_minor
+00026800: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00026810: 2020 2769 7627 2020 2020 2020 2320 7669    'iv'      # vi
+00026820: 206f 6620 4120 6d69 6e6f 7220 3d20 4620   of A minor = F 
+00026830: 6d69 6e6f 720a 2020 2020 2020 2020 2020  minor.          
+00026840: 3e3e 3e20 7265 6c32 6162 735f 6b65 7928  >>> rel2abs_key(
+00026850: 2776 6927 2c20 2756 4927 2c20 676c 6f62  'vi', 'VI', glob
+00026860: 616c 5f6d 696e 6f72 3d54 7275 6529 0a20  al_minor=True). 
+00026870: 2020 2020 2020 2020 2027 6976 2720 2020           'iv'   
+00026880: 2020 2023 2076 6920 6f66 2041 6220 6d61     # vi of Ab ma
+00026890: 6a6f 7220 3d20 4620 6d69 6e6f 720a 2020  jor = F minor.  
+000268a0: 2020 2020 2020 2020 3e3e 3e20 7265 6c32          >>> rel2
+000268b0: 6162 735f 6b65 7928 2776 6927 2c20 2776  abs_key('vi', 'v
+000268c0: 6927 2c20 676c 6f62 616c 5f6d 696e 6f72  i', global_minor
+000268d0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+000268e0: 2027 6269 7627 2020 2020 2020 2023 2076   'biv'       # v
+000268f0: 6920 6f66 2041 6220 6d69 6e6f 7220 3d20  i of Ab minor = 
+00026900: 4662 206d 696e 6f72 0a0a 2020 2020 2020  Fb minor..      
+00026910: 5468 6520 7361 6d65 2065 7861 6d70 6c65  The same example
+00026920: 7320 686f 6c64 2069 6620 796f 7527 7265  s hold if you're
+00026930: 2065 7870 7265 7373 696e 6720 696e 2074   expressing in t
+00026940: 6572 6d73 206f 6620 7468 6520 676c 6f62  erms of the glob
+00026950: 616c 206b 6579 0a20 2020 2020 2074 6865  al key.      the
+00026960: 2072 6f6f 7420 6f66 2061 2056 492d 6368   root of a VI-ch
+00026970: 6f72 6420 7769 7468 696e 2074 6865 206c  ord within the l
+00026980: 6f63 616c 206b 6579 7320 5649 206f 7220  ocal keys VI or 
+00026990: 7669 2e0a 2020 2020 2222 220a 2020 2020  vi..    """.    
+000269a0: 6966 2070 642e 6973 6e75 6c6c 2872 656c  if pd.isnull(rel
+000269b0: 6174 6976 6529 206f 7220 7064 2e69 736e  ative) or pd.isn
+000269c0: 756c 6c28 6c6f 6361 6c6b 6579 293a 0a20  ull(localkey):. 
+000269d0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000269e0: 6c61 7469 7665 0a20 2020 2072 656c 6174  lative.    relat
+000269f0: 6976 6520 3d20 7265 736f 6c76 655f 7265  ive = resolve_re
+00026a00: 6c61 7469 7665 5f6b 6579 7328 7265 6c61  lative_keys(rela
+00026a10: 7469 7665 290a 2020 2020 6c6f 6361 6c6b  tive).    localk
+00026a20: 6579 203d 2072 6573 6f6c 7665 5f72 656c  ey = resolve_rel
+00026a30: 6174 6976 655f 6b65 7973 286c 6f63 616c  ative_keys(local
+00026a40: 6b65 7929 0a20 2020 206d 616a 5f72 6e20  key).    maj_rn 
+00026a50: 3d20 5b27 4927 2c20 2749 4927 2c20 2749  = ['I', 'II', 'I
+00026a60: 4949 272c 2027 4956 272c 2027 5627 2c20  II', 'IV', 'V', 
+00026a70: 2756 4927 2c20 2756 4949 275d 0a20 2020  'VI', 'VII'].   
+00026a80: 206d 696e 5f72 6e20 3d20 5b27 6927 2c20   min_rn = ['i', 
+00026a90: 2769 6927 2c20 2769 6969 272c 2027 6976  'ii', 'iii', 'iv
+00026aa0: 272c 2027 7627 2c20 2776 6927 2c20 2776  ', 'v', 'vi', 'v
+00026ab0: 6969 275d 0a20 2020 2077 6869 7465 5f6b  ii'].    white_k
+00026ac0: 6579 5f6d 616a 6f72 5f61 6363 6964 656e  ey_major_acciden
+00026ad0: 7461 6c73 203d 206e 702e 6172 7261 7928  tals = np.array(
+00026ae0: 5b5b 302c 2030 2c20 302c 2030 2c20 302c  [[0, 0, 0, 0, 0,
+00026af0: 2030 2c20 305d 2c0a 2020 2020 2020 2020   0, 0],.        
 00026b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00026b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026b20: 5b30 2c20 312c 2031 2c20 302c 2030 2c20  [0, 1, 1, 0, 0, 
-00026b30: 312c 2031 5d2c 0a20 2020 2020 2020 2020  1, 1],.         
+00026b20: 2020 2020 205b 302c 2030 2c20 312c 2030       [0, 0, 1, 0
+00026b30: 2c20 302c 2030 2c20 315d 2c0a 2020 2020  , 0, 0, 1],.    
 00026b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00026b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026b60: 2020 2020 5b30 2c20 302c 2030 2c20 2d31      [0, 0, 0, -1
-00026b70: 2c20 302c 2030 2c20 305d 2c0a 2020 2020  , 0, 0, 0],.    
+00026b60: 2020 2020 2020 2020 205b 302c 2031 2c20           [0, 1, 
+00026b70: 312c 2030 2c20 302c 2031 2c20 315d 2c0a  1, 0, 0, 1, 1],.
 00026b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00026b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026ba0: 2020 2020 2020 2020 205b 302c 2030 2c20           [0, 0, 
-00026bb0: 302c 2030 2c20 302c 2030 2c20 315d 2c0a  0, 0, 0, 0, 1],.
-00026bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026ba0: 2020 2020 2020 2020 2020 2020 205b 302c               [0,
+00026bb0: 2030 2c20 302c 202d 312c 2030 2c20 302c   0, 0, -1, 0, 0,
+00026bc0: 2030 5d2c 0a20 2020 2020 2020 2020 2020   0],.           
 00026bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026be0: 2020 2020 2020 2020 2020 2020 205b 302c               [0,
-00026bf0: 2030 2c20 312c 2030 2c20 302c 2031 2c20   0, 1, 0, 0, 1, 
-00026c00: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00026be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026bf0: 2020 5b30 2c20 302c 2030 2c20 302c 2030    [0, 0, 0, 0, 0
+00026c00: 2c20 302c 2031 5d2c 0a20 2020 2020 2020  , 0, 1],.       
 00026c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00026c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c30: 205b 302c 2031 2c20 312c 2030 2c20 312c   [0, 1, 1, 0, 1,
-00026c40: 2031 2c20 315d 5d29 0a20 2020 2072 656c   1, 1]]).    rel
-00026c50: 6174 6976 655f 6163 6369 6465 6e74 616c  ative_accidental
-00026c60: 732c 2072 656c 6174 6976 6520 3d20 7370  s, relative = sp
-00026c70: 6c69 745f 7363 616c 655f 6465 6772 6565  lit_scale_degree
-00026c80: 2872 656c 6174 6976 652c 2063 6f75 6e74  (relative, count
-00026c90: 3d54 7275 652c 206c 6f67 6765 723d 6c6f  =True, logger=lo
-00026ca0: 6767 6572 290a 2020 2020 6c6f 6361 6c6b  gger).    localk
-00026cb0: 6579 5f61 6363 6964 656e 7461 6c73 2c20  ey_accidentals, 
-00026cc0: 6c6f 6361 6c6b 6579 203d 2073 706c 6974  localkey = split
-00026cd0: 5f73 6361 6c65 5f64 6567 7265 6528 6c6f  _scale_degree(lo
-00026ce0: 6361 6c6b 6579 2c20 636f 756e 743d 5472  calkey, count=Tr
-00026cf0: 7565 2c20 6c6f 6767 6572 3d6c 6f67 6765  ue, logger=logge
-00026d00: 7229 0a20 2020 2072 6573 756c 7469 6e67  r).    resulting
-00026d10: 5f61 6363 6964 656e 7461 6c73 203d 2072  _accidentals = r
-00026d20: 656c 6174 6976 655f 6163 6369 6465 6e74  elative_accident
-00026d30: 616c 7320 2b20 6c6f 6361 6c6b 6579 5f61  als + localkey_a
-00026d40: 6363 6964 656e 7461 6c73 0a20 2020 206e  ccidentals.    n
-00026d50: 756d 6572 616c 7320 3d20 6d61 6a5f 726e  umerals = maj_rn
-00026d60: 2069 6620 7265 6c61 7469 7665 2e69 7375   if relative.isu
-00026d70: 7070 6572 2829 2065 6c73 6520 6d69 6e5f  pper() else min_
-00026d80: 726e 0a20 2020 2072 656c 5f6e 756d 203d  rn.    rel_num =
-00026d90: 206e 756d 6572 616c 732e 696e 6465 7828   numerals.index(
-00026da0: 7265 6c61 7469 7665 290a 2020 2020 6c6f  relative).    lo
-00026db0: 6361 6c6b 6579 5f69 6e64 6578 203d 206d  calkey_index = m
-00026dc0: 616a 5f72 6e2e 696e 6465 7828 6c6f 6361  aj_rn.index(loca
-00026dd0: 6c6b 6579 2e75 7070 6572 2829 290a 2020  lkey.upper()).  
-00026de0: 2020 7265 7375 6c74 5f6e 756d 6572 616c    result_numeral
-00026df0: 203d 206e 756d 6572 616c 735b 2872 656c   = numerals[(rel
-00026e00: 5f6e 756d 202b 206c 6f63 616c 6b65 795f  _num + localkey_
-00026e10: 696e 6465 7829 2025 2037 5d0a 2020 2020  index) % 7].    
-00026e20: 6966 206c 6f63 616c 6b65 792e 6973 6c6f  if localkey.islo
-00026e30: 7765 7228 2920 616e 6420 7265 6c5f 6e75  wer() and rel_nu
-00026e40: 6d20 696e 205b 322c 2035 2c20 365d 3a0a  m in [2, 5, 6]:.
-00026e50: 2020 2020 2020 2020 7265 7375 6c74 696e          resultin
-00026e60: 675f 6163 6369 6465 6e74 616c 7320 2d3d  g_accidentals -=
-00026e70: 2031 0a20 2020 2069 6620 676c 6f62 616c   1.    if global
-00026e80: 5f6d 696e 6f72 3a0a 2020 2020 2020 2020  _minor:.        
-00026e90: 6c6f 6361 6c6b 6579 5f69 6e64 6578 203d  localkey_index =
-00026ea0: 2028 6c6f 6361 6c6b 6579 5f69 6e64 6578   (localkey_index
-00026eb0: 202d 2032 2920 2520 370a 2020 2020 7265   - 2) % 7.    re
-00026ec0: 7375 6c74 696e 675f 6163 6369 6465 6e74  sulting_accident
-00026ed0: 616c 7320 2b3d 2077 6869 7465 5f6b 6579  als += white_key
-00026ee0: 5f6d 616a 6f72 5f61 6363 6964 656e 7461  _major_accidenta
-00026ef0: 6c73 5b72 656c 5f6e 756d 5d5b 6c6f 6361  ls[rel_num][loca
-00026f00: 6c6b 6579 5f69 6e64 6578 5d0a 2020 2020  lkey_index].    
-00026f10: 6163 6320 3d20 7265 7375 6c74 696e 675f  acc = resulting_
-00026f20: 6163 6369 6465 6e74 616c 7320 2a20 2723  accidentals * '#
-00026f30: 2720 6966 2072 6573 756c 7469 6e67 5f61  ' if resulting_a
-00026f40: 6363 6964 656e 7461 6c73 203e 2030 2065  ccidentals > 0 e
-00026f50: 6c73 6520 2d72 6573 756c 7469 6e67 5f61  lse -resulting_a
-00026f60: 6363 6964 656e 7461 6c73 202a 2027 6227  ccidentals * 'b'
-00026f70: 0a20 2020 2072 6574 7572 6e20 6163 6320  .    return acc 
-00026f80: 2b20 7265 7375 6c74 5f6e 756d 6572 616c  + result_numeral
-00026f90: 0a0a 0a40 6675 6e63 7469 6f6e 5f6c 6f67  ...@function_log
-00026fa0: 6765 720a 6465 6620 6d61 6b65 5f69 6e74  ger.def make_int
-00026fb0: 6572 7661 6c5f 696e 6465 785f 6672 6f6d  erval_index_from
-00026fc0: 5f64 7572 6174 696f 6e73 2864 662c 2070  _durations(df, p
-00026fd0: 6f73 6974 696f 6e5f 636f 6c3d 2771 7561  osition_col='qua
-00026fe0: 7274 6572 6265 6174 7327 2c20 6475 7261  rterbeats', dura
-00026ff0: 7469 6f6e 5f63 6f6c 3d27 6475 7261 7469  tion_col='durati
-00027000: 6f6e 5f71 6227 2c20 636c 6f73 6564 3d27  on_qb', closed='
-00027010: 6c65 6674 272c 0a20 2020 2020 2020 2020  left',.         
-00027020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027030: 2020 2020 2020 726f 756e 643d 4e6f 6e65        round=None
-00027040: 2c20 6e61 6d65 3d27 696e 7465 7276 616c  , name='interval
-00027050: 2729 3a0a 2020 2020 2222 2247 6976 656e  '):.    """Given
-00027060: 2061 6e20 616e 6e6f 7461 7469 6f6e 7320   an annotations 
-00027070: 7461 626c 6520 7769 7468 2070 6f73 6974  table with posit
-00027080: 696f 6e73 2061 6e64 2064 7572 6174 696f  ions and duratio
-00027090: 6e73 2c20 6372 6561 7465 2061 6e20 3a6f  ns, create an :o
-000270a0: 626a 3a60 7061 6e64 6173 2e49 6e74 6572  bj:`pandas.Inter
-000270b0: 7661 6c49 6e64 6578 602e 0a20 2020 2052  valIndex`..    R
-000270c0: 6574 7572 6e73 204e 6f6e 6520 6966 2061  eturns None if a
-000270d0: 6e79 2072 6f77 2069 7320 756e 6465 7273  ny row is unders
-000270e0: 7065 6369 6669 6564 2e0a 0a20 2020 2050  pecified...    P
-000270f0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00027100: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6620  --------.    df 
-00027110: 3a20 3a6f 626a 3a60 7061 6e64 6173 2e44  : :obj:`pandas.D
-00027120: 6174 6146 7261 6d65 600a 2020 2020 2020  ataFrame`.      
-00027130: 2020 416e 6e6f 7461 7469 6f6e 2074 6162    Annotation tab
-00027140: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
-00027150: 6520 636f 6c75 6d6e 7320 6f66 2060 6070  e columns of ``p
-00027160: 6f73 6974 696f 6e5f 636f 6c60 6020 2864  osition_col`` (d
-00027170: 6566 6175 6c74 3a20 2771 7561 7274 6572  efault: 'quarter
-00027180: 6265 6174 7327 2920 616e 6420 6060 6475  beats') and ``du
-00027190: 7261 7469 6f6e 5f63 6f6c 6060 0a20 2020  ration_col``.   
-000271a0: 2020 2020 2064 6566 6175 6c74 3a20 2764       default: 'd
-000271b0: 7572 6174 696f 6e5f 7162 2729 2e0a 2020  uration_qb')..  
-000271c0: 2020 706f 7369 7469 6f6e 5f63 6f6c 203a    position_col :
-000271d0: 203a 6f62 6a3a 6073 7472 602c 206f 7074   :obj:`str`, opt
-000271e0: 696f 6e61 6c0a 2020 2020 2020 2020 4e61  ional.        Na
-000271f0: 6d65 206f 6620 7468 6520 636f 6c75 6d6e  me of the column
-00027200: 2063 6f6e 7461 696e 696e 6720 706f 7369   containing posi
-00027210: 7469 6f6e 732c 2075 7365 6420 6173 206c  tions, used as l
-00027220: 6566 7420 626f 756e 6461 7269 6573 2e0a  eft boundaries..
-00027230: 2020 2020 6475 7261 7469 6f6e 5f63 6f6c      duration_col
-00027240: 203a 203a 6f62 6a3a 6073 7472 602c 206f   : :obj:`str`, o
-00027250: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00027260: 4e61 6d65 206f 6620 7468 6520 636f 6c75  Name of the colu
-00027270: 6d6e 2063 6f6e 7461 696e 696e 6720 6475  mn containing du
-00027280: 7261 7469 6f6e 7320 7768 6963 6820 7769  rations which wi
-00027290: 6c6c 2062 6520 6164 6465 6420 746f 2074  ll be added to t
-000272a0: 6865 2070 6f73 6974 696f 6e73 2074 6f20  he positions to 
-000272b0: 6f62 7461 696e 2072 6967 6874 2062 6f75  obtain right bou
-000272c0: 6e64 6172 6965 732e 0a20 2020 2063 6c6f  ndaries..    clo
-000272d0: 7365 6420 3a20 3a6f 626a 3a60 7374 7260  sed : :obj:`str`
-000272e0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-000272f0: 2020 2027 6c65 6674 272c 2027 7269 6768     'left', 'righ
-00027300: 7427 206f 7220 2762 6f74 6827 203c 2d20  t' or 'both' <- 
-00027310: 6465 6669 6e69 6e67 2074 6865 2069 6e74  defining the int
-00027320: 6572 7661 6c20 626f 756e 6461 7269 6573  erval boundaries
-00027330: 0a20 2020 2072 6f75 6e64 203a 203a 6f62  .    round : :ob
-00027340: 6a3a 6069 6e74 602c 206f 7074 696f 6e61  j:`int`, optiona
-00027350: 6c0a 2020 2020 2020 2020 546f 2068 6f77  l.        To how
-00027360: 206d 616e 7920 6465 6369 6d61 6c20 706c   many decimal pl
-00027370: 6163 6573 2074 6f20 726f 756e 6420 7468  aces to round th
-00027380: 6520 696e 7465 7276 616c 7327 2062 6f75  e intervals' bou
-00027390: 6e64 6172 7920 7661 6c75 6573 2e0a 2020  ndary values..  
-000273a0: 2020 6e61 6d65 203a 203a 6f62 6a3a 6073    name : :obj:`s
-000273b0: 7472 602c 206f 7074 696f 6e61 6c0a 2020  tr`, optional.  
-000273c0: 2020 2020 2020 4e61 6d65 206f 6620 7468        Name of th
-000273d0: 6520 6372 6561 7465 6420 696e 6465 782e  e created index.
-000273e0: 2044 6566 6175 6c74 7320 746f 2027 696e   Defaults to 'in
-000273f0: 7465 7276 616c 272e 0a0a 2020 2020 5265  terval'...    Re
-00027400: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00027410: 2d0a 2020 2020 3a6f 626a 3a60 7061 6e64  -.    :obj:`pand
-00027420: 6173 2e49 6e74 6572 7661 6c49 6e64 6578  as.IntervalIndex
-00027430: 600a 2020 2020 2020 2020 4120 636f 7079  `.        A copy
-00027440: 206f 6620 6060 6466 6060 2077 6974 6820   of ``df`` with 
-00027450: 7468 6520 6f72 6967 696e 616c 2069 6e64  the original ind
-00027460: 6578 2072 6570 6c61 6365 6420 616e 6420  ex replaced and 
-00027470: 756e 6465 7273 7065 6369 6669 6564 2072  underspecified r
-00027480: 6f77 7320 7265 6d6f 7665 6420 2874 686f  ows removed (tho
-00027490: 7365 2077 6865 7265 206e 6f20 696e 7465  se where no inte
-000274a0: 7276 616c 0a20 2020 2020 2020 2063 6f75  rval.        cou
-000274b0: 6c64 2062 6520 636f 7075 7465 6429 2e0a  ld be coputed)..
-000274c0: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
-000274d0: 6f74 2061 6c6c 2863 2069 6e20 6466 2e63  ot all(c in df.c
-000274e0: 6f6c 756d 6e73 2066 6f72 2063 2069 6e20  olumns for c in 
-000274f0: 2870 6f73 6974 696f 6e5f 636f 6c2c 2064  (position_col, d
-00027500: 7572 6174 696f 6e5f 636f 6c29 293a 0a20  uration_col)):. 
-00027510: 2020 2020 2020 206d 6973 7369 6e67 203d         missing =
-00027520: 205b 6320 666f 7220 6320 696e 2028 706f   [c for c in (po
-00027530: 7369 7469 6f6e 5f63 6f6c 2c20 6475 7261  sition_col, dura
-00027540: 7469 6f6e 5f63 6f6c 2920 6966 2063 206e  tion_col) if c n
-00027550: 6f74 2069 6e20 6466 2e63 6f6c 756d 6e73  ot in df.columns
-00027560: 5d0a 2020 2020 2020 2020 706c 7572 616c  ].        plural
-00027570: 203d 2027 7327 2069 6620 6c65 6e28 6d69   = 's' if len(mi
-00027580: 7373 696e 6729 203e 2031 2065 6c73 6520  ssing) > 1 else 
-00027590: 2727 0a20 2020 2020 2020 206c 6f67 6765  ''.        logge
-000275a0: 722e 7761 726e 696e 6728 6622 436f 6c75  r.warning(f"Colu
-000275b0: 6d6e 7b70 6c75 7261 6c7d 206e 6f74 2070  mn{plural} not p
-000275c0: 7265 7365 6e74 2069 6e20 4461 7461 4672  resent in DataFr
-000275d0: 616d 653a 207b 272c 2027 2e6a 6f69 6e28  ame: {', '.join(
-000275e0: 6d69 7373 696e 6729 7d22 290a 2020 2020  missing)}").    
-000275f0: 2020 2020 7265 7475 726e 0a20 2020 2069      return.    i
-00027600: 6620 6466 5b70 6f73 6974 696f 6e5f 636f  f df[position_co
-00027610: 6c5d 2e69 736e 6128 292e 616e 7928 2920  l].isna().any() 
-00027620: 6f72 2064 665b 6475 7261 7469 6f6e 5f63  or df[duration_c
-00027630: 6f6c 5d2e 6973 6e61 2829 2e61 6e79 2829  ol].isna().any()
-00027640: 3a0a 2020 2020 2020 2020 6d69 7373 696e  :.        missin
-00027650: 6720 3d20 6466 5b64 665b 5b70 6f73 6974  g = df[df[[posit
-00027660: 696f 6e5f 636f 6c2c 2064 7572 6174 696f  ion_col, duratio
-00027670: 6e5f 636f 6c5d 5d2e 6973 6e61 2829 2e61  n_col]].isna().a
-00027680: 6e79 2861 7869 733d 3129 5d0a 2020 2020  ny(axis=1)].    
-00027690: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
-000276a0: 6e67 2866 2243 6f75 6c64 206e 6f74 206d  ng(f"Could not m
-000276b0: 616b 6520 496e 7465 7276 616c 496e 6465  ake IntervalInde
-000276c0: 7820 6265 6361 7573 6520 6f66 206d 6973  x because of mis
-000276d0: 7369 6e67 2076 616c 7565 733a 5c6e 7b6d  sing values:\n{m
-000276e0: 6973 7369 6e67 7d22 290a 2020 2020 2020  issing}").      
-000276f0: 2020 7265 7475 726e 0a20 2020 2074 7279    return.    try
-00027700: 3a0a 2020 2020 2020 2020 6c65 6674 203d  :.        left =
-00027710: 2064 665b 706f 7369 7469 6f6e 5f63 6f6c   df[position_col
-00027720: 5d2e 6173 7479 7065 2866 6c6f 6174 290a  ].astype(float).
-00027730: 2020 2020 2020 2020 7269 6768 7420 3d20          right = 
-00027740: 286c 6566 7420 2b20 6466 5b64 7572 6174  (left + df[durat
-00027750: 696f 6e5f 636f 6c5d 292e 6173 7479 7065  ion_col]).astype
-00027760: 2866 6c6f 6174 290a 2020 2020 2020 2020  (float).        
-00027770: 6966 2072 6f75 6e64 2069 7320 6e6f 7420  if round is not 
-00027780: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027790: 2020 6c65 6674 2c20 7269 6768 7420 3d20    left, right = 
-000277a0: 6c65 6674 2e72 6f75 6e64 2872 6f75 6e64  left.round(round
-000277b0: 292c 2072 6967 6874 2e72 6f75 6e64 2872  ), right.round(r
-000277c0: 6f75 6e64 290a 2020 2020 2020 2020 7265  ound).        re
-000277d0: 7475 726e 2070 642e 496e 7465 7276 616c  turn pd.Interval
-000277e0: 496e 6465 782e 6672 6f6d 5f61 7272 6179  Index.from_array
-000277f0: 7328 6c65 6674 3d6c 6566 742c 2072 6967  s(left=left, rig
-00027800: 6874 3d72 6967 6874 2c20 636c 6f73 6564  ht=right, closed
-00027810: 3d63 6c6f 7365 642c 206e 616d 653d 6e61  =closed, name=na
-00027820: 6d65 290a 2020 2020 6578 6365 7074 2045  me).    except E
-00027830: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
-00027840: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-00027850: 726e 696e 6728 6622 4372 6561 7469 6e67  rning(f"Creating
-00027860: 2049 6e74 6572 7661 6c49 6e64 6578 2066   IntervalIndex f
-00027870: 6169 6c65 6420 7769 7468 2065 7863 6570  ailed with excep
-00027880: 7469 6f6e 207b 657d 2e22 290a 0a40 6675  tion {e}.")..@fu
-00027890: 6e63 7469 6f6e 5f6c 6f67 6765 720a 6465  nction_logger.de
-000278a0: 6620 7265 706c 6163 655f 696e 6465 785f  f replace_index_
-000278b0: 6279 5f69 6e74 6572 7661 6c73 2864 662c  by_intervals(df,
-000278c0: 2070 6f73 6974 696f 6e5f 636f 6c3d 2771   position_col='q
-000278d0: 7561 7274 6572 6265 6174 7327 2c20 6475  uarterbeats', du
-000278e0: 7261 7469 6f6e 5f63 6f6c 3d27 6475 7261  ration_col='dura
-000278f0: 7469 6f6e 5f71 6227 2c20 636c 6f73 6564  tion_qb', closed
-00027900: 3d27 6c65 6674 272c 0a20 2020 2020 2020  ='left',.       
-00027910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027920: 2020 2020 2020 2020 6669 6c74 6572 5f7a          filter_z
-00027930: 6572 6f5f 6475 7261 7469 6f6e 3d46 616c  ero_duration=Fal
-00027940: 7365 2c20 726f 756e 643d 4e6f 6e65 2c20  se, round=None, 
-00027950: 6e61 6d65 3d27 696e 7465 7276 616c 2729  name='interval')
-00027960: 3a0a 2020 2020 2222 2247 6976 656e 2061  :.    """Given a
-00027970: 6e20 616e 6e6f 7461 7469 6f6e 7320 7461  n annotations ta
-00027980: 626c 6520 7769 7468 2070 6f73 6974 696f  ble with positio
-00027990: 6e73 2061 6e64 2064 7572 6174 696f 6e73  ns and durations
-000279a0: 2c20 7265 706c 6163 6573 2069 7473 2069  , replaces its i
-000279b0: 6e64 6578 2077 6974 6820 616e 203a 6f62  ndex with an :ob
-000279c0: 6a3a 6070 616e 6461 732e 496e 7465 7276  j:`pandas.Interv
-000279d0: 616c 496e 6465 7860 2e0a 2020 2020 556e  alIndex`..    Un
-000279e0: 6465 7273 7065 6369 6669 6564 2072 6f77  derspecified row
-000279f0: 7320 6172 6520 7265 6d6f 7665 642e 0a0a  s are removed...
-00027a00: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00027a10: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00027a20: 2020 6466 203a 203a 6f62 6a3a 6070 616e    df : :obj:`pan
-00027a30: 6461 732e 4461 7461 4672 616d 6560 0a20  das.DataFrame`. 
-00027a40: 2020 2020 2020 2041 6e6e 6f74 6174 696f         Annotatio
-00027a50: 6e20 7461 626c 6520 636f 6e74 6169 6e69  n table containi
-00027a60: 6e67 2074 6865 2063 6f6c 756d 6e73 206f  ng the columns o
-00027a70: 6620 6060 706f 7369 7469 6f6e 5f63 6f6c  f ``position_col
-00027a80: 6060 2028 6465 6661 756c 743a 2027 7175  `` (default: 'qu
-00027a90: 6172 7465 7262 6561 7473 2729 2061 6e64  arterbeats') and
-00027aa0: 2060 6064 7572 6174 696f 6e5f 636f 6c60   ``duration_col`
-00027ab0: 600a 2020 2020 2020 2020 6465 6661 756c  `.        defaul
-00027ac0: 743a 2027 6475 7261 7469 6f6e 5f71 6227  t: 'duration_qb'
-00027ad0: 292e 0a20 2020 2070 6f73 6974 696f 6e5f  )..    position_
-00027ae0: 636f 6c20 3a20 3a6f 626a 3a60 7374 7260  col : :obj:`str`
-00027af0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00027b00: 2020 204e 616d 6520 6f66 2074 6865 2063     Name of the c
-00027b10: 6f6c 756d 6e20 636f 6e74 6169 6e69 6e67  olumn containing
-00027b20: 2070 6f73 6974 696f 6e73 2e0a 2020 2020   positions..    
-00027b30: 6475 7261 7469 6f6e 5f63 6f6c 203a 203a  duration_col : :
-00027b40: 6f62 6a3a 6073 7472 602c 206f 7074 696f  obj:`str`, optio
-00027b50: 6e61 6c0a 2020 2020 2020 2020 4e61 6d65  nal.        Name
-00027b60: 206f 6620 7468 6520 636f 6c75 6d6e 2063   of the column c
-00027b70: 6f6e 7461 696e 696e 6720 6475 7261 7469  ontaining durati
-00027b80: 6f6e 732e 0a20 2020 2063 6c6f 7365 6420  ons..    closed 
-00027b90: 3a20 3a6f 626a 3a60 7374 7260 2c20 6f70  : :obj:`str`, op
-00027ba0: 7469 6f6e 616c 0a20 2020 2020 2020 2027  tional.        '
-00027bb0: 6c65 6674 272c 2027 7269 6768 7427 206f  left', 'right' o
-00027bc0: 7220 2762 6f74 6827 203c 2d20 6465 6669  r 'both' <- defi
-00027bd0: 6e69 6e67 2074 6865 2069 6e74 6572 7661  ning the interva
-00027be0: 6c20 626f 756e 6461 7269 6573 0a20 2020  l boundaries.   
-00027bf0: 2066 696c 7465 725f 7a65 726f 5f64 7572   filter_zero_dur
-00027c00: 6174 696f 6e20 3a20 3a6f 626a 3a60 626f  ation : :obj:`bo
-00027c10: 6f6c 602c 206f 7074 696f 6e61 6c0a 2020  ol`, optional.  
-00027c20: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00027c30: 6f20 4661 6c73 652c 206d 6561 6e69 6e67  o False, meaning
-00027c40: 2074 6861 7420 726f 7773 2077 6974 6820   that rows with 
-00027c50: 7a65 726f 2064 7572 6174 696f 6e73 2061  zero durations a
-00027c60: 7265 206d 6169 6e74 6169 6e65 642e 2050  re maintained. P
-00027c70: 6173 7320 5472 7565 2074 6f20 7265 6d6f  ass True to remo
-00027c80: 7665 2074 6865 6d2e 0a20 2020 2072 6f75  ve them..    rou
-00027c90: 6e64 203a 203a 6f62 6a3a 6069 6e74 602c  nd : :obj:`int`,
-00027ca0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00027cb0: 2020 546f 2068 6f77 206d 616e 7920 6465    To how many de
-00027cc0: 6369 6d61 6c20 706c 6163 6573 2074 6f20  cimal places to 
-00027cd0: 726f 756e 6420 7468 6520 696e 7465 7276  round the interv
-00027ce0: 616c 7327 2062 6f75 6e64 6172 7920 7661  als' boundary va
-00027cf0: 6c75 6573 2e0a 2020 2020 6e61 6d65 203a  lues..    name :
-00027d00: 203a 6f62 6a3a 6073 7472 602c 206f 7074   :obj:`str`, opt
-00027d10: 696f 6e61 6c0a 2020 2020 2020 2020 4e61  ional.        Na
-00027d20: 6d65 206f 6620 7468 6520 6372 6561 7465  me of the create
-00027d30: 6420 696e 6465 782e 2044 6566 6175 6c74  d index. Default
-00027d40: 7320 746f 2027 696e 7465 7276 616c 272e  s to 'interval'.
-00027d50: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00027d60: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 3a6f    -------.    :o
-00027d70: 626a 3a60 7061 6e64 6173 2e44 6174 6146  bj:`pandas.DataF
-00027d80: 7261 6d65 600a 2020 2020 2020 2020 4120  rame`.        A 
-00027d90: 636f 7079 206f 6620 6060 6466 6060 2077  copy of ``df`` w
-00027da0: 6974 6820 7468 6520 6f72 6967 696e 616c  ith the original
-00027db0: 2069 6e64 6578 2072 6570 6c61 6365 6420   index replaced 
-00027dc0: 616e 6420 756e 6465 7273 7065 6369 6669  and underspecifi
-00027dd0: 6564 2072 6f77 7320 7265 6d6f 7665 6420  ed rows removed 
-00027de0: 2874 686f 7365 2077 6865 7265 206e 6f20  (those where no 
-00027df0: 696e 7465 7276 616c 0a20 2020 2020 2020  interval.       
-00027e00: 2063 6f75 6c64 2062 6520 636f 6d70 7574   could be comput
-00027e10: 6564 292e 0a20 2020 2022 2222 0a20 2020  ed)..    """.   
-00027e20: 2069 6620 6e6f 7420 616c 6c28 6320 696e   if not all(c in
-00027e30: 2064 662e 636f 6c75 6d6e 7320 666f 7220   df.columns for 
-00027e40: 6320 696e 2028 706f 7369 7469 6f6e 5f63  c in (position_c
-00027e50: 6f6c 2c20 6475 7261 7469 6f6e 5f63 6f6c  ol, duration_col
-00027e60: 2929 3a0a 2020 2020 2020 2020 6d69 7373  )):.        miss
-00027e70: 696e 6720 3d20 5b63 2066 6f72 2063 2069  ing = [c for c i
-00027e80: 6e20 2870 6f73 6974 696f 6e5f 636f 6c2c  n (position_col,
-00027e90: 2064 7572 6174 696f 6e5f 636f 6c29 2069   duration_col) i
-00027ea0: 6620 6320 6e6f 7420 696e 2064 662e 636f  f c not in df.co
-00027eb0: 6c75 6d6e 735d 0a20 2020 2020 2020 2070  lumns].        p
-00027ec0: 6c75 7261 6c20 3d20 2773 2720 6966 206c  lural = 's' if l
-00027ed0: 656e 286d 6973 7369 6e67 2920 3e20 3120  en(missing) > 1 
-00027ee0: 656c 7365 2027 270a 2020 2020 2020 2020  else ''.        
-00027ef0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2866  logger.warning(f
-00027f00: 2243 6f6c 756d 6e7b 706c 7572 616c 7d20  "Column{plural} 
-00027f10: 6e6f 7420 7072 6573 656e 7420 696e 2044  not present in D
-00027f20: 6174 6146 7261 6d65 3a20 7b27 2c20 272e  ataFrame: {', '.
-00027f30: 6a6f 696e 286d 6973 7369 6e67 297d 2229  join(missing)}")
-00027f40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00027f50: 6466 0a20 2020 206d 6173 6b20 3d20 6466  df.    mask = df
-00027f60: 5b70 6f73 6974 696f 6e5f 636f 6c5d 2e6e  [position_col].n
-00027f70: 6f74 6e61 2829 2026 2028 6466 5b70 6f73  otna() & (df[pos
-00027f80: 6974 696f 6e5f 636f 6c5d 2021 3d20 2727  ition_col] != ''
-00027f90: 2920 2620 6466 5b64 7572 6174 696f 6e5f  ) & df[duration_
-00027fa0: 636f 6c5d 2e6e 6f74 6e61 2829 0a20 2020  col].notna().   
-00027fb0: 206e 5f64 726f 7070 6564 203d 2028 7e6d   n_dropped = (~m
-00027fc0: 6173 6b29 2e73 756d 2829 0a20 2020 2069  ask).sum().    i
-00027fd0: 6620 6669 6c74 6572 5f7a 6572 6f5f 6475  f filter_zero_du
-00027fe0: 7261 7469 6f6e 3a0a 2020 2020 2020 2020  ration:.        
-00027ff0: 6d61 736b 2026 3d20 2864 665b 6475 7261  mask &= (df[dura
-00028000: 7469 6f6e 5f63 6f6c 5d20 3e20 3029 0a20  tion_col] > 0). 
-00028010: 2020 2065 6c69 6620 6e5f 6472 6f70 7065     elif n_droppe
-00028020: 6420 3e20 303a 0a20 2020 2020 2020 206c  d > 0:.        l
-00028030: 6f67 6765 722e 696e 666f 2866 2248 6164  ogger.info(f"Had
-00028040: 2074 6f20 6472 6f70 207b 6e5f 6472 6f70   to drop {n_drop
-00028050: 7065 647d 2072 6f77 7320 666f 7220 6372  ped} rows for cr
-00028060: 6561 7469 6e67 2074 6865 2049 6e74 6572  eating the Inter
-00028070: 7661 6c49 6e64 6578 3a5c 6e7b 6466 5b7e  valIndex:\n{df[~
-00028080: 6d61 736b 5d7d 2229 0a20 2020 2064 6620  mask]}").    df 
-00028090: 3d20 6466 5b6d 6173 6b5d 2e63 6f70 7928  = df[mask].copy(
-000280a0: 290a 2020 2020 6976 5f69 6e64 6578 203d  ).    iv_index =
-000280b0: 206d 616b 655f 696e 7465 7276 616c 5f69   make_interval_i
-000280c0: 6e64 6578 5f66 726f 6d5f 6475 7261 7469  ndex_from_durati
-000280d0: 6f6e 7328 6466 2c20 706f 7369 7469 6f6e  ons(df, position
-000280e0: 5f63 6f6c 3d70 6f73 6974 696f 6e5f 636f  _col=position_co
-000280f0: 6c2c 2064 7572 6174 696f 6e5f 636f 6c3d  l, duration_col=
-00028100: 6475 7261 7469 6f6e 5f63 6f6c 2c0a 2020  duration_col,.  
-00028110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028120: 2020 636c 6f73 6564 3d63 6c6f 7365 642c    closed=closed,
-00028130: 2072 6f75 6e64 3d72 6f75 6e64 2c20 6e61   round=round, na
-00028140: 6d65 3d6e 616d 652c 206c 6f67 6765 723d  me=name, logger=
-00028150: 6c6f 6767 6572 290a 2020 2020 6966 2064  logger).    if d
-00028160: 665b 6475 7261 7469 6f6e 5f63 6f6c 5d2e  f[duration_col].
-00028170: 6474 7970 6520 213d 2066 6c6f 6174 3a0a  dtype != float:.
-00028180: 2020 2020 2020 2020 7769 7468 2077 6172          with war
-00028190: 6e69 6e67 732e 6361 7463 685f 7761 726e  nings.catch_warn
-000281a0: 696e 6773 2829 3a0a 2020 2020 2020 2020  ings():.        
-000281b0: 2020 2020 2320 5365 7474 696e 6720 7661      # Setting va
-000281c0: 6c75 6573 2069 6e2d 706c 6163 6520 6973  lues in-place is
-000281d0: 2066 696e 652c 2069 676e 6f72 6520 7468   fine, ignore th
-000281e0: 6520 7761 726e 696e 6720 696e 2050 616e  e warning in Pan
-000281f0: 6461 7320 3e3d 2031 2e35 2e30 0a20 2020  das >= 1.5.0.   
-00028200: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-00028210: 6361 6e20 6265 2072 656d 6f76 6564 2c20  can be removed, 
-00028220: 6966 2050 616e 6461 7320 312e 352e 3020  if Pandas 1.5.0 
-00028230: 646f 6573 206e 6f74 206e 6565 6420 746f  does not need to
-00028240: 2062 6520 7375 7070 6f72 7465 6420 616e   be supported an
-00028250: 7920 6c6f 6e67 6572 2e0a 2020 2020 2020  y longer..      
-00028260: 2020 2020 2020 2320 5365 6520 616c 736f        # See also
-00028270: 3a20 6874 7470 733a 2f2f 7374 6163 6b6f  : https://stacko
-00028280: 7665 7266 6c6f 772e 636f 6d2f 712f 3734  verflow.com/q/74
-00028290: 3035 3733 3637 2f38 3539 3539 310a 2020  057367/859591.  
-000282a0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-000282b0: 6773 2e66 696c 7465 7277 6172 6e69 6e67  gs.filterwarning
-000282c0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-000282d0: 2020 2022 6967 6e6f 7265 222c 0a20 2020     "ignore",.   
-000282e0: 2020 2020 2020 2020 2020 2020 2063 6174               cat
-000282f0: 6567 6f72 793d 4675 7475 7265 5761 726e  egory=FutureWarn
-00028300: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-00028310: 2020 2020 206d 6573 7361 6765 3d28 0a20       message=(. 
-00028320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028330: 2020 2022 2e2a 7769 6c6c 2061 7474 656d     ".*will attem
-00028340: 7074 2074 6f20 7365 7420 7468 6520 7661  pt to set the va
-00028350: 6c75 6573 2069 6e70 6c61 6365 2069 6e73  lues inplace ins
-00028360: 7465 6164 206f 6620 616c 7761 7973 2073  tead of always s
-00028370: 6574 7469 6e67 2061 206e 6577 2061 7272  etting a new arr
-00028380: 6179 2e20 220a 2020 2020 2020 2020 2020  ay. ".          
-00028390: 2020 2020 2020 2020 2020 2254 6f20 7265            "To re
-000283a0: 7461 696e 2074 6865 206f 6c64 2062 6568  tain the old beh
-000283b0: 6176 696f 722c 2075 7365 2065 6974 6865  avior, use eithe
-000283c0: 722e 2a22 0a20 2020 2020 2020 2020 2020  r.*".           
-000283d0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-000283e0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000283f0: 2020 6466 2e6c 6f63 5b3a 2c20 6475 7261    df.loc[:, dura
-00028400: 7469 6f6e 5f63 6f6c 5d20 3d20 7064 2e74  tion_col] = pd.t
-00028410: 6f5f 6e75 6d65 7269 6328 6466 5b64 7572  o_numeric(df[dur
-00028420: 6174 696f 6e5f 636f 6c5d 290a 2020 2020  ation_col]).    
-00028430: 6966 2069 765f 696e 6465 7820 6973 204e  if iv_index is N
-00028440: 6f6e 653a 0a20 2020 2020 2020 206c 6f67  one:.        log
-00028450: 6765 722e 7761 726e 696e 6728 2243 7265  ger.warning("Cre
-00028460: 6174 696e 6720 496e 7465 7276 616c 496e  ating IntervalIn
-00028470: 6465 7820 6661 696c 6564 2e22 290a 2020  dex failed.").  
-00028480: 2020 2020 2020 7265 7475 726e 2064 660a        return df.
-00028490: 2020 2020 6466 2e69 6e64 6578 203d 2069      df.index = i
-000284a0: 765f 696e 6465 780a 2020 2020 7265 7475  v_index.    retu
-000284b0: 726e 2064 660a 0a64 6566 2062 6f6f 6c65  rn df..def boole
-000284c0: 616e 5f6d 6f64 655f 636f 6c32 7374 7269  an_mode_col2stri
-000284d0: 6e67 7328 5329 202d 3e20 7064 2e53 6572  ngs(S) -> pd.Ser
-000284e0: 6965 733a 0a20 2020 2022 2222 5475 726e  ies:.    """Turn
-000284f0: 2074 6865 2062 6f6f 6c65 616e 2069 735f   the boolean is_
-00028500: 6d69 6e6f 7220 636f 6c75 6d6e 7320 696e  minor columns in
-00028510: 746f 2073 7472 696e 6720 636f 6c75 6d6e  to string column
-00028520: 7320 7375 6368 2074 6861 7420 5472 7565  s such that True
-00028530: 203d 3e20 276d 696e 6f72 272c 2046 616c   => 'minor', Fal
-00028540: 7365 203d 3e20 276d 616a 6f72 272e 2222  se => 'major'.""
-00028550: 220a 2020 2020 7265 7475 726e 2053 2e6d  ".    return S.m
-00028560: 6170 287b 5472 7565 3a20 276d 696e 6f72  ap({True: 'minor
-00028570: 272c 2046 616c 7365 3a20 276d 616a 6f72  ', False: 'major
-00028580: 277d 290a 0a64 6566 2072 6570 6c61 6365  '})..def replace
-00028590: 5f62 6f6f 6c65 616e 5f6d 6f64 655f 6279  _boolean_mode_by
-000285a0: 5f73 7472 696e 6773 2864 6629 202d 3e20  _strings(df) -> 
-000285b0: 7064 2e44 6174 6146 7261 6d65 3a0a 2020  pd.DataFrame:.  
-000285c0: 2020 2222 2252 6570 6c61 6365 7320 626f    """Replaces bo
-000285d0: 6f6c 6561 6e20 275f 6973 5f6d 696e 6f72  olean '_is_minor
-000285e0: 2720 636f 6c75 6d6e 7320 7769 7468 2073  ' columns with s
-000285f0: 7472 696e 6720 636f 6c75 6d6e 7320 7265  tring columns re
-00028600: 6e61 6d65 6420 746f 2027 5f6d 6f64 6527  named to '_mode'
-00028610: 2e0a 2020 2020 4578 616d 706c 653a 2064  ..    Example: d
-00028620: 665b 2773 6f6d 655f 636f 6c27 2c20 2773  f['some_col', 's
-00028630: 6f6d 655f 6e61 6d65 5f69 735f 6d69 6e6f  ome_name_is_mino
-00028640: 7227 5d20 3d3e 2064 665b 2773 6f6d 655f  r'] => df['some_
-00028650: 636f 6c27 2c20 2773 6f6d 655f 6e61 6d65  col', 'some_name
-00028660: 5f6d 6f64 6527 5d0a 2020 2020 2222 220a  _mode'].    """.
-00028670: 2020 2020 626f 6f6c 5f63 6f6c 7320 3d20      bool_cols = 
-00028680: 5b63 6f6c 2066 6f72 2063 6f6c 2069 6e20  [col for col in 
-00028690: 6466 2e63 6f6c 756d 6e73 2069 6620 636f  df.columns if co
-000286a0: 6c2e 656e 6473 7769 7468 2827 5f69 735f  l.endswith('_is_
-000286b0: 6d69 6e6f 7227 295d 0a20 2020 2069 6620  minor')].    if 
-000286c0: 6c65 6e28 626f 6f6c 5f63 6f6c 7329 203d  len(bool_cols) =
-000286d0: 3d20 303a 0a20 2020 2020 2020 2072 6574  = 0:.        ret
-000286e0: 7572 6e20 6466 0a20 2020 2064 6620 3d20  urn df.    df = 
-000286f0: 6466 2e63 6f70 7928 290a 2020 2020 7265  df.copy().    re
-00028700: 6e61 6d69 6e67 203d 207b 7d0a 2020 2020  naming = {}.    
-00028710: 666f 7220 636f 6c5f 6e61 6d65 2069 6e20  for col_name in 
-00028720: 626f 6f6c 5f63 6f6c 733a 0a20 2020 2020  bool_cols:.     
-00028730: 2020 206e 756d 6572 616c 5f6e 616d 6520     numeral_name 
-00028740: 3d20 636f 6c5f 6e61 6d65 5b3a 2d6c 656e  = col_name[:-len
-00028750: 2827 5f69 735f 6d69 6e6f 7227 295d 0a20  ('_is_minor')]. 
-00028760: 2020 2020 2020 2069 6620 636f 6c5f 6e61         if col_na
-00028770: 6d65 2069 6e20 6466 2e63 6f6c 756d 6e73  me in df.columns
-00028780: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-00028790: 775f 636f 6c5f 6e61 6d65 203d 2066 227b  w_col_name = f"{
-000287a0: 6e75 6d65 7261 6c5f 6e61 6d65 7d5f 6d6f  numeral_name}_mo
-000287b0: 6465 220a 2020 2020 2020 2020 2020 2020  de".            
-000287c0: 6e65 775f 636f 6c20 3d20 626f 6f6c 6561  new_col = boolea
-000287d0: 6e5f 6d6f 6465 5f63 6f6c 3273 7472 696e  n_mode_col2strin
-000287e0: 6773 2864 665b 636f 6c5f 6e61 6d65 5d29  gs(df[col_name])
-000287f0: 0a20 2020 2020 2020 2020 2020 2064 662e  .            df.
-00028800: 6c6f 635b 3a2c 636f 6c5f 6e61 6d65 5d20  loc[:,col_name] 
-00028810: 3d20 6e65 775f 636f 6c0a 2020 2020 2020  = new_col.      
-00028820: 2020 2020 2020 7265 6e61 6d69 6e67 5b63        renaming[c
-00028830: 6f6c 5f6e 616d 655d 203d 206e 6577 5f63  ol_name] = new_c
-00028840: 6f6c 5f6e 616d 650a 2020 2020 6466 2e72  ol_name.    df.r
-00028850: 656e 616d 6528 636f 6c75 6d6e 733d 7265  ename(columns=re
-00028860: 6e61 6d69 6e67 2c20 696e 706c 6163 653d  naming, inplace=
-00028870: 5472 7565 290a 2020 2020 7265 7475 726e  True).    return
-00028880: 2064 660a 0a40 6675 6e63 7469 6f6e 5f6c   df..@function_l
-00028890: 6f67 6765 720a 6465 6620 7265 736f 6c76  ogger.def resolv
-000288a0: 655f 7265 6c61 7469 7665 5f6b 6579 7328  e_relative_keys(
-000288b0: 7265 6c61 7469 7665 726f 6f74 2c20 6d69  relativeroot, mi
-000288c0: 6e6f 723d 4661 6c73 6529 3a0a 2020 2020  nor=False):.    
-000288d0: 2222 2220 5265 736f 6c76 6520 6e65 7374  """ Resolve nest
-000288e0: 6564 2072 656c 6174 6976 6520 6b65 7973  ed relative keys
-000288f0: 2c20 652e 672e 2027 562f 562f 5627 203d  , e.g. 'V/V/V' =
-00028900: 3e20 2756 4927 2e0a 0a20 2020 2055 7365  > 'VI'...    Use
-00028910: 733a 203a 7079 3a66 756e 633a 6072 656c  s: :py:func:`rel
-00028920: 3261 6273 5f6b 6579 602c 203a 7079 3a66  2abs_key`, :py:f
-00028930: 756e 633a 6073 7472 5f69 735f 6d69 6e6f  unc:`str_is_mino
-00028940: 7260 0a0a 2020 2020 7265 6c61 7469 7665  r`..    relative
-00028950: 726f 6f74 203a 203a 6f62 6a3a 6073 7472  root : :obj:`str
-00028960: 600a 2020 2020 2020 2020 4f6e 6520 6f72  `.        One or
-00028970: 2073 6576 6572 616c 2072 656c 6174 6976   several relativ
-00028980: 6520 6b65 7973 2c20 652e 672e 2069 762f  e keys, e.g. iv/
-00028990: 762f 5649 2028 666f 7572 7468 2073 6361  v/VI (fourth sca
-000289a0: 6c65 2064 6567 7265 6520 6f66 2074 6865  le degree of the
-000289b0: 2066 6966 7468 2073 6361 6c65 2064 6567   fifth scale deg
-000289c0: 7265 6520 6f66 2074 6865 2073 6978 7468  ree of the sixth
-000289d0: 2073 6361 6c65 2064 6567 7265 6529 0a20   scale degree). 
-000289e0: 2020 206d 696e 6f72 203a 203a 6f62 6a3a     minor : :obj:
-000289f0: 6062 6f6f 6c60 2c20 6f70 7469 6f6e 616c  `bool`, optional
-00028a00: 0a20 2020 2020 2020 2050 6173 7320 5472  .        Pass Tr
-00028a10: 7565 2069 6620 7468 6520 6c61 7374 206f  ue if the last o
-00028a20: 6620 7468 6520 7265 6c61 7469 7665 206b  f the relative k
-00028a30: 6579 7320 6973 2074 6f20 6265 2069 6e74  eys is to be int
-00028a40: 6572 7072 6574 6564 2077 6974 6869 6e20  erpreted within 
-00028a50: 6120 6d69 6e6f 7220 636f 6e74 6578 742e  a minor context.
-00028a60: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-00028a70: 7064 2e69 736e 756c 6c28 7265 6c61 7469  pd.isnull(relati
-00028a80: 7665 726f 6f74 293a 0a20 2020 2020 2020  veroot):.       
-00028a90: 2072 6574 7572 6e20 7265 6c61 7469 7665   return relative
-00028aa0: 726f 6f74 0a20 2020 2073 706c 203d 2072  root.    spl = r
-00028ab0: 656c 6174 6976 6572 6f6f 742e 7370 6c69  elativeroot.spli
-00028ac0: 7428 272f 2729 0a20 2020 2069 6620 6c65  t('/').    if le
-00028ad0: 6e28 7370 6c29 203c 2032 3a0a 2020 2020  n(spl) < 2:.    
-00028ae0: 2020 2020 7265 7475 726e 2072 656c 6174      return relat
-00028af0: 6976 6572 6f6f 740a 2020 2020 6966 206c  iveroot.    if l
-00028b00: 656e 2873 706c 2920 3d3d 2032 3a0a 2020  en(spl) == 2:.  
-00028b10: 2020 2020 2020 6170 706c 6965 642c 2074        applied, t
-00028b20: 6f20 3d20 7370 6c0a 2020 2020 2020 2020  o = spl.        
-00028b30: 7265 7475 726e 2072 656c 3261 6273 5f6b  return rel2abs_k
-00028b40: 6579 2861 7070 6c69 6564 2c20 746f 2c20  ey(applied, to, 
-00028b50: 6d69 6e6f 722c 206c 6f67 6765 723d 6c6f  minor, logger=lo
-00028b60: 6767 6572 290a 2020 2020 7072 6576 696f  gger).    previo
-00028b70: 7573 2c20 6c61 7374 203d 2027 2f27 2e6a  us, last = '/'.j
-00028b80: 6f69 6e28 7370 6c5b 3a2d 315d 292c 2073  oin(spl[:-1]), s
-00028b90: 706c 5b2d 315d 0a20 2020 2072 6574 7572  pl[-1].    retur
-00028ba0: 6e20 7265 6c32 6162 735f 6b65 7928 7265  n rel2abs_key(re
-00028bb0: 736f 6c76 655f 7265 6c61 7469 7665 5f6b  solve_relative_k
-00028bc0: 6579 7328 7072 6576 696f 7573 2c20 7374  eys(previous, st
-00028bd0: 725f 6973 5f6d 696e 6f72 286c 6173 742c  r_is_minor(last,
-00028be0: 2069 735f 6e61 6d65 3d46 616c 7365 2929   is_name=False))
-00028bf0: 2c20 6c61 7374 2c20 6d69 6e6f 7229 0a0a  , last, minor)..
-00028c00: 0a64 6566 2073 6572 6965 735f 6973 5f6d  .def series_is_m
-00028c10: 696e 6f72 2853 2c20 6973 5f6e 616d 653d  inor(S, is_name=
-00028c20: 5472 7565 293a 0a20 2020 2022 2222 2052  True):.    """ R
-00028c30: 6574 7572 6e73 2062 6f6f 6c65 616e 2053  eturns boolean S
-00028c40: 6572 6965 7320 7768 6572 6520 6576 6572  eries where ever
-00028c50: 7920 7661 6c75 6520 696e 2060 6053 6060  y value in ``S``
-00028c60: 2072 6570 7265 7365 6e74 696e 6720 6120   representing a 
-00028c70: 6d69 6e6f 7220 6b65 792f 6368 6f72 6420  minor key/chord 
-00028c80: 6973 2054 7275 652e 2222 220a 2020 2020  is True.""".    
-00028c90: 2320 7265 6765 7820 3d20 7227 285b 412d  # regex = r'([A-
-00028ca0: 4761 2d67 5d29 5b23 7c62 5d2a 2720 6966  Ga-g])[#|b]*' if
-00028cb0: 2069 735f 6e61 6d65 2065 6c73 6520 275b   is_name else '[
-00028cc0: 237c 625d 2a28 5c77 2b29 270a 2020 2020  #|b]*(\w+)'.    
-00028cd0: 2320 7265 7475 726e 2053 2e73 7472 2e72  # return S.str.r
-00028ce0: 6570 6c61 6365 2872 6567 6578 2c20 6c61  eplace(regex, la
-00028cf0: 6d62 6461 206d 3a20 6d2e 6772 6f75 7028  mbda m: m.group(
-00028d00: 3129 292e 7374 722e 6973 6c6f 7765 7228  1)).str.islower(
-00028d10: 290a 2020 2020 7265 7475 726e 2053 2e73  ).    return S.s
-00028d20: 7472 2e69 736c 6f77 6572 2829 2020 2320  tr.islower()  # 
-00028d30: 6173 2073 6f6f 6e20 6173 206f 6e65 2063  as soon as one c
-00028d40: 6861 7261 6374 6572 2069 7320 6e6f 7420  haracter is not 
-00028d50: 6c6f 7765 7263 6173 652c 2069 7420 7368  lowercase, it sh
-00028d60: 6f75 6c64 2062 6520 6d61 6a6f 720a 0a0a  ould be major...
-00028d70: 6465 6620 7374 725f 6973 5f6d 696e 6f72  def str_is_minor
-00028d80: 2874 6f6e 652c 2069 735f 6e61 6d65 3d54  (tone, is_name=T
-00028d90: 7275 6529 3a0a 2020 2020 2222 2220 5265  rue):.    """ Re
-00028da0: 7475 726e 7320 5472 7565 2069 6620 6060  turns True if ``
-00028db0: 746f 6e65 6060 2072 6570 7265 7365 6e74  tone`` represent
-00028dc0: 7320 6120 6d69 6e6f 7220 6b65 7920 6f72  s a minor key or
-00028dd0: 2063 686f 7264 2e22 2222 0a20 2020 2023   chord.""".    #
-00028de0: 2072 6567 6578 203d 2072 2728 5b41 2d47   regex = r'([A-G
-00028df0: 612d 675d 295b 237c 625d 2a27 2069 6620  a-g])[#|b]*' if 
-00028e00: 6973 5f6e 616d 6520 656c 7365 2027 5b23  is_name else '[#
-00028e10: 7c62 5d2a 285c 772b 2927 0a20 2020 2023  |b]*(\w+)'.    #
-00028e20: 206d 203d 2072 652e 6d61 7463 6828 7265   m = re.match(re
-00028e30: 6765 782c 2074 6f6e 6529 0a20 2020 2023  gex, tone).    #
-00028e40: 2069 6620 6d20 6973 204e 6f6e 653a 0a20   if m is None:. 
-00028e50: 2020 2023 2020 2020 2072 6574 7572 6e20     #     return 
-00028e60: 6d0a 2020 2020 2320 7265 7475 726e 206d  m.    # return m
-00028e70: 2e67 726f 7570 2831 292e 6973 6c6f 7765  .group(1).islowe
-00028e80: 7228 290a 2020 2020 7265 7475 726e 2074  r().    return t
-00028e90: 6f6e 652e 6973 6c6f 7765 7228 290a 0a0a  one.islower()...
-00028ea0: 4066 756e 6374 696f 6e5f 6c6f 6767 6572  @function_logger
-00028eb0: 0a64 6566 2074 7261 6e73 706f 7365 5f63  .def transpose_c
-00028ec0: 6861 6e67 6573 2863 6861 6e67 6573 2c20  hanges(changes, 
-00028ed0: 6f6c 645f 6e75 6d2c 206e 6577 5f6e 756d  old_num, new_num
-00028ee0: 2c20 6f6c 645f 6d69 6e6f 723d 4661 6c73  , old_minor=Fals
-00028ef0: 652c 206e 6577 5f6d 696e 6f72 3d46 616c  e, new_minor=Fal
-00028f00: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
-00028f10: 2053 696e 6365 2074 6865 2069 6e74 6572   Since the inter
-00028f20: 7661 6c20 7369 7a65 7320 6578 7072 6573  val sizes expres
-00028f30: 7365 6420 6279 2074 6865 2063 6861 6e67  sed by the chang
-00028f40: 6573 206f 6620 7468 6520 4443 4d4c 2068  es of the DCML h
-00028f50: 6172 6d6f 6e79 2073 796e 7461 780a 2020  armony syntax.  
-00028f60: 2020 6465 7065 6e64 206f 6e20 7468 6520    depend on the 
-00028f70: 6e75 6d65 7261 6c27 7320 706f 7369 7469  numeral's positi
-00028f80: 6f6e 2069 6e20 7468 6520 7363 616c 652c  on in the scale,
-00028f90: 2074 6865 7365 206d 6179 2063 6861 6e67   these may chang
-00028fa0: 6520 6966 2074 6865 206e 756d 6572 616c  e if the numeral
-00028fb0: 0a20 2020 2069 7320 7472 616e 7370 6f73  .    is transpos
-00028fc0: 6564 2e20 5468 6973 2066 756e 6374 696f  ed. This functio
-00028fd0: 6e20 6578 7072 6573 7365 7320 7468 6520  n expresses the 
-00028fe0: 7361 6d65 2063 6861 6e67 6573 2066 6f72  same changes for
-00028ff0: 2074 6865 206e 6577 2070 6f73 6974 696f   the new positio
-00029000: 6e2e 0a20 2020 2043 686f 7264 2074 6f6e  n..    Chord ton
-00029010: 6520 616c 7465 7261 7469 6f6e 7320 286f  e alterations (o
-00029020: 6620 3320 616e 6420 3529 2073 7461 7920  f 3 and 5) stay 
-00029030: 756e 746f 7563 6865 642e 0a0a 2020 2020  untouched...    
-00029040: 5573 6573 3a20 3a70 793a 6675 6e63 3a60  Uses: :py:func:`
-00029050: 6368 616e 6765 7332 7470 6360 0a0a 2020  changes2tpc`..  
-00029060: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00029070: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00029080: 6368 616e 6765 7320 3a20 3a6f 626a 3a60  changes : :obj:`
-00029090: 7374 7260 0a20 2020 2020 2020 2041 2073  str`.        A s
-000290a0: 7472 696e 6720 6f66 2063 6861 6e67 6573  tring of changes
-000290b0: 2066 6f6c 6c6f 7769 6e67 2074 6865 2044   following the D
-000290c0: 434d 4c20 6861 726d 6f6e 7920 7374 616e  CML harmony stan
-000290d0: 6461 7264 2e0a 2020 2020 6f6c 645f 6e75  dard..    old_nu
-000290e0: 6d2c 206e 6577 5f6e 756d 203a 203a 6f62  m, new_num : :ob
-000290f0: 6a3a 6073 7472 603a 0a20 2020 2020 2020  j:`str`:.       
-00029100: 204f 6c64 206e 756d 6572 616c 2c20 6e65   Old numeral, ne
-00029110: 7720 6e75 6d65 7261 6c2e 0a20 2020 206f  w numeral..    o
-00029120: 6c64 5f6d 696e 6f72 2c20 6e65 775f 6d69  ld_minor, new_mi
-00029130: 6e6f 7220 3a20 3a6f 626a 3a60 626f 6f6c  nor : :obj:`bool
-00029140: 602c 206f 7074 696f 6e61 6c0a 2020 2020  `, optional.    
-00029150: 2020 2020 466f 7220 6561 6368 206e 756d      For each num
-00029160: 6572 616c 2c20 7061 7373 2054 7275 6520  eral, pass True 
-00029170: 6966 2069 7420 6f63 6375 7273 2069 6e20  if it occurs in 
-00029180: 6120 6d69 6e6f 7220 636f 6e74 6578 742e  a minor context.
-00029190: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-000291a0: 7064 2e69 736e 756c 6c28 6368 616e 6765  pd.isnull(change
-000291b0: 7329 3a0a 2020 2020 2020 2020 7265 7475  s):.        retu
-000291c0: 726e 2063 6861 6e67 6573 0a20 2020 206f  rn changes.    o
-000291d0: 6c64 203d 2063 6861 6e67 6573 3274 7063  ld = changes2tpc
-000291e0: 2863 6861 6e67 6573 2c20 6f6c 645f 6e75  (changes, old_nu
-000291f0: 6d2c 206d 696e 6f72 3d6f 6c64 5f6d 696e  m, minor=old_min
-00029200: 6f72 2c20 726f 6f74 5f61 6c74 6572 6174  or, root_alterat
-00029210: 696f 6e73 3d54 7275 6529 0a20 2020 206e  ions=True).    n
-00029220: 6577 203d 2063 6861 6e67 6573 3274 7063  ew = changes2tpc
-00029230: 2863 6861 6e67 6573 2c20 6e65 775f 6e75  (changes, new_nu
-00029240: 6d2c 206d 696e 6f72 3d6e 6577 5f6d 696e  m, minor=new_min
-00029250: 6f72 2c20 726f 6f74 5f61 6c74 6572 6174  or, root_alterat
-00029260: 696f 6e73 3d54 7275 6529 0a20 2020 2072  ions=True).    r
-00029270: 6573 203d 205b 5d0a 2020 2020 6765 745f  es = [].    get_
-00029280: 6163 6320 3d20 6c61 6d62 6461 206e 3a20  acc = lambda n: 
-00029290: 6e20 2a20 2723 2720 6966 206e 203e 2030  n * '#' if n > 0
-000292a0: 2065 6c73 6520 2d6e 202a 2027 6227 0a20   else -n * 'b'. 
-000292b0: 2020 2066 6f72 2028 6675 6c6c 2c20 6164     for (full, ad
-000292c0: 6465 642c 2061 6363 2c20 6368 6f72 645f  ded, acc, chord_
-000292d0: 696e 7465 7276 616c 2c20 6976 3129 2c20  interval, iv1), 
-000292e0: 285f 2c20 5f2c 205f 2c20 5f2c 2069 7632  (_, _, _, _, iv2
-000292f0: 2920 696e 207a 6970 286f 6c64 2c20 6e65  ) in zip(old, ne
-00029300: 7729 3a0a 2020 2020 2020 2020 6966 2069  w):.        if i
-00029310: 7631 2069 7320 4e6f 6e65 206f 7220 6976  v1 is None or iv
-00029320: 3120 3d3d 2069 7632 3a0a 2020 2020 2020  1 == iv2:.      
-00029330: 2020 2020 2020 7265 732e 6170 7065 6e64        res.append
-00029340: 2866 756c 6c29 0a20 2020 2020 2020 2065  (full).        e
-00029350: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00029360: 2064 203d 2069 7632 202d 2069 7631 0a20   d = iv2 - iv1. 
-00029370: 2020 2020 2020 2020 2020 2069 6620 6420             if d 
-00029380: 2520 3720 3e20 303a 0a20 2020 2020 2020  % 7 > 0:.       
-00029390: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000293a0: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
-000293b0: 2020 2020 2020 2020 2020 2020 2066 2254               f"T
-000293c0: 6865 2064 6966 6665 7265 6e63 6520 6265  he difference be
-000293d0: 7477 6565 6e20 7468 6520 696e 7465 7276  tween the interv
-000293e0: 616c 7320 6f66 207b 6675 6c6c 7d20 696e  als of {full} in
-000293f0: 207b 6f6c 645f 6e75 6d7d 2061 6e64 207b   {old_num} and {
-00029400: 6e65 775f 6e75 6d7d 2028 696e 207b 276d  new_num} (in {'m
-00029410: 696e 6f72 2720 6966 206d 696e 6f72 2065  inor' if minor e
-00029420: 6c73 6520 276d 616a 6f72 277d 2920 646f  lse 'major'}) do
-00029430: 6e27 7420 6469 6666 6572 2062 7920 6368  n't differ by ch
-00029440: 726f 6d61 7469 6320 7365 6d69 746f 6e65  romatic semitone
-00029450: 732e 2229 0a20 2020 2020 2020 2020 2020  s.").           
-00029460: 206e 5f61 6363 203d 2061 6363 2e63 6f75   n_acc = acc.cou
-00029470: 6e74 2827 2327 2920 2d20 6163 632e 636f  nt('#') - acc.co
-00029480: 756e 7428 2762 2729 0a20 2020 2020 2020  unt('b').       
-00029490: 2020 2020 206e 6577 5f61 6363 203d 2067       new_acc = g
-000294a0: 6574 5f61 6363 286e 5f61 6363 202d 2064  et_acc(n_acc - d
-000294b0: 202f 2f20 3729 0a20 2020 2020 2020 2020   // 7).         
-000294c0: 2020 2072 6573 2e61 7070 656e 6428 6164     res.append(ad
-000294d0: 6465 6420 2b20 6e65 775f 6163 6320 2b20  ded + new_acc + 
-000294e0: 6368 6f72 645f 696e 7465 7276 616c 290a  chord_interval).
-000294f0: 2020 2020 7265 7475 726e 2027 272e 6a6f      return ''.jo
-00029500: 696e 2872 6573 290a 0a0a 4066 756e 6374  in(res)...@funct
-00029510: 696f 6e5f 6c6f 6767 6572 0a64 6566 2066  ion_logger.def f
-00029520: 6561 7475 7265 7332 7470 6373 286e 756d  eatures2tpcs(num
-00029530: 6572 616c 2c20 666f 726d 3d4e 6f6e 652c  eral, form=None,
-00029540: 2066 6967 6261 7373 3d4e 6f6e 652c 2063   figbass=None, c
-00029550: 6861 6e67 6573 3d4e 6f6e 652c 2072 656c  hanges=None, rel
-00029560: 6174 6976 6572 6f6f 743d 4e6f 6e65 2c20  ativeroot=None, 
-00029570: 6b65 793d 2743 272c 206d 696e 6f72 3d4e  key='C', minor=N
-00029580: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00029590: 2020 2020 2020 206d 6572 6765 5f74 6f6e         merge_ton
-000295a0: 6573 3d54 7275 652c 2062 6173 735f 6f6e  es=True, bass_on
-000295b0: 6c79 3d46 616c 7365 2c20 6d63 3d4e 6f6e  ly=False, mc=Non
-000295c0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-000295d0: 4769 7665 6e20 7468 6520 6665 6174 7572  Given the featur
-000295e0: 6573 206f 6620 6120 6368 6f72 6420 6c61  es of a chord la
-000295f0: 6265 6c2c 2074 6869 7320 6675 6e63 7469  bel, this functi
-00029600: 6f6e 2072 6574 7572 6e73 2074 6865 2063  on returns the c
-00029610: 686f 7264 2074 6f6e 6573 0a20 2020 2069  hord tones.    i
-00029620: 6e20 7468 6520 6f72 6465 7220 6f66 2074  n the order of t
-00029630: 6865 2069 6e76 6572 7369 6f6e 2c20 7374  he inversion, st
-00029640: 6172 7469 6e67 2066 726f 6d20 7468 6520  arting from the 
-00029650: 6261 7373 206e 6f74 652e 2054 6865 2074  bass note. The t
-00029660: 6f6e 6573 2061 7265 0a20 2020 2065 7870  ones are.    exp
-00029670: 7265 7373 6564 2061 7320 746f 6e61 6c20  ressed as tonal 
-00029680: 7069 7463 6820 636c 6173 7365 732c 2077  pitch classes, w
-00029690: 6865 7265 202d 313d 462c 2030 3d43 2c20  here -1=F, 0=C, 
-000296a0: 313d 4720 6574 632e 0a0a 2020 2020 5573  1=G etc...    Us
-000296b0: 6573 3a20 3a70 793a 6675 6e63 3a60 7e2e  es: :py:func:`~.
-000296c0: 7574 696c 732e 6368 616e 6765 7332 6c69  utils.changes2li
-000296d0: 7374 602c 203a 7079 3a66 756e 633a 607e  st`, :py:func:`~
-000296e0: 2e75 7469 6c73 2e6e 616d 6532 6669 6674  .utils.name2fift
-000296f0: 6873 602c 203a 7079 3a66 756e 633a 607e  hs`, :py:func:`~
-00029700: 2e75 7469 6c73 2e72 6573 6f6c 7665 5f72  .utils.resolve_r
-00029710: 656c 6174 6976 655f 6b65 7973 602c 203a  elative_keys`, :
-00029720: 7079 3a66 756e 633a 607e 2e75 7469 6c73  py:func:`~.utils
-00029730: 2e72 6f6d 616e 5f6e 756d 6572 616c 3266  .roman_numeral2f
-00029740: 6966 7468 7360 2c0a 2020 2020 3a70 793a  ifths`,.    :py:
-00029750: 6675 6e63 3a60 7e2e 7574 696c 732e 736f  func:`~.utils.so
-00029760: 7274 5f74 7063 7360 2c20 3a70 793a 6675  rt_tpcs`, :py:fu
-00029770: 6e63 3a60 7e2e 7574 696c 732e 7374 725f  nc:`~.utils.str_
-00029780: 6973 5f6d 696e 6f72 600a 0a20 2020 2050  is_minor`..    P
-00029790: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000297a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 756d  --------.    num
-000297b0: 6572 616c 3a20 3a6f 626a 3a60 7374 7260  eral: :obj:`str`
-000297c0: 0a20 2020 2020 2020 2052 6f6d 616e 206e  .        Roman n
-000297d0: 756d 6572 616c 206f 6620 7468 6520 6368  umeral of the ch
-000297e0: 6f72 6427 7320 726f 6f74 0a20 2020 2066  ord's root.    f
-000297f0: 6f72 6d3a 207b 4e6f 6e65 2c20 274d 272c  orm: {None, 'M',
-00029800: 2027 6f27 2c20 272b 2720 2725 277d 2c20   'o', '+' '%'}, 
-00029810: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00029820: 2049 6e64 6963 6174 6573 2074 6865 2063   Indicates the c
-00029830: 686f 7264 2074 7970 6520 6966 206e 6f74  hord type if not
-00029840: 2061 206d 616a 6f72 206f 7220 6d69 6e6f   a major or mino
-00029850: 7220 7472 6961 6420 2866 6f72 2077 6869  r triad (for whi
-00029860: 6368 2060 6066 6f72 6d60 6020 6973 204e  ch ``form`` is N
-00029870: 6f6e 6529 2e0a 2020 2020 2020 2020 2725  one)..        '%
-00029880: 2720 616e 6420 274d 2720 6361 6e20 6f6e  ' and 'M' can on
-00029890: 6c79 206f 6363 7572 2061 7320 7465 7472  ly occur as tetr
-000298a0: 6164 732c 206e 6f74 2061 7320 7472 6961  ads, not as tria
-000298b0: 6473 2e0a 2020 2020 6669 6762 6173 733a  ds..    figbass:
-000298c0: 207b 4e6f 6e65 2c20 2736 272c 2027 3634   {None, '6', '64
-000298d0: 272c 2027 3727 2c20 2736 3527 2c20 2734  ', '7', '65', '4
-000298e0: 3327 2c20 2732 277d 2c20 6f70 7469 6f6e  3', '2'}, option
-000298f0: 616c 0a20 2020 2020 2020 2049 6e64 6963  al.        Indic
-00029900: 6174 6573 2063 686f 7264 2773 2069 6e76  ates chord's inv
-00029910: 6572 7369 6f6e 2e20 5061 7373 204e 6f6e  ersion. Pass Non
-00029920: 6520 666f 7220 7472 6961 6420 726f 6f74  e for triad root
-00029930: 2070 6f73 6974 696f 6e2e 0a20 2020 2063   position..    c
-00029940: 6861 6e67 6573 3a20 3a6f 626a 3a60 7374  hanges: :obj:`st
-00029950: 7260 2c20 6f70 7469 6f6e 616c 0a20 2020  r`, optional.   
-00029960: 2020 2020 2041 6464 6564 2073 7465 7073       Added steps
-00029970: 2073 7563 6820 6173 2027 2b36 2720 6f72   such as '+6' or
-00029980: 2073 7573 7065 6e73 696f 6e73 2073 7563   suspensions suc
-00029990: 6820 6173 2027 3427 206f 7220 616e 7920  h as '4' or any 
-000299a0: 636f 6d62 696e 6174 696f 6e20 7375 6368  combination such
-000299b0: 2061 7320 2839 2b36 3429 2e0a 2020 2020   as (9+64)..    
-000299c0: 2020 2020 4e75 6d62 6572 7320 6e65 6564      Numbers need
-000299d0: 2074 6f20 6265 2069 6e20 6465 7363 656e   to be in descen
-000299e0: 6469 6e67 206f 7264 6572 2e0a 2020 2020  ding order..    
-000299f0: 7265 6c61 7469 7665 726f 6f74 3a20 3a6f  relativeroot: :o
-00029a00: 626a 3a60 7374 7260 2c20 6f70 7469 6f6e  bj:`str`, option
-00029a10: 616c 0a20 2020 2020 2020 2050 6173 7320  al.        Pass 
-00029a20: 6120 526f 6d61 6e20 7363 616c 6520 6465  a Roman scale de
-00029a30: 6772 6565 2069 6620 606e 756d 6572 616c  gree if `numeral
-00029a40: 6020 6973 2074 6f20 6265 2061 7070 6c69  ` is to be appli
-00029a50: 6564 2074 6f20 6120 6469 6666 6572 656e  ed to a differen
-00029a60: 7420 7363 616c 650a 2020 2020 2020 2020  t scale.        
-00029a70: 6465 6772 6565 206f 6620 7468 6520 6c6f  degree of the lo
-00029a80: 6361 6c20 6b65 792c 2061 7320 696e 2027  cal key, as in '
-00029a90: 5636 352f 5627 0a20 2020 206b 6579 203a  V65/V'.    key :
-00029aa0: 203a 6f62 6a3a 6073 7472 6020 6f72 203a   :obj:`str` or :
-00029ab0: 6f62 6a3a 6069 6e74 602c 206f 7074 696f  obj:`int`, optio
-00029ac0: 6e61 6c0a 2020 2020 2020 2020 5468 6520  nal.        The 
-00029ad0: 6c6f 6361 6c20 6b65 7920 6578 7072 6573  local key expres
-00029ae0: 7365 6420 6173 2074 6865 2072 6f6f 7427  sed as the root'
-00029af0: 7320 6e6f 7465 206e 616d 6520 6f72 2061  s note name or a
-00029b00: 2074 6f6e 616c 2070 6974 6368 2063 6c61   tonal pitch cla
-00029b10: 7373 2e0a 2020 2020 2020 2020 4966 2069  ss..        If i
-00029b20: 7420 6973 2061 206e 616d 6520 616e 6420  t is a name and 
-00029b30: 606d 696e 6f72 6020 6973 2060 4e6f 6e65  `minor` is `None
-00029b40: 602c 2075 7070 6572 6361 7365 206d 6561  `, uppercase mea
-00029b50: 6e73 206d 616a 6f72 2061 6e64 206c 6f77  ns major and low
-00029b60: 6572 6361 7365 206d 696e 6f72 2e0a 2020  ercase minor..  
-00029b70: 2020 2020 2020 4966 2069 7420 6973 2061        If it is a
-00029b80: 2074 6f6e 616c 2070 6974 6368 2063 6c61   tonal pitch cla
-00029b90: 7373 2c20 606d 696e 6f72 6020 6e65 6564  ss, `minor` need
-00029ba0: 7320 746f 2062 6520 7370 6563 6966 6965  s to be specifie
-00029bb0: 642e 0a20 2020 206d 696e 6f72 203a 203a  d..    minor : :
-00029bc0: 6f62 6a3a 6062 6f6f 6c60 2c20 6f70 7469  obj:`bool`, opti
-00029bd0: 6f6e 616c 0a20 2020 2020 2020 2050 6173  onal.        Pas
-00029be0: 7320 5472 7565 2066 6f72 206d 696e 6f72  s True for minor
-00029bf0: 2061 6e64 2046 616c 7365 2066 6f72 206d   and False for m
-00029c00: 616a 6f72 2e20 4361 6e20 6265 206f 6d69  ajor. Can be omi
-00029c10: 7474 6564 2069 6620 606b 6579 6020 6973  tted if `key` is
-00029c20: 2061 206e 6f74 6520 6e61 6d65 2e0a 2020   a note name..  
-00029c30: 2020 2020 2020 5468 6973 2061 6666 6563        This affec
-00029c40: 7473 2063 616c 6375 6c61 7469 6f6e 206f  ts calculation o
-00029c50: 6620 6368 6f72 6473 2072 656c 6174 6564  f chords related
-00029c60: 2074 6f20 4949 492c 2056 4920 616e 6420   to III, VI and 
-00029c70: 5649 492e 0a20 2020 206d 6572 6765 5f74  VII..    merge_t
-00029c80: 6f6e 6573 203a 203a 6f62 6a3a 6062 6f6f  ones : :obj:`boo
-00029c90: 6c60 2c20 6f70 7469 6f6e 616c 0a20 2020  l`, optional.   
-00029ca0: 2020 2020 2050 6173 7320 4661 6c73 6520       Pass False 
-00029cb0: 6966 2079 6f75 2077 616e 7420 7468 6520  if you want the 
-00029cc0: 6675 6e63 7469 6f6e 2074 6f20 7265 7475  function to retu
-00029cd0: 726e 2074 776f 2074 7570 6c65 732c 206f  rn two tuples, o
-00029ce0: 6e65 2077 6974 6820 2870 6f74 656e 7469  ne with (potenti
-00029cf0: 616c 6c79 2073 7573 7065 6e64 6564 290a  ally suspended).
-00029d00: 2020 2020 2020 2020 6368 6f72 6420 746f          chord to
-00029d10: 6e65 7320 616e 6420 6f6e 6520 7769 7468  nes and one with
-00029d20: 2061 6464 6564 206e 6f74 6573 2e0a 2020   added notes..  
-00029d30: 2020 6261 7373 5f6f 6e6c 7920 3a20 3a6f    bass_only : :o
-00029d40: 626a 3a60 626f 6f6c 602c 206f 7074 696f  bj:`bool`, optio
-00029d50: 6e61 6c0a 2020 2020 2020 2020 5265 7475  nal.        Retu
-00029d60: 726e 206f 6e6c 7920 7468 6520 6261 7373  rn only the bass
-00029d70: 206e 6f74 6520 696e 7374 6561 6420 6f66   note instead of
-00029d80: 2061 6c6c 2063 686f 7264 2074 6f6e 6573   all chord tones
-00029d90: 2e0a 2020 2020 6d63 203a 2069 6e74 206f  ..    mc : int o
-00029da0: 7220 7374 720a 2020 2020 2020 2020 5061  r str.        Pa
-00029db0: 7373 206d 6561 7375 7265 2063 6f75 6e74  ss measure count
-00029dc0: 2074 6f20 6469 7370 6c61 7920 6974 2069   to display it i
-00029dd0: 6e20 7761 726e 696e 6773 2e0a 0a20 2020  n warnings...   
-00029de0: 2022 2222 0a20 2020 2069 6620 7064 2e69   """.    if pd.i
-00029df0: 736e 756c 6c28 6e75 6d65 7261 6c29 206f  snull(numeral) o
-00029e00: 7220 6e75 6d65 7261 6c20 3d3d 2027 406e  r numeral == '@n
-00029e10: 6f6e 6527 3a0a 2020 2020 2020 2020 6966  one':.        if
-00029e20: 2062 6173 735f 6f6e 6c79 206f 7220 6d65   bass_only or me
-00029e30: 7267 655f 746f 6e65 733a 0a20 2020 2020  rge_tones:.     
-00029e40: 2020 2020 2020 2072 6574 7572 6e20 7064         return pd
-00029e50: 2e4e 410a 2020 2020 2020 2020 656c 7365  .NA.        else
-00029e60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00029e70: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
-00029e80: 2020 2020 2020 2027 6368 6f72 645f 746f         'chord_to
-00029e90: 6e65 7327 3a20 7064 2e4e 412c 0a20 2020  nes': pd.NA,.   
-00029ea0: 2020 2020 2020 2020 2020 2020 2027 6164               'ad
-00029eb0: 6465 645f 746f 6e65 7327 3a20 7064 2e4e  ded_tones': pd.N
-00029ec0: 412c 0a20 2020 2020 2020 2020 2020 2020  A,.             
-00029ed0: 2020 2027 726f 6f74 273a 2070 642e 4e41     'root': pd.NA
-00029ee0: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
-00029ef0: 2020 2020 666f 726d 2c20 6669 6762 6173      form, figbas
-00029f00: 732c 2063 6861 6e67 6573 2c20 7265 6c61  s, changes, rela
-00029f10: 7469 7665 726f 6f74 203d 2074 7570 6c65  tiveroot = tuple
-00029f20: 280a 2020 2020 2020 2020 2727 2069 6620  (.        '' if 
-00029f30: 7064 2e69 736e 756c 6c28 7661 6c29 2065  pd.isnull(val) e
-00029f40: 6c73 6520 7661 6c20 666f 7220 7661 6c20  lse val for val 
-00029f50: 696e 2028 666f 726d 2c20 6669 6762 6173  in (form, figbas
-00029f60: 732c 2063 6861 6e67 6573 2c20 7265 6c61  s, changes, rela
-00029f70: 7469 7665 726f 6f74 2929 0a20 2020 206c  tiveroot)).    l
-00029f80: 6162 656c 203d 2066 227b 6e75 6d65 7261  abel = f"{numera
-00029f90: 6c7d 7b66 6f72 6d7d 7b66 6967 6261 7373  l}{form}{figbass
-00029fa0: 7d7b 2728 2720 2b20 6368 616e 6765 7320  }{'(' + changes 
-00029fb0: 2b20 2729 2720 6966 2063 6861 6e67 6573  + ')' if changes
-00029fc0: 2021 3d20 2727 2065 6c73 6520 2727 7d7b   != '' else ''}{
-00029fd0: 272f 2720 2b20 7265 6c61 7469 7665 726f  '/' + relativero
-00029fe0: 6f74 2069 6620 7265 6c61 7469 7665 726f  ot if relativero
-00029ff0: 6f74 2021 3d20 2727 2065 6c73 6520 2727  ot != '' else ''
-0002a000: 7d22 0a20 2020 204d 4320 3d20 2727 2069  }".    MC = '' i
-0002a010: 6620 6d63 2069 7320 4e6f 6e65 2065 6c73  f mc is None els
-0002a020: 6520 6627 4d43 207b 6d63 7d3a 2027 0a20  e f'MC {mc}: '. 
-0002a030: 2020 2069 6620 6d69 6e6f 7220 6973 204e     if minor is N
-0002a040: 6f6e 653a 0a20 2020 2020 2020 2074 7279  one:.        try
-0002a050: 3a0a 2020 2020 2020 2020 2020 2020 6d69  :.            mi
-0002a060: 6e6f 7220 3d20 7374 725f 6973 5f6d 696e  nor = str_is_min
-0002a070: 6f72 286b 6579 2c20 6973 5f6e 616d 653d  or(key, is_name=
-0002a080: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0002a090: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-0002a0a0: 224d 6f64 6520 696e 6665 7272 6564 2066  "Mode inferred f
-0002a0b0: 726f 6d20 7b6b 6579 7d2e 2229 0a20 2020  rom {key}.").   
-0002a0c0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-0002a0d0: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
-0002a0e0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0002a0f0: 726f 7228 6622 4966 2070 6172 616d 6574  ror(f"If paramet
-0002a100: 6572 2027 6d69 6e6f 7227 2069 7320 6e6f  er 'minor' is no
-0002a110: 7420 7370 6563 6966 6965 642c 2027 6b65  t specified, 'ke
-0002a120: 7927 206e 6565 6473 2074 6f20 6265 2061  y' needs to be a
-0002a130: 2073 7472 696e 672c 206e 6f74 207b 6b65   string, not {ke
-0002a140: 797d 2229 0a0a 2020 2020 6b65 7920 3d20  y}")..    key = 
-0002a150: 6e61 6d65 3266 6966 7468 7328 6b65 792c  name2fifths(key,
-0002a160: 206c 6f67 6765 723d 6c6f 6767 6572 290a   logger=logger).
-0002a170: 0a20 2020 2069 6620 666f 726d 2069 6e20  .    if form in 
-0002a180: 5b27 2527 2c20 274d 272c 2027 2b4d 275d  ['%', 'M', '+M']
-0002a190: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
-0002a1a0: 2066 6967 6261 7373 2069 6e20 5b27 3727   figbass in ['7'
-0002a1b0: 2c20 2736 3527 2c20 2734 3327 2c0a 2020  , '65', '43',.  
-0002a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a1d0: 2020 2020 2020 2020 2027 3227 5d2c 2066           '2'], f
-0002a1e0: 227b 4d43 7d7b 6c61 6265 6c7d 3a20 7b66  "{MC}{label}: {f
-0002a1f0: 6f72 6d7d 2072 6571 7569 7265 7320 6669  orm} requires fi
-0002a200: 6762 6173 7320 2837 2c20 3635 2c20 3433  gbass (7, 65, 43
-0002a210: 2c20 6f72 2032 2920 7369 6e63 6520 6974  , or 2) since it
-0002a220: 2073 7065 6369 6669 6573 2061 2063 686f   specifies a cho
-0002a230: 7264 2773 2073 6576 656e 7468 2e22 0a0a  rd's seventh."..
-0002a240: 2020 2020 6966 2072 656c 6174 6976 6572      if relativer
-0002a250: 6f6f 7420 213d 2027 273a 0a20 2020 2020  oot != '':.     
-0002a260: 2020 2072 6573 6f6c 7665 6420 3d20 7265     resolved = re
-0002a270: 736f 6c76 655f 7265 6c61 7469 7665 5f6b  solve_relative_k
-0002a280: 6579 7328 7265 6c61 7469 7665 726f 6f74  eys(relativeroot
-0002a290: 2c20 6d69 6e6f 722c 206c 6f67 6765 723d  , minor, logger=
-0002a2a0: 6c6f 6767 6572 290a 2020 2020 2020 2020  logger).        
-0002a2b0: 7265 6c5f 6d69 6e6f 7220 3d20 7374 725f  rel_minor = str_
-0002a2c0: 6973 5f6d 696e 6f72 2872 6573 6f6c 7665  is_minor(resolve
-0002a2d0: 642c 2069 735f 6e61 6d65 3d46 616c 7365  d, is_name=False
-0002a2e0: 290a 2020 2020 2020 2020 7472 616e 7370  ).        transp
-0002a2f0: 203d 2072 6f6d 616e 5f6e 756d 6572 616c   = roman_numeral
-0002a300: 3266 6966 7468 7328 7265 736f 6c76 6564  2fifths(resolved
-0002a310: 2c20 6d69 6e6f 722c 206c 6f67 6765 723d  , minor, logger=
-0002a320: 6c6f 6767 6572 290a 2020 2020 2020 2020  logger).        
-0002a330: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
-0002a340: 2020 2020 2020 2020 2020 6622 7b4d 437d            f"{MC}
-0002a350: 4368 6f72 6420 6170 706c 6965 6420 746f  Chord applied to
-0002a360: 207b 7265 6c61 7469 7665 726f 6f74 7d2e   {relativeroot}.
-0002a370: 2054 6865 7265 666f 7265 2074 7261 6e73   Therefore trans
-0002a380: 706f 7369 6e67 2069 7420 6279 207b 7472  posing it by {tr
-0002a390: 616e 7370 7d20 6669 6674 6873 2e22 290a  ansp} fifths.").
-0002a3a0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-0002a3b0: 6561 7475 7265 7332 7470 6373 286e 756d  eatures2tpcs(num
-0002a3c0: 6572 616c 3d6e 756d 6572 616c 2c20 666f  eral=numeral, fo
-0002a3d0: 726d 3d66 6f72 6d2c 2066 6967 6261 7373  rm=form, figbass
-0002a3e0: 3d66 6967 6261 7373 2c20 7265 6c61 7469  =figbass, relati
-0002a3f0: 7665 726f 6f74 3d4e 6f6e 652c 2063 6861  veroot=None, cha
-0002a400: 6e67 6573 3d63 6861 6e67 6573 2c0a 2020  nges=changes,.  
-0002a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a420: 2020 2020 2020 2020 2020 206b 6579 3d6b             key=k
-0002a430: 6579 202b 2074 7261 6e73 702c 206d 696e  ey + transp, min
-0002a440: 6f72 3d72 656c 5f6d 696e 6f72 2c20 6d65  or=rel_minor, me
-0002a450: 7267 655f 746f 6e65 733d 6d65 7267 655f  rge_tones=merge_
-0002a460: 746f 6e65 732c 2062 6173 735f 6f6e 6c79  tones, bass_only
-0002a470: 3d62 6173 735f 6f6e 6c79 2c20 6d63 3d6d  =bass_only, mc=m
-0002a480: 632c 0a20 2020 2020 2020 2020 2020 2020  c,.             
-0002a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a4a0: 6c6f 6767 6572 3d6c 6f67 6765 7229 0a0a  logger=logger)..
-0002a4b0: 2020 2020 6966 206e 756d 6572 616c 2e6c      if numeral.l
-0002a4c0: 6f77 6572 2829 203d 3d20 2723 7669 6927  ower() == '#vii'
-0002a4d0: 2061 6e64 206e 6f74 206d 696e 6f72 3a0a   and not minor:.
-0002a4e0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-0002a4f0: 6172 6e69 6e67 2866 227b 4d43 7d7b 6e75  arning(f"{MC}{nu
-0002a500: 6d65 7261 6c7d 2069 6e20 6d61 6a6f 7220  meral} in major 
-0002a510: 636f 6e74 6578 7420 636f 7272 6563 7465  context correcte
-0002a520: 6420 746f 207b 6e75 6d65 7261 6c5b 313a  d to {numeral[1:
-0002a530: 5d7d 2e22 2c0a 2020 2020 2020 2020 2020  ]}.",.          
-0002a540: 2020 2020 2020 2020 2020 2020 2065 7874               ext
-0002a550: 7261 3d7b 276d 6573 7361 6765 5f69 6427  ra={'message_id'
-0002a560: 3a20 2832 372c 204d 4329 7d29 0a20 2020  : (27, MC)}).   
-0002a570: 2020 2020 206e 756d 6572 616c 203d 206e       numeral = n
-0002a580: 756d 6572 616c 5b31 3a5d 0a0a 2020 2020  umeral[1:]..    
-0002a590: 726f 6f74 5f61 6c74 6572 6174 696f 6e2c  root_alteration,
-0002a5a0: 206e 756d 5f64 6567 7265 6520 3d20 7370   num_degree = sp
-0002a5b0: 6c69 745f 7363 616c 655f 6465 6772 6565  lit_scale_degree
-0002a5c0: 286e 756d 6572 616c 2c20 636f 756e 743d  (numeral, count=
-0002a5d0: 5472 7565 2c20 6c6f 6767 6572 3d6c 6f67  True, logger=log
-0002a5e0: 6765 7229 0a0a 2020 2020 2320 6275 696c  ger)..    # buil
-0002a5f0: 6420 322d 6f63 7461 7665 2064 6961 746f  d 2-octave diato
-0002a600: 6e69 6320 7363 616c 6520 6f6e 2043 206d  nic scale on C m
-0002a610: 616a 6f72 2f6d 696e 6f72 0a20 2020 2072  ajor/minor.    r
-0002a620: 6f6f 7420 3d20 5b27 4927 2c20 2749 4927  oot = ['I', 'II'
-0002a630: 2c20 2749 4949 272c 2027 4956 272c 2027  , 'III', 'IV', '
-0002a640: 5627 2c20 2756 4927 2c20 2756 4949 275d  V', 'VI', 'VII']
-0002a650: 2e69 6e64 6578 286e 756d 5f64 6567 7265  .index(num_degre
-0002a660: 652e 7570 7065 7228 2929 0a20 2020 2074  e.upper()).    t
-0002a670: 7063 7320 3d20 3220 2a20 5b69 202b 206b  pcs = 2 * [i + k
-0002a680: 6579 2066 6f72 2069 2069 6e20 2830 2c20  ey for i in (0, 
-0002a690: 322c 202d 332c 202d 312c 2031 2c20 2d34  2, -3, -1, 1, -4
-0002a6a0: 2c20 2d32 295d 2069 6620 6d69 6e6f 7220  , -2)] if minor 
-0002a6b0: 656c 7365 2032 202a 205b 6920 2b20 6b65  else 2 * [i + ke
-0002a6c0: 7920 666f 7220 6920 696e 2028 302c 2032  y for i in (0, 2
-0002a6d0: 2c20 342c 202d 312c 2031 2c20 332c 2035  , 4, -1, 1, 3, 5
-0002a6e0: 295d 0a20 2020 2023 2073 7461 7274 696e  )].    # startin
-0002a6f0: 6720 7468 6520 7363 616c 6520 6672 6f6d  g the scale from
-0002a700: 2063 686f 7264 2072 6f6f 742c 2069 2e65   chord root, i.e
-0002a710: 2e20 726f 6f74 2077 696c 6c20 6265 2074  . root will be t
-0002a720: 7063 735b 305d 2c20 7468 6520 6368 6f72  pcs[0], the chor
-0002a730: 6427 7320 7365 7665 6e74 6820 7470 6373  d's seventh tpcs
-0002a740: 5b36 5d20 6574 632e 0a20 2020 2074 7063  [6] etc..    tpc
-0002a750: 7320 3d20 7470 6373 5b72 6f6f 743a 5d20  s = tpcs[root:] 
-0002a760: 2b20 7470 6373 5b3a 726f 6f74 5d0a 2020  + tpcs[:root].  
-0002a770: 2020 726f 6f74 203d 2074 7063 735b 305d    root = tpcs[0]
-0002a780: 202b 2037 202a 2072 6f6f 745f 616c 7465   + 7 * root_alte
-0002a790: 7261 7469 6f6e 0a20 2020 2074 7063 735b  ration.    tpcs[
-0002a7a0: 305d 203d 2072 6f6f 7420 2023 206f 6374  0] = root  # oct
-0002a7b0: 6176 6520 7374 6179 7320 6469 6174 6f6e  ave stays diaton
-0002a7c0: 6963 2c20 6973 206e 6f74 2061 6c74 6572  ic, is not alter
-0002a7d0: 6564 0a20 2020 2023 6c6f 6767 6572 2e64  ed.    #logger.d
-0002a7e0: 6562 7567 2866 227b 6e75 6d5f 6465 6772  ebug(f"{num_degr
-0002a7f0: 6565 7d3a 2054 6865 207b 276d 696e 6f72  ee}: The {'minor
-0002a800: 2720 6966 206d 696e 6f72 2065 6c73 6520  ' if minor else 
-0002a810: 276d 616a 6f72 277d 2073 6361 6c65 2073  'major'} scale s
-0002a820: 7461 7274 696e 6720 6672 6f6d 2074 6865  tarting from the
-0002a830: 2072 6f6f 743a 207b 7470 6373 7d22 290a   root: {tpcs}").
-0002a840: 0a20 2020 2064 6566 2073 6574 5f69 7628  .    def set_iv(
-0002a850: 6368 6f72 645f 696e 7465 7276 616c 2c20  chord_interval, 
-0002a860: 696e 7465 7276 616c 5f73 697a 6529 3a0a  interval_size):.
-0002a870: 2020 2020 2020 2020 2222 2220 4164 6420          """ Add 
-0002a880: 746f 2074 6865 2069 6e74 6572 7661 6c20  to the interval 
-0002a890: 6f66 2061 2067 6976 656e 2063 686f 7264  of a given chord
-0002a8a0: 2069 6e74 6572 7661 6c20 696e 2060 7470   interval in `tp
-0002a8b0: 6373 6020 2862 6f74 6820 7669 6577 6564  cs` (both viewed
-0002a8c0: 2066 726f 6d20 7468 6520 726f 6f74 206e   from the root n
-0002a8d0: 6f74 6529 2e0a 0a20 2020 2020 2020 2050  ote)...        P
-0002a8e0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0002a8f0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0002a900: 2020 2020 2063 686f 7264 5f69 6e74 6572       chord_inter
-0002a910: 7661 6c20 3a20 3a6f 626a 3a60 696e 7460  val : :obj:`int`
-0002a920: 0a20 2020 2020 2020 2020 2020 2050 6173  .            Pas
-0002a930: 7320 3020 666f 7220 7468 6520 726f 6f74  s 0 for the root
-0002a940: 206e 6f74 652c 2032 2066 6f72 2074 6865   note, 2 for the
-0002a950: 2074 6869 7264 2c20 3820 666f 7220 7468   third, 8 for th
-0002a960: 6520 6e69 6e74 6820 6574 632e 0a20 2020  e ninth etc..   
-0002a970: 2020 2020 2069 6e74 6572 7661 6c5f 7369       interval_si
-0002a980: 7a65 203a 203a 6f62 6a3a 6069 6e74 600a  ze : :obj:`int`.
-0002a990: 2020 2020 2020 2020 2020 2020 5374 6163              Stac
-0002a9a0: 6b2d 6f66 2d66 6966 7468 7320 696e 7465  k-of-fifths inte
-0002a9b0: 7276 616c 2e0a 2020 2020 2020 2020 2222  rval..        ""
-0002a9c0: 220a 2020 2020 2020 2020 6e6f 6e6c 6f63  ".        nonloc
-0002a9d0: 616c 2074 7063 732c 2072 6f6f 740a 2020  al tpcs, root.  
-0002a9e0: 2020 2020 2020 6976 203d 2072 6f6f 7420        iv = root 
-0002a9f0: 2b20 696e 7465 7276 616c 5f73 697a 650a  + interval_size.
-0002aa00: 2020 2020 2020 2020 7470 6373 5b63 686f          tpcs[cho
-0002aa10: 7264 5f69 6e74 6572 7661 6c5d 203d 2069  rd_interval] = i
-0002aa20: 760a 2020 2020 2020 2020 7470 6373 5b63  v.        tpcs[c
-0002aa30: 686f 7264 5f69 6e74 6572 7661 6c20 2b20  hord_interval + 
-0002aa40: 375d 203d 2069 760a 0a20 2020 2069 735f  7] = iv..    is_
-0002aa50: 7472 6961 6420 3d20 6669 6762 6173 7320  triad = figbass 
-0002aa60: 696e 205b 2727 2c20 2736 272c 2027 3634  in ['', '6', '64
-0002aa70: 275d 0a20 2020 2069 735f 7365 7665 6e74  '].    is_sevent
-0002aa80: 685f 6368 6f72 6420 3d20 6669 6762 6173  h_chord = figbas
-0002aa90: 7320 696e 205b 2737 272c 2027 3635 272c  s in ['7', '65',
-0002aaa0: 2027 3433 272c 2027 3227 5d0a 2020 2020   '43', '2'].    
-0002aab0: 6966 206e 6f74 2069 735f 7472 6961 6420  if not is_triad 
-0002aac0: 616e 6420 6e6f 7420 6973 5f73 6576 656e  and not is_seven
-0002aad0: 7468 5f63 686f 7264 3a0a 2020 2020 2020  th_chord:.      
-0002aae0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0002aaf0: 6f72 2866 227b 4d43 7d7b 6669 6762 6173  or(f"{MC}{figbas
-0002ab00: 737d 2069 7320 6e6f 7420 6120 7661 6c69  s} is not a vali
-0002ab10: 6420 6368 6f72 6420 696e 7665 7273 696f  d chord inversio
-0002ab20: 6e2e 2229 0a0a 2020 2020 6966 2066 6f72  n.")..    if for
-0002ab30: 6d20 3d3d 2027 6f27 3a0a 2020 2020 2020  m == 'o':.      
-0002ab40: 2020 7365 745f 6976 2832 2c20 2d33 290a    set_iv(2, -3).
-0002ab50: 2020 2020 2020 2020 7365 745f 6976 2834          set_iv(4
-0002ab60: 2c20 2d36 290a 2020 2020 2020 2020 6966  , -6).        if
-0002ab70: 2069 735f 7365 7665 6e74 685f 6368 6f72   is_seventh_chor
-0002ab80: 643a 0a20 2020 2020 2020 2020 2020 2073  d:.            s
-0002ab90: 6574 5f69 7628 362c 202d 3929 0a20 2020  et_iv(6, -9).   
-0002aba0: 2065 6c69 6620 666f 726d 203d 3d20 2725   elif form == '%
-0002abb0: 273a 0a20 2020 2020 2020 2073 6574 5f69  ':.        set_i
-0002abc0: 7628 322c 202d 3329 0a20 2020 2020 2020  v(2, -3).       
-0002abd0: 2073 6574 5f69 7628 342c 202d 3629 0a20   set_iv(4, -6). 
-0002abe0: 2020 2020 2020 2073 6574 5f69 7628 362c         set_iv(6,
-0002abf0: 202d 3229 0a20 2020 2065 6c69 6620 666f   -2).    elif fo
-0002ac00: 726d 203d 3d20 272b 273a 0a20 2020 2020  rm == '+':.     
-0002ac10: 2020 2073 6574 5f69 7628 322c 2034 290a     set_iv(2, 4).
-0002ac20: 2020 2020 2020 2020 7365 745f 6976 2834          set_iv(4
-0002ac30: 2c20 3829 0a20 2020 2020 2020 2069 6620  , 8).        if 
-0002ac40: 6973 5f73 6576 656e 7468 5f63 686f 7264  is_seventh_chord
-0002ac50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002ac60: 745f 6976 2836 2c20 2d32 290a 2020 2020  t_iv(6, -2).    
-0002ac70: 656c 6966 2066 6f72 6d20 3d3d 2027 2b4d  elif form == '+M
-0002ac80: 273a 0a20 2020 2020 2020 2073 6574 5f69  ':.        set_i
-0002ac90: 7628 322c 2034 290a 2020 2020 2020 2020  v(2, 4).        
-0002aca0: 7365 745f 6976 2834 2c20 3829 0a20 2020  set_iv(4, 8).   
-0002acb0: 2020 2020 2073 6574 5f69 7628 362c 2035       set_iv(6, 5
-0002acc0: 290a 2020 2020 656c 7365 3a20 2023 2074  ).    else:  # t
-0002acd0: 7269 6164 2077 6974 6820 6f72 2077 6974  riad with or wit
-0002ace0: 686f 7574 206d 616a 6f72 206f 7220 6d69  hout major or mi
-0002acf0: 6e6f 7220 7365 7665 6e0a 2020 2020 2020  nor seven.      
-0002ad00: 2020 7365 745f 6976 2834 2c20 3129 0a20    set_iv(4, 1). 
-0002ad10: 2020 2020 2020 2069 6620 6e75 6d5f 6465         if num_de
-0002ad20: 6772 6565 2e69 7375 7070 6572 2829 3a0a  gree.isupper():.
-0002ad30: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-0002ad40: 6976 2832 2c20 3429 0a20 2020 2020 2020  iv(2, 4).       
-0002ad50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0002ad60: 2020 2073 6574 5f69 7628 322c 202d 3329     set_iv(2, -3)
-0002ad70: 0a20 2020 2020 2020 2069 6620 666f 726d  .        if form
-0002ad80: 203d 3d20 274d 273a 0a20 2020 2020 2020   == 'M':.       
-0002ad90: 2020 2020 2073 6574 5f69 7628 362c 2035       set_iv(6, 5
-0002ada0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
-0002adb0: 735f 7365 7665 6e74 685f 6368 6f72 643a  s_seventh_chord:
-0002adc0: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
-0002add0: 5f69 7628 362c 202d 3229 0a0a 2020 2020  _iv(6, -2)..    
-0002ade0: 746f 6e65 5f66 756e 6374 696f 6e73 203d  tone_functions =
-0002adf0: 2028 302c 2032 2c20 342c 2036 2920 6966   (0, 2, 4, 6) if
-0002ae00: 2069 735f 7365 7665 6e74 685f 6368 6f72   is_seventh_chor
-0002ae10: 6420 656c 7365 2028 302c 2032 2c20 3429  d else (0, 2, 4)
-0002ae20: 0a20 2020 2072 6f6f 745f 706f 7369 7469  .    root_positi
-0002ae30: 6f6e 203d 207b 693a 205b 7470 6373 5b69  on = {i: [tpcs[i
-0002ae40: 5d5d 2066 6f72 2069 2069 6e20 746f 6e65  ]] for i in tone
-0002ae50: 5f66 756e 6374 696f 6e73 7d0a 2020 2020  _functions}.    
-0002ae60: 7265 706c 6163 656d 656e 7473 2020 3d20  replacements  = 
-0002ae70: 7b69 3a20 5b5d 2066 6f72 2069 2069 6e20  {i: [] for i in 
-0002ae80: 746f 6e65 5f66 756e 6374 696f 6e73 7d0a  tone_functions}.
-0002ae90: 0a20 2020 2064 6566 2072 6570 6c61 6365  .    def replace
-0002aea0: 5f63 686f 7264 5f74 6f6e 6528 7768 6963  _chord_tone(whic
-0002aeb0: 682c 2062 7929 3a0a 2020 2020 2020 2020  h, by):.        
-0002aec0: 6e6f 6e6c 6f63 616c 2072 6f6f 745f 706f  nonlocal root_po
-0002aed0: 7369 7469 6f6e 2c20 7265 706c 6163 656d  sition, replacem
-0002aee0: 656e 7473 0a20 2020 2020 2020 2069 6620  ents.        if 
-0002aef0: 7768 6963 6820 696e 2072 6f6f 745f 706f  which in root_po
-0002af00: 7369 7469 6f6e 3a0a 2020 2020 2020 2020  sition:.        
-0002af10: 2020 2020 726f 6f74 5f70 6f73 6974 696f      root_positio
-0002af20: 6e5b 7768 6963 685d 203d 205b 5d0a 2020  n[which] = [].  
-0002af30: 2020 2020 2020 2020 2020 7265 706c 6163            replac
-0002af40: 656d 656e 7473 5b77 6869 6368 5d2e 696e  ements[which].in
-0002af50: 7365 7274 2830 2c20 6279 290a 2020 2020  sert(0, by).    
-0002af60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002af70: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-0002af80: 6e69 6e67 2866 224f 6e6c 7920 6368 6f72  ning(f"Only chor
-0002af90: 6420 746f 6e65 7320 5b30 2c32 2c34 2c28  d tones [0,2,4,(
-0002afa0: 3629 5d20 6361 6e20 6265 2072 6570 6c61  6)] can be repla
-0002afb0: 6365 642c 206e 6f74 207b 7768 6963 687d  ced, not {which}
-0002afc0: 2229 0a0a 2020 2020 2320 6170 706c 7920  ")..    # apply 
-0002afd0: 6368 616e 6765 730a 2020 2020 616c 7473  changes.    alts
-0002afe0: 203d 2063 6861 6e67 6573 326c 6973 7428   = changes2list(
-0002aff0: 6368 616e 6765 732c 2073 6f72 743d 4661  changes, sort=Fa
-0002b000: 6c73 6529 0a20 2020 2061 6464 6564 5f6e  lse).    added_n
-0002b010: 6f74 6573 203d 205b 5d0a 2020 2020 666f  otes = [].    fo
-0002b020: 7220 6675 6c6c 2c20 6164 645f 7265 6d6f  r full, add_remo
-0002b030: 7665 2c20 6163 632c 2063 686f 7264 5f69  ve, acc, chord_i
-0002b040: 6e74 6572 7661 6c20 696e 2061 6c74 733a  nterval in alts:
-0002b050: 0a20 2020 2020 2020 2061 6464 6564 203d  .        added =
-0002b060: 2061 6464 5f72 656d 6f76 6520 3d3d 2027   add_remove == '
-0002b070: 2b27 0a20 2020 2020 2020 2073 7562 7374  +'.        subst
-0002b080: 7261 6374 6564 203d 2061 6464 5f72 656d  racted = add_rem
-0002b090: 6f76 6520 3d3d 2027 2d27 0a20 2020 2020  ove == '-'.     
-0002b0a0: 2020 2072 6570 6c61 6369 6e67 5f75 7070     replacing_upp
-0002b0b0: 6572 203d 2061 6464 5f72 656d 6f76 6520  er = add_remove 
-0002b0c0: 3d3d 2027 5e27 0a20 2020 2020 2020 2072  == '^'.        r
-0002b0d0: 6570 6c61 6369 6e67 5f6c 6f77 6572 203d  eplacing_lower =
-0002b0e0: 2061 6464 5f72 656d 6f76 6520 3d3d 2027   add_remove == '
-0002b0f0: 7627 0a20 2020 2020 2020 2063 686f 7264  v'.        chord
-0002b100: 5f69 6e74 6572 7661 6c20 3d20 696e 7428  _interval = int(
-0002b110: 6368 6f72 645f 696e 7465 7276 616c 2920  chord_interval) 
-0002b120: 2d20 310a 2020 2020 2020 2020 2323 2320  - 1.        ### 
-0002b130: 4672 6f6d 2068 6572 6520 6f6e 2c20 6063  From here on, `c
-0002b140: 686f 7264 5f69 6e74 6572 7661 6c60 2069  hord_interval` i
-0002b150: 7320 6465 6372 656d 656e 7465 642c 2069  s decremented, i
-0002b160: 2e65 2e20 7468 6520 726f 6f74 2069 7320  .e. the root is 
-0002b170: 302c 2074 6865 2073 6576 656e 7468 2069  0, the seventh i
-0002b180: 7320 3620 6574 632e 2028 6a75 7374 206c  s 6 etc. (just l
-0002b190: 696b 6520 696e 2060 7470 6373 6029 0a20  ike in `tpcs`). 
-0002b1a0: 2020 2020 2020 2069 6620 2863 686f 7264         if (chord
-0002b1b0: 5f69 6e74 6572 7661 6c20 3d3d 2030 2061  _interval == 0 a
-0002b1c0: 6e64 206e 6f74 2073 7562 7374 7261 6374  nd not substract
-0002b1d0: 6564 2920 6f72 2063 686f 7264 5f69 6e74  ed) or chord_int
-0002b1e0: 6572 7661 6c20 3e20 3133 3a0a 2020 2020  erval > 13:.    
-0002b1f0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-0002b200: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-0002b210: 2020 2020 2020 2020 6622 7b4d 437d 4368          f"{MC}Ch
-0002b220: 616e 6765 207b 6675 6c6c 7d20 6973 206d  ange {full} is m
-0002b230: 6561 6e69 6e67 6c65 7373 2061 6e64 2069  eaningless and i
-0002b240: 676e 6f72 6564 2062 6563 6175 7365 2069  gnored because i
-0002b250: 7420 636f 6e63 6572 6e73 2063 686f 7264  t concerns chord
-0002b260: 2074 6f6e 6520 7b63 686f 7264 5f69 6e74   tone {chord_int
-0002b270: 6572 7661 6c20 2b20 317d 2e22 290a 2020  erval + 1}.").  
-0002b280: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0002b290: 7565 0a20 2020 2020 2020 206e 6578 745f  ue.        next_
-0002b2a0: 6f63 7461 7665 203d 2063 686f 7264 5f69  octave = chord_i
-0002b2b0: 6e74 6572 7661 6c20 3e20 370a 2020 2020  nterval > 7.    
-0002b2c0: 2020 2020 7368 6966 7420 3d20 3720 2a20      shift = 7 * 
-0002b2d0: 2861 6363 2e63 6f75 6e74 2827 2327 2920  (acc.count('#') 
-0002b2e0: 2d20 6163 632e 636f 756e 7428 2762 2729  - acc.count('b')
-0002b2f0: 290a 2020 2020 2020 2020 6e65 775f 7661  ).        new_va
-0002b300: 6c20 3d20 7470 6373 5b63 686f 7264 5f69  l = tpcs[chord_i
-0002b310: 6e74 6572 7661 6c5d 202b 2073 6869 6674  nterval] + shift
-0002b320: 0a20 2020 2020 2020 2069 6620 7375 6273  .        if subs
-0002b330: 7472 6163 7465 643a 0a20 2020 2020 2020  tracted:.       
-0002b340: 2020 2020 2069 6620 6368 6f72 645f 696e       if chord_in
-0002b350: 7465 7276 616c 206e 6f74 2069 6e20 746f  terval not in to
-0002b360: 6e65 5f66 756e 6374 696f 6e73 3a0a 2020  ne_functions:.  
-0002b370: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0002b380: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
-0002b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b3a0: 2020 6622 7b4d 437d 5468 6520 6368 616e    f"{MC}The chan
-0002b3b0: 6765 207b 6675 6c6c 7d20 6861 7320 6e6f  ge {full} has no
-0002b3c0: 2065 6666 6563 7420 6265 6361 7573 6520   effect because 
-0002b3d0: 6974 2063 6f6e 6365 726e 7320 616e 2069  it concerns an i
-0002b3e0: 6e74 6572 7661 6c20 7768 6963 6820 6973  nterval which is
-0002b3f0: 206e 6f74 2069 6d70 6c69 6564 2062 7920   not implied by 
-0002b400: 7b6e 756d 6572 616c 7d7b 666f 726d 7d7b  {numeral}{form}{
-0002b410: 6669 6762 6173 737d 2e22 290a 2020 2020  figbass}.").    
-0002b420: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002b430: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-0002b440: 6f74 5f70 6f73 6974 696f 6e5b 6368 6f72  ot_position[chor
-0002b450: 645f 696e 7465 7276 616c 5d20 3d20 5b5d  d_interval] = []
-0002b460: 0a20 2020 2020 2020 2065 6c69 6620 6164  .        elif ad
-0002b470: 6465 643a 0a20 2020 2020 2020 2020 2020  ded:.           
-0002b480: 2061 6464 6564 5f6e 6f74 6573 2e61 7070   added_notes.app
-0002b490: 656e 6428 6e65 775f 7661 6c29 0a20 2020  end(new_val).   
-0002b4a0: 2020 2020 2065 6c69 6620 6e65 7874 5f6f       elif next_o
-0002b4b0: 6374 6176 653a 0a20 2020 2020 2020 2020  ctave:.         
-0002b4c0: 2020 2069 6620 616e 7928 2872 6570 6c61     if any((repla
-0002b4d0: 6369 6e67 5f6c 6f77 6572 2c20 7265 706c  cing_lower, repl
-0002b4e0: 6163 696e 675f 7570 7065 722c 2073 7562  acing_upper, sub
-0002b4f0: 7374 7261 6374 6564 2929 3a0a 2020 2020  stracted)):.    
-0002b500: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0002b510: 6572 2e69 6e66 6f28 6622 7b4d 437d 7b66  er.info(f"{MC}{f
-0002b520: 756c 6c5b 305d 7d20 6861 7320 6e6f 2065  ull[0]} has no e
-0002b530: 6666 6563 7420 696e 207b 6675 6c6c 7d20  ffect in {full} 
-0002b540: 2062 6563 6175 7365 2074 6865 2069 6e74   because the int
-0002b550: 6572 7661 6c20 6973 206c 6172 6765 7220  erval is larger 
-0002b560: 7468 616e 2061 6e20 6f63 7461 7665 2e22  than an octave."
-0002b570: 290a 2020 2020 2020 2020 2020 2020 6164  ).            ad
-0002b580: 6465 645f 6e6f 7465 732e 6170 7065 6e64  ded_notes.append
-0002b590: 286e 6577 5f76 616c 290a 2020 2020 2020  (new_val).      
-0002b5a0: 2020 656c 6966 2063 686f 7264 5f69 6e74    elif chord_int
-0002b5b0: 6572 7661 6c20 696e 205b 312c 2033 2c20  erval in [1, 3, 
-0002b5c0: 355d 3a20 2023 2074 6865 7365 2061 7265  5]:  # these are
-0002b5d0: 2063 6861 6e67 6573 2074 6f20 7363 616c   changes to scal
-0002b5e0: 6520 6465 6772 6565 2032 2c20 342c 2036  e degree 2, 4, 6
-0002b5f0: 2074 6861 7420 7265 706c 6163 6520 7468   that replace th
-0002b600: 6520 6c6f 7765 7220 6e65 6967 6862 6f75  e lower neighbou
-0002b610: 7220 756e 6c65 7373 2074 6865 7920 6861  r unless they ha
-0002b620: 7665 2061 2023 206f 7220 5e0a 2020 2020  ve a # or ^.    
-0002b630: 2020 2020 2020 2020 6966 2027 2327 2069          if '#' i
-0002b640: 6e20 6163 6320 6f72 2072 6570 6c61 6369  n acc or replaci
-0002b650: 6e67 5f75 7070 6572 3a0a 2020 2020 2020  ng_upper:.      
-0002b660: 2020 2020 2020 2020 2020 6966 2027 2327            if '#'
-0002b670: 2069 6e20 6163 6320 616e 6420 7265 706c   in acc and repl
-0002b680: 6163 696e 675f 7570 7065 723a 0a20 2020  acing_upper:.   
-0002b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b6a0: 206c 6f67 6765 722e 696e 666f 2866 227b   logger.info(f"{
-0002b6b0: 4d43 7d5e 2069 7320 7265 6475 6e64 616e  MC}^ is redundan
-0002b6c0: 7420 696e 207b 6675 6c6c 7d2e 2229 0a20  t in {full}."). 
-0002b6d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0002b6e0: 6620 6368 6f72 645f 696e 7465 7276 616c  f chord_interval
-0002b6f0: 203d 3d20 3520 616e 6420 6973 5f74 7269   == 5 and is_tri
-0002b700: 6164 3a20 2023 206c 6561 6469 6e67 2074  ad:  # leading t
-0002b710: 6f6e 6520 746f 2037 2062 7574 206e 6f74  one to 7 but not
-0002b720: 2069 6e20 7365 7665 6e74 6820 6368 6f72   in seventh chor
-0002b730: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0002b740: 2020 2020 2020 6164 6465 645f 6e6f 7465        added_note
-0002b750: 732e 6170 7065 6e64 286e 6577 5f76 616c  s.append(new_val
-0002b760: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002b770: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002b780: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-0002b790: 6163 655f 6368 6f72 645f 746f 6e65 2863  ace_chord_tone(c
-0002b7a0: 686f 7264 5f69 6e74 6572 7661 6c20 2b20  hord_interval + 
-0002b7b0: 312c 206e 6577 5f76 616c 290a 2020 2020  1, new_val).    
-0002b7c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002b7d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002b7e0: 2072 6570 6c61 6369 6e67 5f6c 6f77 6572   replacing_lower
-0002b7f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002b800: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-0002b810: 6f28 6622 7b4d 437d 7620 6973 2072 6564  o(f"{MC}v is red
-0002b820: 756e 6461 6e74 2069 6e20 7b66 756c 6c7d  undant in {full}
-0002b830: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0002b840: 2020 2020 7265 706c 6163 655f 6368 6f72      replace_chor
-0002b850: 645f 746f 6e65 2863 686f 7264 5f69 6e74  d_tone(chord_int
-0002b860: 6572 7661 6c20 2d20 312c 206e 6577 5f76  erval - 1, new_v
-0002b870: 616c 290a 2020 2020 2020 2020 656c 7365  al).        else
-0002b880: 3a20 2023 2063 686f 7264 2074 6f6e 6520  :  # chord tone 
-0002b890: 616c 7465 7261 7469 6f6e 730a 2020 2020  alterations.    
-0002b8a0: 2020 2020 2020 2020 6966 2072 6570 6c61          if repla
-0002b8b0: 6369 6e67 5f6c 6f77 6572 3a0a 2020 2020  cing_lower:.    
-0002b8c0: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
-0002b8d0: 444f 3a20 5468 6973 206d 7573 7420 6265  DO: This must be
-0002b8e0: 2070 6f73 7369 626c 652c 2065 2e67 2e20   possible, e.g. 
-0002b8f0: 5628 3676 3529 2077 6865 7265 2035 2069  V(6v5) where 5 i
-0002b900: 7320 7375 7370 656e 7369 6f6e 206f 6620  s suspension of 
-0002b910: 340a 2020 2020 2020 2020 2020 2020 2020  4.              
-0002b920: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
-0002b930: 7b4d 437d 7b66 756c 6c7d 202d 3e20 6368  {MC}{full} -> ch
-0002b940: 6f72 6420 746f 6e65 7320 6361 6e6e 6f74  ord tones cannot
-0002b950: 2072 6570 6c61 6365 206e 6569 6768 626f   replace neighbo
-0002b960: 7572 732c 2075 7365 202b 2069 6e73 7465  urs, use + inste
-0002b970: 6164 2e22 290a 2020 2020 2020 2020 2020  ad.").          
-0002b980: 2020 656c 6966 2063 686f 7264 5f69 6e74    elif chord_int
-0002b990: 6572 7661 6c20 3d3d 2036 2061 6e64 2066  erval == 6 and f
-0002b9a0: 6967 6261 7373 2021 3d20 2737 273a 2020  igbass != '7':  
-0002b9b0: 2320 3774 6820 6172 6520 6120 7370 6563  # 7th are a spec
-0002b9c0: 6961 6c20 6361 7365 3a0a 2020 2020 2020  ial case:.      
-0002b9d0: 2020 2020 2020 2020 2020 6966 2066 6967            if fig
-0002b9e0: 6261 7373 203d 3d20 2727 3a20 2023 2069  bass == '':  # i
-0002b9f0: 6e20 726f 6f74 2070 6f73 6974 696f 6e20  n root position 
-0002ba00: 7472 6961 6473 2074 6865 7920 6172 6520  triads they are 
-0002ba10: 6164 6465 640a 2020 2020 2020 2020 2020  added.          
-0002ba20: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
-0002ba30: 3a20 5468 6520 7374 616e 6461 7264 2069  : The standard i
-0002ba40: 7320 6c61 636b 696e 6720 6120 6469 7374  s lacking a dist
-0002ba50: 696e 6374 696f 6e2c 2062 6563 6175 7365  inction, because
-0002ba60: 2074 6865 2072 6f6f 7420 696e 2072 6f6f   the root in roo
-0002ba70: 7420 706f 732e 2063 616e 2061 6c73 6f20  t pos. can also 
-0002ba80: 6265 2072 6570 6c61 6365 6420 6672 6f6d  be replaced from
-0002ba90: 2062 656c 6f77 210a 2020 2020 2020 2020   below!.        
-0002baa0: 2020 2020 2020 2020 2020 2020 6164 6465              adde
-0002bab0: 645f 6e6f 7465 732e 6170 7065 6e64 286e  d_notes.append(n
-0002bac0: 6577 5f76 616c 290a 2020 2020 2020 2020  ew_val).        
-0002bad0: 2020 2020 2020 2020 656c 6966 2066 6967          elif fig
-0002bae0: 6261 7373 2069 6e20 5b27 3627 2c20 2736  bass in ['6', '6
-0002baf0: 3427 5d20 6f72 2027 2327 2069 6e20 6163  4'] or '#' in ac
-0002bb00: 633a 2020 2320 696e 2069 6e76 6572 7465  c:  # in inverte
-0002bb10: 6420 7472 6961 6473 2074 6865 7920 7265  d triads they re
-0002bb20: 706c 6163 6520 7468 6520 726f 6f74 2c20  place the root, 
-0002bb30: 6173 2064 6f65 7320 2337 0a20 2020 2020  as does #7.     
-0002bb40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0002bb50: 6570 6c61 6365 5f63 686f 7264 5f74 6f6e  eplace_chord_ton
-0002bb60: 6528 302c 206e 6577 5f76 616c 290a 2020  e(0, new_val).  
-0002bb70: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0002bb80: 7365 3a20 2023 206f 7468 6572 7769 7365  se:  # otherwise
-0002bb90: 2074 6865 7920 6172 6520 756e 636c 6561   they are unclea
-0002bba0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0002bbb0: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-0002bbc0: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
-0002bbd0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0002bbe0: 7b4d 437d 496e 2073 6576 656e 7468 2063  {MC}In seventh c
-0002bbf0: 686f 7264 732c 2073 7563 6820 6173 207b  hords, such as {
-0002bc00: 6c61 6265 6c7d 2c20 6974 2069 7320 6e6f  label}, it is no
-0002bc10: 7420 636c 6561 7220 7768 6574 6865 7220  t clear whether 
-0002bc20: 7468 6520 7b66 756c 6c7d 2061 6c74 6572  the {full} alter
-0002bc30: 7320 7468 6520 3720 6f72 2072 6570 6c61  s the 7 or repla
-0002bc40: 6365 7320 7468 6520 3820 616e 6420 7368  ces the 8 and sh
-0002bc50: 6f75 6c64 206e 6f74 2062 6520 7573 6564  ould not be used
-0002bc60: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-0002bc70: 2020 2020 2020 2020 2020 2020 6578 7472              extr
-0002bc80: 613d 7b22 6d65 7373 6167 655f 6964 223a  a={"message_id":
-0002bc90: 2028 3138 2c20 297d 290a 2020 2020 2020   (18, )}).      
-0002bca0: 2020 2020 2020 656c 6966 2074 7063 735b        elif tpcs[
-0002bcb0: 6368 6f72 645f 696e 7465 7276 616c 5d20  chord_interval] 
-0002bcc0: 3d3d 206e 6577 5f76 616c 3a0a 2020 2020  == new_val:.    
-0002bcd0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0002bce0: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
-0002bcf0: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-0002bd00: 4d43 7d54 6865 2063 6861 6e67 6520 7b66  MC}The change {f
-0002bd10: 756c 6c7d 2068 6173 206e 6f20 6566 6665  ull} has no effe
-0002bd20: 6374 2069 6e20 7b6e 756d 6572 616c 7d7b  ct in {numeral}{
-0002bd30: 666f 726d 7d7b 6669 6762 6173 737d 2229  form}{figbass}")
-0002bd40: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0002bd50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0002bd60: 2020 2072 6f6f 745f 706f 7369 7469 6f6e     root_position
-0002bd70: 5b63 686f 7264 5f69 6e74 6572 7661 6c5d  [chord_interval]
-0002bd80: 203d 205b 6e65 775f 7661 6c5d 0a0a 2020   = [new_val]..  
-0002bd90: 2020 6669 6762 6173 7332 6261 7373 203d    figbass2bass =
-0002bda0: 207b 0a20 2020 2020 2020 2027 273a 2030   {.        '': 0
-0002bdb0: 2c0a 2020 2020 2020 2020 2737 273a 2030  ,.        '7': 0
-0002bdc0: 2c0a 2020 2020 2020 2020 2736 273a 2031  ,.        '6': 1
-0002bdd0: 2c0a 2020 2020 2020 2020 2736 3527 3a20  ,.        '65': 
-0002bde0: 312c 0a20 2020 2020 2020 2027 3634 273a  1,.        '64':
-0002bdf0: 2032 2c0a 2020 2020 2020 2020 2734 3327   2,.        '43'
-0002be00: 3a20 322c 0a20 2020 2020 2020 2027 3227  : 2,.        '2'
-0002be10: 3a20 330a 2020 2020 7d0a 2020 2020 6261  : 3.    }.    ba
-0002be20: 7373 203d 2066 6967 6261 7373 3262 6173  ss = figbass2bas
-0002be30: 735b 6669 6762 6173 735d 0a20 2020 2063  s[figbass].    c
-0002be40: 686f 7264 5f74 6f6e 6573 203d 205b 5d0a  hord_tones = [].
-0002be50: 2020 2020 746f 6e65 5f66 756e 6374 696f      tone_functio
-0002be60: 6e5f 6e61 6d65 7320 3d20 7b0a 2020 2020  n_names = {.    
-0002be70: 2020 2020 303a 2027 726f 6f74 272c 0a20      0: 'root',. 
-0002be80: 2020 2020 2020 2032 3a20 2733 7264 272c         2: '3rd',
-0002be90: 0a20 2020 2020 2020 2034 3a20 2735 7468  .        4: '5th
-0002bea0: 272c 0a20 2020 2020 2020 2036 3a20 2737  ',.        6: '7
-0002beb0: 7468 272c 0a20 2020 207d 0a20 2020 2066  th',.    }.    f
-0002bec0: 6f72 2074 6620 696e 2074 6f6e 655f 6675  or tf in tone_fu
-0002bed0: 6e63 7469 6f6e 735b 6261 7373 3a5d 202b  nctions[bass:] +
-0002bee0: 2074 6f6e 655f 6675 6e63 7469 6f6e 735b   tone_functions[
-0002bef0: 3a62 6173 735d 3a0a 2020 2020 2020 2020  :bass]:.        
-0002bf00: 6368 6f72 645f 746f 6e65 2c20 7265 706c  chord_tone, repl
-0002bf10: 6163 696e 675f 746f 6e65 7320 3d20 726f  acing_tones = ro
-0002bf20: 6f74 5f70 6f73 6974 696f 6e5b 7466 5d2c  ot_position[tf],
-0002bf30: 2072 6570 6c61 6365 6d65 6e74 735b 7466   replacements[tf
-0002bf40: 5d0a 2020 2020 2020 2020 6966 2063 686f  ].        if cho
-0002bf50: 7264 5f74 6f6e 6520 3d3d 2072 6570 6c61  rd_tone == repla
-0002bf60: 6369 6e67 5f74 6f6e 6573 203d 3d20 5b5d  cing_tones == []
-0002bf70: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-0002bf80: 6767 6572 2e64 6562 7567 2866 227b 4d43  gger.debug(f"{MC
-0002bf90: 7d7b 6c61 6265 6c7d 2072 6573 756c 7473  }{label} results
-0002bfa0: 2069 6e20 6120 6368 6f72 6420 7769 7468   in a chord with
-0002bfb0: 6f75 7420 7b74 6f6e 655f 6675 6e63 7469  out {tone_functi
-0002bfc0: 6f6e 5f6e 616d 6573 5b74 665d 7d2e 2229  on_names[tf]}.")
-0002bfd0: 0a20 2020 2020 2020 2069 6620 6368 6f72  .        if chor
-0002bfe0: 645f 746f 6e65 2021 3d20 5b5d 3a0a 2020  d_tone != []:.  
-0002bff0: 2020 2020 2020 2020 2020 6368 6f72 645f            chord_
-0002c000: 746f 6e65 732e 6170 7065 6e64 2863 686f  tones.append(cho
-0002c010: 7264 5f74 6f6e 655b 305d 290a 2020 2020  rd_tone[0]).    
-0002c020: 2020 2020 2020 2020 6966 2072 6570 6c61          if repla
-0002c030: 6369 6e67 5f74 6f6e 6573 2021 3d20 5b5d  cing_tones != []
-0002c040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002c050: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
-0002c060: 2866 227b 4d43 7d7b 6c61 6265 6c7d 2072  (f"{MC}{label} r
-0002c070: 6573 756c 7473 2069 6e20 6120 6368 6f72  esults in a chor
-0002c080: 6420 746f 6e65 207b 746f 6e65 5f66 756e  d tone {tone_fun
-0002c090: 6374 696f 6e5f 6e61 6d65 735b 7466 5d7d  ction_names[tf]}
-0002c0a0: 2041 4e44 2069 7473 2072 6570 6c61 6365   AND its replace
-0002c0b0: 6d65 6e74 2873 2920 2854 5043 207b 7265  ment(s) (TPC {re
-0002c0c0: 706c 6163 696e 675f 746f 6e65 737d 292e  placing_tones}).
-0002c0d0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0002c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c0f0: 2020 6622 596f 7520 6d69 6768 7420 7761    f"You might wa
-0002c100: 6e74 2074 6f20 6164 6420 6120 2b20 746f  nt to add a + to
-0002c110: 2064 6973 7469 6e67 7569 7368 2066 726f   distinguish fro
-0002c120: 6d20 6120 7375 7370 656e 7369 6f6e 2c20  m a suspension, 
-0002c130: 6f72 2061 6464 2074 6869 7320 7761 726e  or add this warn
-0002c140: 696e 6720 746f 2049 474e 4f52 4544 5f57  ing to IGNORED_W
-0002c150: 4152 4e49 4e47 5320 7769 7468 2061 2063  ARNINGS with a c
-0002c160: 6f6d 6d65 6e74 2e22 2c0a 2020 2020 2020  omment.",.      
-0002c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c180: 2020 2020 2020 2020 2065 7874 7261 3d7b           extra={
-0002c190: 226d 6573 7361 6765 5f69 6422 3a20 2836  "message_id": (6
-0002c1a0: 2c20 6d63 2c20 6c61 6265 6c29 7d29 0a20  , mc, label)}). 
-0002c1b0: 2020 2020 2020 2063 686f 7264 5f74 6f6e         chord_ton
-0002c1c0: 6573 2e65 7874 656e 6428 7265 706c 6163  es.extend(replac
-0002c1d0: 696e 675f 746f 6e65 7329 0a0a 2020 2020  ing_tones)..    
-0002c1e0: 6261 7373 5f74 7063 203d 2063 686f 7264  bass_tpc = chord
-0002c1f0: 5f74 6f6e 6573 5b30 5d0a 2020 2020 6966  _tones[0].    if
-0002c200: 2062 6173 735f 6f6e 6c79 3a0a 2020 2020   bass_only:.    
-0002c210: 2020 2020 7265 7475 726e 2062 6173 735f      return bass_
-0002c220: 7470 630a 2020 2020 656c 6966 206d 6572  tpc.    elif mer
-0002c230: 6765 5f74 6f6e 6573 3a0a 2020 2020 2020  ge_tones:.      
-0002c240: 2020 7265 7475 726e 2074 7570 6c65 2873    return tuple(s
-0002c250: 6f72 745f 7470 6373 2863 686f 7264 5f74  ort_tpcs(chord_t
-0002c260: 6f6e 6573 202b 2061 6464 6564 5f6e 6f74  ones + added_not
-0002c270: 6573 2c20 7374 6172 743d 6261 7373 5f74  es, start=bass_t
-0002c280: 7063 2929 0a20 2020 2065 6c73 653a 0a20  pc)).    else:. 
-0002c290: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
-0002c2a0: 2020 2020 2020 2020 2020 2020 2763 686f              'cho
-0002c2b0: 7264 5f74 6f6e 6573 273a 2074 7570 6c65  rd_tones': tuple
-0002c2c0: 2863 686f 7264 5f74 6f6e 6573 292c 0a20  (chord_tones),. 
-0002c2d0: 2020 2020 2020 2020 2020 2027 6164 6465             'adde
-0002c2e0: 645f 746f 6e65 7327 3a20 7475 706c 6528  d_tones': tuple(
-0002c2f0: 6164 6465 645f 6e6f 7465 7329 2c0a 2020  added_notes),.  
-0002c300: 2020 2020 2020 2020 2020 2772 6f6f 7427            'root'
-0002c310: 3a20 726f 6f74 2c0a 2020 2020 2020 2020  : root,.        
-0002c320: 7d0a 0a64 6566 2070 6174 6832 7061 7265  }..def path2pare
-0002c330: 6e74 5f63 6f72 7075 7328 7061 7468 293a  nt_corpus(path):
-0002c340: 0a20 2020 2022 2222 5761 6c6b 2075 7020  .    """Walk up 
-0002c350: 7468 6520 7061 7468 2061 6e64 2072 6574  the path and ret
-0002c360: 7572 6e20 7468 6520 6e61 6d65 206f 6620  urn the name of 
-0002c370: 7468 6520 6669 7273 7420 7375 7065 7264  the first superd
-0002c380: 6972 6563 746f 7279 2074 6861 7420 6973  irectory that is
-0002c390: 2061 2067 6974 2072 6570 6f73 6974 6f72   a git repositor
-0002c3a0: 7920 6f72 2063 6f6e 7461 696e 7320 6120  y or contains a 
-0002c3b0: 276d 6574 6164 6174 612e 7473 7627 2066  'metadata.tsv' f
-0002c3c0: 696c 652e 2222 220a 2020 2020 6966 2070  ile.""".    if p
-0002c3d0: 6174 6820 696e 2028 2727 2c20 272f 2729  ath in ('', '/')
-0002c3e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0002c3f0: 204e 6f6e 650a 2020 2020 7472 793a 0a20   None.    try:. 
-0002c400: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-0002c410: 682e 6973 6469 7228 7061 7468 293a 0a20  h.isdir(path):. 
-0002c420: 2020 2020 2020 2020 2020 206c 6973 7464             listd
-0002c430: 6972 203d 206f 732e 6c69 7374 6469 7228  ir = os.listdir(
-0002c440: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
-0002c450: 2020 6966 2027 6d65 7461 6461 7461 2e74    if 'metadata.t
-0002c460: 7376 2720 696e 206c 6973 7464 6972 206f  sv' in listdir o
-0002c470: 7220 272e 6769 7427 2069 6e20 6c69 7374  r '.git' in list
-0002c480: 6469 723a 0a20 2020 2020 2020 2020 2020  dir:.           
-0002c490: 2020 2020 2072 6574 7572 6e20 7061 7468       return path
-0002c4a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002c4b0: 7061 7468 3270 6172 656e 745f 636f 7270  path2parent_corp
-0002c4c0: 7573 286f 732e 7061 7468 2e64 6972 6e61  us(os.path.dirna
-0002c4d0: 6d65 2870 6174 6829 290a 2020 2020 6578  me(path)).    ex
-0002c4e0: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
-0002c4f0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-0002c500: 6f6e 650a 0a0a 4066 756e 6374 696f 6e5f  one...@function_
-0002c510: 6c6f 6767 6572 0a64 6566 2063 686f 7264  logger.def chord
-0002c520: 3274 7063 7328 6368 6f72 642c 2072 6567  2tpcs(chord, reg
-0002c530: 6578 3d4e 6f6e 652c 202a 2a6b 7761 7267  ex=None, **kwarg
-0002c540: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
-0002c550: 5370 6c69 7420 6120 6368 6f72 6420 6c61  Split a chord la
-0002c560: 6265 6c20 696e 746f 2069 7473 2066 6561  bel into its fea
-0002c570: 7475 7265 7320 616e 6420 6170 706c 7920  tures and apply 
-0002c580: 6665 6174 7572 6573 3274 7063 7328 292e  features2tpcs().
-0002c590: 0a0a 2020 2020 5573 6573 3a20 6665 6174  ..    Uses: feat
-0002c5a0: 7572 6573 3274 7063 7328 290a 0a20 2020  ures2tpcs()..   
-0002c5b0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0002c5c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
-0002c5d0: 686f 7264 203a 203a 6f62 6a3a 6073 7472  hord : :obj:`str
-0002c5e0: 600a 2020 2020 2020 2020 4368 6f72 6420  `.        Chord 
-0002c5f0: 6c61 6265 6c20 7468 6174 2063 616e 2062  label that can b
-0002c600: 6520 7370 6c69 7420 696e 746f 2074 6865  e split into the
-0002c610: 2066 6561 7475 7265 7320 5b27 6e75 6d65   features ['nume
-0002c620: 7261 6c27 2c20 2766 6f72 6d27 2c20 2766  ral', 'form', 'f
-0002c630: 6967 6261 7373 272c 2027 6368 616e 6765  igbass', 'change
-0002c640: 7327 2c20 2772 656c 6174 6976 6572 6f6f  s', 'relativeroo
-0002c650: 7427 5d2e 0a20 2020 2072 6567 6578 203a  t']..    regex :
-0002c660: 203a 6f62 6a3a 6072 652e 5061 7474 6572   :obj:`re.Patter
-0002c670: 6e60 2c20 6f70 7469 6f6e 616c 0a20 2020  n`, optional.   
-0002c680: 2020 2020 2043 6f6d 7069 6c65 6420 7265       Compiled re
-0002c690: 6765 7820 7769 7468 206e 616d 6564 2067  gex with named g
-0002c6a0: 726f 7570 7320 666f 7220 7468 6520 6669  roups for the fi
-0002c6b0: 7665 2066 6561 7475 7265 732e 2042 7920  ve features. By 
-0002c6c0: 6465 6661 756c 742c 2074 6865 2063 7572  default, the cur
-0002c6d0: 7265 6e74 2076 6572 7369 6f6e 206f 6620  rent version of 
-0002c6e0: 7468 6520 4443 4d4c 2068 6172 6d6f 6e79  the DCML harmony
-0002c6f0: 0a20 2020 2020 2020 2061 6e6e 6f74 6174  .        annotat
-0002c700: 696f 6e20 7374 616e 6461 7264 2069 7320  ion standard is 
-0002c710: 7573 6564 2e0a 2020 2020 2a2a 6b77 6172  used..    **kwar
-0002c720: 6773 203a 0a20 2020 2020 2020 2061 7267  gs :.        arg
-0002c730: 756d 656e 7473 2066 6f72 2066 6561 7475  uments for featu
-0002c740: 7265 7332 7470 6373 2028 7061 7373 204d  res2tpcs (pass M
-0002c750: 4320 746f 2073 686f 7720 6974 2069 6e20  C to show it in 
-0002c760: 7761 726e 696e 6773 2129 0a20 2020 2022  warnings!).    "
-0002c770: 2222 0a20 2020 2069 6620 7265 6765 7820  "".    if regex 
-0002c780: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0002c790: 2072 6567 6578 203d 2044 434d 4c5f 5245   regex = DCML_RE
-0002c7a0: 4745 580a 2020 2020 6368 6f72 645f 6665  GEX.    chord_fe
-0002c7b0: 6174 7572 6573 203d 2072 652e 6d61 7463  atures = re.matc
-0002c7c0: 6828 7265 6765 782c 2063 686f 7264 290a  h(regex, chord).
-0002c7d0: 2020 2020 6173 7365 7274 2063 686f 7264      assert chord
-0002c7e0: 5f66 6561 7475 7265 7320 6973 206e 6f74  _features is not
-0002c7f0: 204e 6f6e 652c 2066 227b 6368 6f72 647d   None, f"{chord}
-0002c800: 2064 6f65 7320 6e6f 7420 6d61 7463 6820   does not match 
-0002c810: 7468 6520 7265 6765 782e 220a 2020 2020  the regex.".    
-0002c820: 6368 6f72 645f 6665 6174 7572 6573 203d  chord_features =
-0002c830: 2063 686f 7264 5f66 6561 7475 7265 732e   chord_features.
-0002c840: 6772 6f75 7064 6963 7428 290a 2020 2020  groupdict().    
-0002c850: 6e75 6d65 7261 6c2c 2066 6f72 6d2c 2066  numeral, form, f
-0002c860: 6967 6261 7373 2c20 6368 616e 6765 732c  igbass, changes,
-0002c870: 2072 656c 6174 6976 6572 6f6f 7420 3d20   relativeroot = 
-0002c880: 7475 706c 6528 6368 6f72 645f 6665 6174  tuple(chord_feat
-0002c890: 7572 6573 5b66 5d20 666f 7220 6620 696e  ures[f] for f in
-0002c8a0: 2028 276e 756d 6572 616c 272c 2027 666f   ('numeral', 'fo
-0002c8b0: 726d 272c 2027 6669 6762 6173 7327 2c20  rm', 'figbass', 
-0002c8c0: 2763 6861 6e67 6573 272c 2027 7265 6c61  'changes', 'rela
-0002c8d0: 7469 7665 726f 6f74 2729 290a 2020 2020  tiveroot')).    
-0002c8e0: 7265 7475 726e 2066 6561 7475 7265 7332  return features2
-0002c8f0: 7470 6373 286e 756d 6572 616c 3d6e 756d  tpcs(numeral=num
-0002c900: 6572 616c 2c20 666f 726d 3d66 6f72 6d2c  eral, form=form,
-0002c910: 2066 6967 6261 7373 3d66 6967 6261 7373   figbass=figbass
-0002c920: 2c20 6368 616e 6765 733d 6368 616e 6765  , changes=change
-0002c930: 732c 2072 656c 6174 6976 6572 6f6f 743d  s, relativeroot=
-0002c940: 7265 6c61 7469 7665 726f 6f74 2c0a 2020  relativeroot,.  
-0002c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c960: 2020 2020 2020 206c 6f67 6765 723d 6c6f         logger=lo
-0002c970: 6767 6572 2c20 2a2a 6b77 6172 6773 290a  gger, **kwargs).
-0002c980: 0a0a 6465 6620 7472 616e 7370 6f73 6528  ..def transpose(
-0002c990: 652c 206e 293a 0a20 2020 2022 2222 2041  e, n):.    """ A
-0002c9a0: 6464 2060 6e60 2074 6f20 616c 6c20 656c  dd `n` to all el
-0002c9b0: 656d 656e 7473 2060 6560 2072 6563 7572  ements `e` recur
-0002c9c0: 7369 7665 6c79 2e0a 2020 2020 2222 220a  sively..    """.
-0002c9d0: 2020 2020 7265 7475 726e 206d 6170 3265      return map2e
-0002c9e0: 6c65 6d65 6e74 7328 652c 206c 616d 6264  lements(e, lambd
-0002c9f0: 6120 783a 2078 202b 206e 290a 0a0a 6465  a x: x + n)...de
-0002ca00: 6620 7061 7273 655f 6967 6e6f 7265 645f  f parse_ignored_
-0002ca10: 7761 726e 696e 6773 286d 6573 7361 6765  warnings(message
-0002ca20: 733a 2043 6f6c 6c65 6374 696f 6e5b 7374  s: Collection[st
-0002ca30: 725d 2920 2d3e 2049 7465 7261 746f 725b  r]) -> Iterator[
-0002ca40: 5475 706c 655b 7374 722c 2054 7570 6c65  Tuple[str, Tuple
-0002ca50: 5b69 6e74 5d5d 5d3a 0a20 2020 2022 2222  [int]]]:.    """
-0002ca60: 5475 726e 7320 6120 6c69 7374 206f 6620  Turns a list of 
-0002ca70: 6c6f 6720 6d65 7373 6167 6573 2069 6e74  log messages int
-0002ca80: 6f20 616e 2069 7465 7261 746f 7220 6f66  o an iterator of
-0002ca90: 2028 6c6f 6767 6572 5f6e 616d 652c 2028   (logger_name, (
-0002caa0: 6d65 7373 6167 655f 696e 666f 2c20 2e2e  message_info, ..
-0002cab0: 2e29 2920 7061 6972 732e 0a20 2020 204c  .)) pairs..    L
-0002cac0: 6f67 206d 6573 7361 6765 7320 636f 6e73  og messages cons
-0002cad0: 6973 7420 6f66 2061 2068 6561 6465 7220  ist of a header 
-0002cae0: 6f66 2074 6865 2073 6861 7065 2057 4152  of the shape WAR
-0002caf0: 4e49 4e47 5f45 4e55 4d5f 4d45 4d42 4552  NING_ENUM_MEMBER
-0002cb00: 2028 656e 756d 5f76 616c 7565 2c20 5b6d   (enum_value, [m
-0002cb10: 632c 206d 6f72 655f 696e 666f 2e2e 2e5d  c, more_info...]
-0002cb20: 2920 6d73 332e 2850 6172 7365 7c43 6f72  ) ms3.(Parse|Cor
-0002cb30: 7075 7329 2e63 6f72 7075 732e 666e 616d  pus).corpus.fnam
-0002cb40: 6520 5b2d 2d20 706f 7465 6e74 6961 6c6c  e [-- potentiall
-0002cb50: 7920 6d6f 7265 2c20 6972 7265 6c65 7661  y more, irreleva
-0002cb60: 6e74 2073 7475 6666 5d2e 0a20 2020 2054  nt stuff]..    T
-0002cb70: 6865 2068 6561 6465 7220 6d69 6768 7420  he header might 
-0002cb80: 6265 2066 6f6c 6c6f 7765 6420 6279 2073  be followed by s
-0002cb90: 6576 6572 616c 206c 696e 6573 206f 6620  everal lines of 
-0002cba0: 636f 6d6d 656e 7473 2c20 6561 6368 2062  comments, each b
-0002cbb0: 6567 696e 6e69 6e67 2077 6974 6820 6120  eginning with a 
-0002cbc0: 7370 6163 6520 6f72 2074 6162 2e0a 2020  space or tab..  
-0002cbd0: 2020 2222 220a 2020 2020 6966 2069 7369    """.    if isi
-0002cbe0: 6e73 7461 6e63 6528 6d65 7373 6167 6573  nstance(messages
-0002cbf0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-0002cc00: 7969 656c 6420 6672 6f6d 2070 6172 7365  yield from parse
-0002cc10: 5f69 676e 6f72 6564 5f77 6172 6e69 6e67  _ignored_warning
-0002cc20: 7328 5b6d 6573 7361 6765 735d 290a 2020  s([messages]).  
-0002cc30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002cc40: 666f 7220 6d65 7373 6167 6520 696e 206d  for message in m
-0002cc50: 6573 7361 6765 733a 0a20 2020 2020 2020  essages:.       
-0002cc60: 2020 2020 2069 6620 275c 6e27 2069 6e20       if '\n' in 
-0002cc70: 6d65 7373 6167 653a 0a20 2020 2020 2020  message:.       
-0002cc80: 2020 2020 2020 2020 2079 6965 6c64 2066           yield f
-0002cc90: 726f 6d20 7061 7273 655f 6967 6e6f 7265  rom parse_ignore
-0002cca0: 645f 7761 726e 696e 6773 286d 6573 7361  d_warnings(messa
-0002ccb0: 6765 2e73 706c 6974 2827 5c6e 2729 290a  ge.split('\n')).
-0002ccc0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0002ccd0: 206d 6573 7361 6765 203d 3d20 2727 3a0a   message == '':.
-0002cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ccf0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0002cd00: 2020 2020 2065 6c69 6620 6d65 7373 6167       elif messag
-0002cd10: 655b 305d 2069 6e20 2827 2027 2c20 275c  e[0] in (' ', '\
-0002cd20: 7427 2c20 2723 2729 3a0a 2020 2020 2020  t', '#'):.      
-0002cd30: 2020 2020 2020 2020 2020 2320 6966 2073            # if s
-0002cd40: 6576 6572 616c 206c 696e 6573 206f 6620  everal lines of 
-0002cd50: 6120 7761 726e 696e 6720 7765 7265 2063  a warning were c
-0002cd60: 6f70 6965 642c 2075 7365 206f 6e6c 7920  opied, use only 
-0002cd70: 7468 6520 6669 7273 7420 6f6e 650a 2020  the first one.  
-0002cd80: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0002cd90: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-0002cda0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0002cdb0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-0002cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cdd0: 2020 2320 6966 2074 6865 2061 6e6e 6f74    # if the annot
-0002cde0: 6174 6f72 2063 6f70 6965 6420 746f 6f20  ator copied too 
-0002cdf0: 6d75 6368 2c20 6375 7420 6f66 6620 7468  much, cut off th
-0002ce00: 6520 7265 6475 6e64 616e 7420 696e 666f  e redundant info
-0002ce10: 726d 6174 696f 6e20 6174 2074 6865 2065  rmation at the e
-0002ce20: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-0002ce30: 2020 2020 2020 2072 6564 756e 6461 6e74         redundant
-0002ce40: 203d 2020 6d65 7373 6167 652e 696e 6465   =  message.inde
-0002ce50: 7828 2720 2d2d 2027 290a 2020 2020 2020  x(' -- ').      
-0002ce60: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0002ce70: 7373 6167 6520 3d20 6d65 7373 6167 655b  ssage = message[
-0002ce80: 3a72 6564 756e 6461 6e74 5d0a 2020 2020  :redundant].    
-0002ce90: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0002cea0: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
-0002ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cec0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-0002ced0: 2020 2020 2020 2020 6d65 7373 6167 6520          message 
-0002cee0: 3d20 6d65 7373 6167 652e 7374 7269 7028  = message.strip(
-0002cef0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002cf00: 2020 7370 6c69 745f 7265 203d 2072 225e    split_re = r"^
-0002cf10: 282e 2a29 2028 5c53 2b29 2422 0a20 2020  (.*) (\S+)$".   
-0002cf20: 2020 2020 2020 2020 2020 2020 2074 7279               try
-0002cf30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002cf40: 2020 2020 2020 6d73 672c 206c 6f67 6765        msg, logge
-0002cf50: 725f 6e61 6d65 203d 2072 652e 6d61 7463  r_name = re.matc
-0002cf60: 6828 7370 6c69 745f 7265 2c20 6d65 7373  h(split_re, mess
-0002cf70: 6167 6529 2e67 726f 7570 7328 290a 2020  age).groups().  
-0002cf80: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-0002cf90: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
-0002cfa0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-0002cfb0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-0002cfc0: 2254 6865 2066 6f6c 6c6f 7769 6e67 206d  "The following m
-0002cfd0: 6573 7361 6765 2063 6f75 6c64 206e 6f74  essage could not
-0002cfe0: 2062 6520 7370 6c69 742c 2061 7070 6172   be split, appar
-0002cff0: 656e 746c 7920 6974 2064 6f65 7320 6e6f  ently it does no
-0002d000: 7420 656e 6420 7769 7468 2074 6865 206c  t end with the l
-0002d010: 6f67 6765 725f 6e61 6d65 3a20 7b6d 6573  ogger_name: {mes
-0002d020: 7361 6765 7d22 290a 2020 2020 2020 2020  sage}").        
-0002d030: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0002d040: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0002d050: 2020 6966 206d 7367 5b2d 315d 2021 3d20    if msg[-1] != 
-0002d060: 2729 273a 0a20 2020 2020 2020 2020 2020  ')':.           
-0002d070: 2020 2020 2020 2020 2069 6620 616e 7928           if any(
-0002d080: 6d73 672e 7374 6172 7473 7769 7468 286c  msg.startswith(l
-0002d090: 6576 656c 2920 666f 7220 6c65 7665 6c20  evel) for level 
-0002d0a0: 696e 2028 2744 4542 5547 272c 2027 494e  in ('DEBUG', 'IN
-0002d0b0: 464f 272c 2027 5741 524e 494e 4727 2c20  FO', 'WARNING', 
-0002d0c0: 2745 5252 4f52 272c 2027 4352 4954 4943  'ERROR', 'CRITIC
-0002d0d0: 414c 2729 293a 0a20 2020 2020 2020 2020  AL')):.         
-0002d0e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0002d0f0: 206d 6573 7361 6765 5f69 6420 6861 7320   message_id has 
-0002d100: 6e6f 7420 2879 6574 2920 7370 6563 6966  not (yet) specif
-0002d110: 6965 6420 666f 7220 7468 6973 206c 6f67  ied for this log
-0002d120: 206d 6573 7361 6765 2061 6e64 2069 7320   message and is 
-0002d130: 6967 6e6f 7265 643b 0a20 2020 2020 2020  ignored;.       
-0002d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d150: 2023 2061 2077 6172 6e69 6e67 2063 6f75   # a warning cou
-0002d160: 6c64 2062 6520 696d 706c 656d 656e 7465  ld be implemente
-0002d170: 6420 6174 2074 6869 7320 706f 696e 740a  d at this point.
-0002d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d190: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0002d1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002d1b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0002d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d1d0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0002d1e0: 726f 7228 6622 556e 6578 7065 6374 6564  ror(f"Unexpected
-0002d1f0: 206c 6f67 206d 6573 7361 6765 2066 6f72   log message for
-0002d200: 6d61 743a 207b 6d73 677d 2229 0a20 2020  mat: {msg}").   
-0002d210: 2020 2020 2020 2020 2020 2020 2074 7570               tup
-0002d220: 6c65 5f73 7461 7274 203d 206d 7367 2e69  le_start = msg.i
-0002d230: 6e64 6578 2827 2827 2920 2b20 310a 2020  ndex('(') + 1.  
-0002d240: 2020 2020 2020 2020 2020 2020 2020 7475                tu
-0002d250: 706c 655f 7374 7220 3d20 6d73 675b 7475  ple_str = msg[tu
-0002d260: 706c 655f 7374 6172 743a 2d31 5d0a 2020  ple_start:-1].  
-0002d270: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0002d280: 666f 203d 2073 7472 3269 6e74 7475 706c  fo = str2inttupl
-0002d290: 6528 7475 706c 655f 7374 722c 2073 7472  e(tuple_str, str
-0002d2a0: 6963 743d 4661 6c73 6529 0a20 2020 2020  ict=False).     
-0002d2b0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-0002d2c0: 206c 6f67 6765 725f 6e61 6d65 2c20 696e   logger_name, in
-0002d2d0: 666f 0a0a 6465 6620 6967 6e6f 7265 645f  fo..def ignored_
-0002d2e0: 7761 726e 696e 6773 3264 6963 7428 6d65  warnings2dict(me
-0002d2f0: 7373 6167 6573 3a20 436f 6c6c 6563 7469  ssages: Collecti
-0002d300: 6f6e 5b73 7472 5d29 202d 3e20 4469 6374  on[str]) -> Dict
-0002d310: 5b73 7472 2c20 4c69 7374 5b54 7570 6c65  [str, List[Tuple
-0002d320: 5b69 6e74 5d5d 5d3a 0a20 2020 2022 2222  [int]]]:.    """
-0002d330: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-0002d340: 2020 6d65 7373 6167 6573 3a0a 0a20 2020    messages:..   
-0002d350: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0002d360: 7b6c 6f67 6765 725f 6e61 6d65 202d 3e20  {logger_name -> 
-0002d370: 5b69 676e 6f72 6564 5f77 6172 6e69 6e67  [ignored_warning
-0002d380: 735d 7d20 6469 6374 2e0a 2020 2020 2222  s]} dict..    ""
-0002d390: 220a 2020 2020 6967 6e6f 7265 645f 7761  ".    ignored_wa
-0002d3a0: 726e 696e 6773 203d 2064 6566 6175 6c74  rnings = default
-0002d3b0: 6469 6374 286c 6973 7429 0a20 2020 2066  dict(list).    f
-0002d3c0: 6f72 206c 6f67 6765 725f 6e61 6d65 2c20  or logger_name, 
-0002d3d0: 696e 666f 2069 6e20 7061 7273 655f 6967  info in parse_ig
-0002d3e0: 6e6f 7265 645f 7761 726e 696e 6773 286d  nored_warnings(m
-0002d3f0: 6573 7361 6765 7329 3a0a 2020 2020 2020  essages):.      
-0002d400: 2020 6967 6e6f 7265 645f 7761 726e 696e    ignored_warnin
-0002d410: 6773 5b6c 6f67 6765 725f 6e61 6d65 5d2e  gs[logger_name].
-0002d420: 6170 7065 6e64 2869 6e66 6f29 0a20 2020  append(info).   
-0002d430: 2072 6574 7572 6e20 6469 6374 2869 676e   return dict(ign
-0002d440: 6f72 6564 5f77 6172 6e69 6e67 7329 0a0a  ored_warnings)..
-0002d450: 6465 6620 7061 7273 655f 6967 6e6f 7265  def parse_ignore
-0002d460: 645f 7761 726e 696e 6773 5f66 696c 6528  d_warnings_file(
-0002d470: 7061 7468 3a20 7374 7229 202d 3e20 4469  path: str) -> Di
-0002d480: 6374 5b73 7472 2c20 4c69 7374 5b54 7570  ct[str, List[Tup
-0002d490: 6c65 5b69 6e74 2c20 5475 706c 655b 696e  le[int, Tuple[in
-0002d4a0: 745d 5d5d 5d3a 0a20 2020 2022 2222 5061  t]]]]:.    """Pa
-0002d4b0: 7273 6520 6669 6c65 2077 6974 6820 6c6f  rse file with lo
-0002d4c0: 6720 6d65 7373 6167 6573 2074 6861 7420  g messages that 
-0002d4d0: 6861 7665 2074 6f20 6265 2069 676e 6f72  have to be ignor
-0002d4e0: 6564 2074 6f20 7468 6520 6469 6374 2e0a  ed to the dict..
-0002d4f0: 2020 2020 5468 6520 6578 7065 6374 6564      The expected
-0002d500: 2073 7472 7563 7475 7265 206f 6620 6d65   structure of me
-0002d510: 7373 6167 653a 2077 6172 6e69 6e67 5f74  ssage: warning_t
-0002d520: 7970 6520 2877 6172 6e69 6e67 5f74 7970  ype (warning_typ
-0002d530: 655f 6964 2c20 2a69 6e74 6567 6572 7329  e_id, *integers)
-0002d540: 2066 696c 650a 2020 2020 4578 616d 706c   file.    Exampl
-0002d550: 6520 6f66 206d 6573 7361 6765 3a20 494e  e of message: IN
-0002d560: 434f 5252 4543 545f 564f 4c54 415f 4d4e  CORRECT_VOLTA_MN
-0002d570: 5f57 4152 4e49 4e47 2028 322c 2039 3429  _WARNING (2, 94)
-0002d580: 206d 7333 2e50 6172 7365 2e6d 6978 6564   ms3.Parse.mixed
-0002d590: 5f66 696c 6573 2e44 6964 3033 4d2d 536f  _files.Did03M-So
-0002d5a0: 6e5f 7265 6769 6e61 2d31 3736 322d 5361  n_regina-1762-Sa
-0002d5b0: 7274 692e 6d73 6378 2e4d 6561 7375 7265  rti.mscx.Measure
-0002d5c0: 4c69 7374 0a0a 2020 2020 5061 7261 6d65  List..    Parame
-0002d5d0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0002d5e0: 2d2d 2d0a 2020 2020 6b65 7920 3a20 3a6f  ---.    key : :o
-0002d5f0: 626a 3a60 7374 7260 0a20 2020 2020 2020  bj:`str`.       
-0002d600: 207c 2050 6174 6820 746f 2049 474e 4f52   | Path to IGNOR
-0002d610: 4544 5f57 4152 4e49 4e47 530a 0a20 2020  ED_WARNINGS..   
-0002d620: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-0002d630: 2d2d 2d2d 0a20 2020 203a 6f62 6a3a 2064  ----.    :obj: d
-0002d640: 6963 740a 2020 2020 2020 2020 7b6c 6f67  ict.        {log
-0002d650: 6765 725f 6e61 6d65 3a20 5b28 6d65 7373  ger_name: [(mess
-0002d660: 6167 655f 6964 2c20 6c61 6265 6c5f 6f66  age_id, label_of
-0002d670: 5f6d 6573 7361 6765 292c 2028 6d65 7373  _message), (mess
-0002d680: 6167 655f 6964 2c20 6c61 6265 6c5f 6f66  age_id, label_of
-0002d690: 5f6d 6573 7361 6765 292c 202e 2e2e 5d7d  _message), ...]}
-0002d6a0: 2e0a 2020 2020 2222 220a 2020 2020 7061  ..    """.    pa
-0002d6b0: 7468 203d 2072 6573 6f6c 7665 5f64 6972  th = resolve_dir
-0002d6c0: 2870 6174 6829 0a20 2020 206d 6573 7361  (path).    messa
-0002d6d0: 6765 7320 3d20 6f70 656e 2870 6174 682c  ges = open(path,
-0002d6e0: 2027 7227 2c20 656e 636f 6469 6e67 3d27   'r', encoding='
-0002d6f0: 7574 662d 3827 292e 7265 6164 6c69 6e65  utf-8').readline
-0002d700: 7328 290a 2020 2020 7265 7475 726e 2069  s().    return i
-0002d710: 676e 6f72 6564 5f77 6172 6e69 6e67 7332  gnored_warnings2
-0002d720: 6469 6374 286d 6573 7361 6765 7329 0a0a  dict(messages)..
-0002d730: 0a64 6566 206f 7665 726c 6170 7069 6e67  .def overlapping
-0002d740: 5f63 6875 6e6b 5f70 6572 5f69 6e74 6572  _chunk_per_inter
-0002d750: 7661 6c28 6466 3a20 7064 2e44 6174 6146  val(df: pd.DataF
-0002d760: 7261 6d65 2c0a 2020 2020 2020 2020 2020  rame,.          
-0002d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d780: 2020 2020 2020 2020 2069 6e74 6572 7661           interva
-0002d790: 6c73 3a20 4c69 7374 5b70 642e 496e 7465  ls: List[pd.Inte
-0002d7a0: 7276 616c 5d2c 0a20 2020 2020 2020 2020  rval],.         
+00026c30: 2020 2020 2020 5b30 2c20 302c 2031 2c20        [0, 0, 1, 
+00026c40: 302c 2030 2c20 312c 2031 5d2c 0a20 2020  0, 0, 1, 1],.   
+00026c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026c70: 2020 2020 2020 2020 2020 5b30 2c20 312c            [0, 1,
+00026c80: 2031 2c20 302c 2031 2c20 312c 2031 5d5d   1, 0, 1, 1, 1]]
+00026c90: 290a 2020 2020 7265 6c61 7469 7665 5f61  ).    relative_a
+00026ca0: 6363 6964 656e 7461 6c73 2c20 7265 6c61  ccidentals, rela
+00026cb0: 7469 7665 203d 2073 706c 6974 5f73 6361  tive = split_sca
+00026cc0: 6c65 5f64 6567 7265 6528 7265 6c61 7469  le_degree(relati
+00026cd0: 7665 2c20 636f 756e 743d 5472 7565 2c20  ve, count=True, 
+00026ce0: 6c6f 6767 6572 3d6c 6f67 6765 7229 0a20  logger=logger). 
+00026cf0: 2020 206c 6f63 616c 6b65 795f 6163 6369     localkey_acci
+00026d00: 6465 6e74 616c 732c 206c 6f63 616c 6b65  dentals, localke
+00026d10: 7920 3d20 7370 6c69 745f 7363 616c 655f  y = split_scale_
+00026d20: 6465 6772 6565 286c 6f63 616c 6b65 792c  degree(localkey,
+00026d30: 2063 6f75 6e74 3d54 7275 652c 206c 6f67   count=True, log
+00026d40: 6765 723d 6c6f 6767 6572 290a 2020 2020  ger=logger).    
+00026d50: 7265 7375 6c74 696e 675f 6163 6369 6465  resulting_accide
+00026d60: 6e74 616c 7320 3d20 7265 6c61 7469 7665  ntals = relative
+00026d70: 5f61 6363 6964 656e 7461 6c73 202b 206c  _accidentals + l
+00026d80: 6f63 616c 6b65 795f 6163 6369 6465 6e74  ocalkey_accident
+00026d90: 616c 730a 2020 2020 6e75 6d65 7261 6c73  als.    numerals
+00026da0: 203d 206d 616a 5f72 6e20 6966 2072 656c   = maj_rn if rel
+00026db0: 6174 6976 652e 6973 7570 7065 7228 2920  ative.isupper() 
+00026dc0: 656c 7365 206d 696e 5f72 6e0a 2020 2020  else min_rn.    
+00026dd0: 7265 6c5f 6e75 6d20 3d20 6e75 6d65 7261  rel_num = numera
+00026de0: 6c73 2e69 6e64 6578 2872 656c 6174 6976  ls.index(relativ
+00026df0: 6529 0a20 2020 206c 6f63 616c 6b65 795f  e).    localkey_
+00026e00: 696e 6465 7820 3d20 6d61 6a5f 726e 2e69  index = maj_rn.i
+00026e10: 6e64 6578 286c 6f63 616c 6b65 792e 7570  ndex(localkey.up
+00026e20: 7065 7228 2929 0a20 2020 2072 6573 756c  per()).    resul
+00026e30: 745f 6e75 6d65 7261 6c20 3d20 6e75 6d65  t_numeral = nume
+00026e40: 7261 6c73 5b28 7265 6c5f 6e75 6d20 2b20  rals[(rel_num + 
+00026e50: 6c6f 6361 6c6b 6579 5f69 6e64 6578 2920  localkey_index) 
+00026e60: 2520 375d 0a20 2020 2069 6620 6c6f 6361  % 7].    if loca
+00026e70: 6c6b 6579 2e69 736c 6f77 6572 2829 2061  lkey.islower() a
+00026e80: 6e64 2072 656c 5f6e 756d 2069 6e20 5b32  nd rel_num in [2
+00026e90: 2c20 352c 2036 5d3a 0a20 2020 2020 2020  , 5, 6]:.       
+00026ea0: 2072 6573 756c 7469 6e67 5f61 6363 6964   resulting_accid
+00026eb0: 656e 7461 6c73 202d 3d20 310a 2020 2020  entals -= 1.    
+00026ec0: 6966 2067 6c6f 6261 6c5f 6d69 6e6f 723a  if global_minor:
+00026ed0: 0a20 2020 2020 2020 206c 6f63 616c 6b65  .        localke
+00026ee0: 795f 696e 6465 7820 3d20 286c 6f63 616c  y_index = (local
+00026ef0: 6b65 795f 696e 6465 7820 2d20 3229 2025  key_index - 2) %
+00026f00: 2037 0a20 2020 2072 6573 756c 7469 6e67   7.    resulting
+00026f10: 5f61 6363 6964 656e 7461 6c73 202b 3d20  _accidentals += 
+00026f20: 7768 6974 655f 6b65 795f 6d61 6a6f 725f  white_key_major_
+00026f30: 6163 6369 6465 6e74 616c 735b 7265 6c5f  accidentals[rel_
+00026f40: 6e75 6d5d 5b6c 6f63 616c 6b65 795f 696e  num][localkey_in
+00026f50: 6465 785d 0a20 2020 2061 6363 203d 2072  dex].    acc = r
+00026f60: 6573 756c 7469 6e67 5f61 6363 6964 656e  esulting_acciden
+00026f70: 7461 6c73 202a 2027 2327 2069 6620 7265  tals * '#' if re
+00026f80: 7375 6c74 696e 675f 6163 6369 6465 6e74  sulting_accident
+00026f90: 616c 7320 3e20 3020 656c 7365 202d 7265  als > 0 else -re
+00026fa0: 7375 6c74 696e 675f 6163 6369 6465 6e74  sulting_accident
+00026fb0: 616c 7320 2a20 2762 270a 2020 2020 7265  als * 'b'.    re
+00026fc0: 7475 726e 2061 6363 202b 2072 6573 756c  turn acc + resul
+00026fd0: 745f 6e75 6d65 7261 6c0a 0a0a 4066 756e  t_numeral...@fun
+00026fe0: 6374 696f 6e5f 6c6f 6767 6572 0a64 6566  ction_logger.def
+00026ff0: 206d 616b 655f 696e 7465 7276 616c 5f69   make_interval_i
+00027000: 6e64 6578 5f66 726f 6d5f 6475 7261 7469  ndex_from_durati
+00027010: 6f6e 7328 6466 2c20 706f 7369 7469 6f6e  ons(df, position
+00027020: 5f63 6f6c 3d27 7175 6172 7465 7262 6561  _col='quarterbea
+00027030: 7473 272c 2064 7572 6174 696f 6e5f 636f  ts', duration_co
+00027040: 6c3d 2764 7572 6174 696f 6e5f 7162 272c  l='duration_qb',
+00027050: 2063 6c6f 7365 643d 276c 6566 7427 2c0a   closed='left',.
+00027060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027070: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00027080: 6f75 6e64 3d4e 6f6e 652c 206e 616d 653d  ound=None, name=
+00027090: 2769 6e74 6572 7661 6c27 293a 0a20 2020  'interval'):.   
+000270a0: 2022 2222 4769 7665 6e20 616e 2061 6e6e   """Given an ann
+000270b0: 6f74 6174 696f 6e73 2074 6162 6c65 2077  otations table w
+000270c0: 6974 6820 706f 7369 7469 6f6e 7320 616e  ith positions an
+000270d0: 6420 6475 7261 7469 6f6e 732c 2063 7265  d durations, cre
+000270e0: 6174 6520 616e 203a 6f62 6a3a 6070 616e  ate an :obj:`pan
+000270f0: 6461 732e 496e 7465 7276 616c 496e 6465  das.IntervalInde
+00027100: 7860 2e0a 2020 2020 5265 7475 726e 7320  x`..    Returns 
+00027110: 4e6f 6e65 2069 6620 616e 7920 726f 7720  None if any row 
+00027120: 6973 2075 6e64 6572 7370 6563 6966 6965  is underspecifie
+00027130: 642e 0a0a 2020 2020 5061 7261 6d65 7465  d...    Paramete
+00027140: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00027150: 2d0a 2020 2020 6466 203a 203a 6f62 6a3a  -.    df : :obj:
+00027160: 6070 616e 6461 732e 4461 7461 4672 616d  `pandas.DataFram
+00027170: 6560 0a20 2020 2020 2020 2041 6e6e 6f74  e`.        Annot
+00027180: 6174 696f 6e20 7461 626c 6520 636f 6e74  ation table cont
+00027190: 6169 6e69 6e67 2074 6865 2063 6f6c 756d  aining the colum
+000271a0: 6e73 206f 6620 6060 706f 7369 7469 6f6e  ns of ``position
+000271b0: 5f63 6f6c 6060 2028 6465 6661 756c 743a  _col`` (default:
+000271c0: 2027 7175 6172 7465 7262 6561 7473 2729   'quarterbeats')
+000271d0: 2061 6e64 2060 6064 7572 6174 696f 6e5f   and ``duration_
+000271e0: 636f 6c60 600a 2020 2020 2020 2020 6465  col``.        de
+000271f0: 6661 756c 743a 2027 6475 7261 7469 6f6e  fault: 'duration
+00027200: 5f71 6227 292e 0a20 2020 2070 6f73 6974  _qb')..    posit
+00027210: 696f 6e5f 636f 6c20 3a20 3a6f 626a 3a60  ion_col : :obj:`
+00027220: 7374 7260 2c20 6f70 7469 6f6e 616c 0a20  str`, optional. 
+00027230: 2020 2020 2020 204e 616d 6520 6f66 2074         Name of t
+00027240: 6865 2063 6f6c 756d 6e20 636f 6e74 6169  he column contai
+00027250: 6e69 6e67 2070 6f73 6974 696f 6e73 2c20  ning positions, 
+00027260: 7573 6564 2061 7320 6c65 6674 2062 6f75  used as left bou
+00027270: 6e64 6172 6965 732e 0a20 2020 2064 7572  ndaries..    dur
+00027280: 6174 696f 6e5f 636f 6c20 3a20 3a6f 626a  ation_col : :obj
+00027290: 3a60 7374 7260 2c20 6f70 7469 6f6e 616c  :`str`, optional
+000272a0: 0a20 2020 2020 2020 204e 616d 6520 6f66  .        Name of
+000272b0: 2074 6865 2063 6f6c 756d 6e20 636f 6e74   the column cont
+000272c0: 6169 6e69 6e67 2064 7572 6174 696f 6e73  aining durations
+000272d0: 2077 6869 6368 2077 696c 6c20 6265 2061   which will be a
+000272e0: 6464 6564 2074 6f20 7468 6520 706f 7369  dded to the posi
+000272f0: 7469 6f6e 7320 746f 206f 6274 6169 6e20  tions to obtain 
+00027300: 7269 6768 7420 626f 756e 6461 7269 6573  right boundaries
+00027310: 2e0a 2020 2020 636c 6f73 6564 203a 203a  ..    closed : :
+00027320: 6f62 6a3a 6073 7472 602c 206f 7074 696f  obj:`str`, optio
+00027330: 6e61 6c0a 2020 2020 2020 2020 276c 6566  nal.        'lef
+00027340: 7427 2c20 2772 6967 6874 2720 6f72 2027  t', 'right' or '
+00027350: 626f 7468 2720 3c2d 2064 6566 696e 696e  both' <- definin
+00027360: 6720 7468 6520 696e 7465 7276 616c 2062  g the interval b
+00027370: 6f75 6e64 6172 6965 730a 2020 2020 726f  oundaries.    ro
+00027380: 756e 6420 3a20 3a6f 626a 3a60 696e 7460  und : :obj:`int`
+00027390: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+000273a0: 2020 2054 6f20 686f 7720 6d61 6e79 2064     To how many d
+000273b0: 6563 696d 616c 2070 6c61 6365 7320 746f  ecimal places to
+000273c0: 2072 6f75 6e64 2074 6865 2069 6e74 6572   round the inter
+000273d0: 7661 6c73 2720 626f 756e 6461 7279 2076  vals' boundary v
+000273e0: 616c 7565 732e 0a20 2020 206e 616d 6520  alues..    name 
+000273f0: 3a20 3a6f 626a 3a60 7374 7260 2c20 6f70  : :obj:`str`, op
+00027400: 7469 6f6e 616c 0a20 2020 2020 2020 204e  tional.        N
+00027410: 616d 6520 6f66 2074 6865 2063 7265 6174  ame of the creat
+00027420: 6564 2069 6e64 6578 2e20 4465 6661 756c  ed index. Defaul
+00027430: 7473 2074 6f20 2769 6e74 6572 7661 6c27  ts to 'interval'
+00027440: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+00027450: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 203a     -------.    :
+00027460: 6f62 6a3a 6070 616e 6461 732e 496e 7465  obj:`pandas.Inte
+00027470: 7276 616c 496e 6465 7860 0a20 2020 2020  rvalIndex`.     
+00027480: 2020 2041 2063 6f70 7920 6f66 2060 6064     A copy of ``d
+00027490: 6660 6020 7769 7468 2074 6865 206f 7269  f`` with the ori
+000274a0: 6769 6e61 6c20 696e 6465 7820 7265 706c  ginal index repl
+000274b0: 6163 6564 2061 6e64 2075 6e64 6572 7370  aced and undersp
+000274c0: 6563 6966 6965 6420 726f 7773 2072 656d  ecified rows rem
+000274d0: 6f76 6564 2028 7468 6f73 6520 7768 6572  oved (those wher
+000274e0: 6520 6e6f 2069 6e74 6572 7661 6c0a 2020  e no interval.  
+000274f0: 2020 2020 2020 636f 756c 6420 6265 2063        could be c
+00027500: 6f70 7574 6564 292e 0a20 2020 2022 2222  oputed)..    """
+00027510: 0a20 2020 2069 6620 6e6f 7420 616c 6c28  .    if not all(
+00027520: 6320 696e 2064 662e 636f 6c75 6d6e 7320  c in df.columns 
+00027530: 666f 7220 6320 696e 2028 706f 7369 7469  for c in (positi
+00027540: 6f6e 5f63 6f6c 2c20 6475 7261 7469 6f6e  on_col, duration
+00027550: 5f63 6f6c 2929 3a0a 2020 2020 2020 2020  _col)):.        
+00027560: 6d69 7373 696e 6720 3d20 5b63 2066 6f72  missing = [c for
+00027570: 2063 2069 6e20 2870 6f73 6974 696f 6e5f   c in (position_
+00027580: 636f 6c2c 2064 7572 6174 696f 6e5f 636f  col, duration_co
+00027590: 6c29 2069 6620 6320 6e6f 7420 696e 2064  l) if c not in d
+000275a0: 662e 636f 6c75 6d6e 735d 0a20 2020 2020  f.columns].     
+000275b0: 2020 2070 6c75 7261 6c20 3d20 2773 2720     plural = 's' 
+000275c0: 6966 206c 656e 286d 6973 7369 6e67 2920  if len(missing) 
+000275d0: 3e20 3120 656c 7365 2027 270a 2020 2020  > 1 else ''.    
+000275e0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+000275f0: 6e67 2866 2243 6f6c 756d 6e7b 706c 7572  ng(f"Column{plur
+00027600: 616c 7d20 6e6f 7420 7072 6573 656e 7420  al} not present 
+00027610: 696e 2044 6174 6146 7261 6d65 3a20 7b27  in DataFrame: {'
+00027620: 2c20 272e 6a6f 696e 286d 6973 7369 6e67  , '.join(missing
+00027630: 297d 2229 0a20 2020 2020 2020 2072 6574  )}").        ret
+00027640: 7572 6e0a 2020 2020 6966 2064 665b 706f  urn.    if df[po
+00027650: 7369 7469 6f6e 5f63 6f6c 5d2e 6973 6e61  sition_col].isna
+00027660: 2829 2e61 6e79 2829 206f 7220 6466 5b64  ().any() or df[d
+00027670: 7572 6174 696f 6e5f 636f 6c5d 2e69 736e  uration_col].isn
+00027680: 6128 292e 616e 7928 293a 0a20 2020 2020  a().any():.     
+00027690: 2020 206d 6973 7369 6e67 203d 2064 665b     missing = df[
+000276a0: 6466 5b5b 706f 7369 7469 6f6e 5f63 6f6c  df[[position_col
+000276b0: 2c20 6475 7261 7469 6f6e 5f63 6f6c 5d5d  , duration_col]]
+000276c0: 2e69 736e 6128 292e 616e 7928 6178 6973  .isna().any(axis
+000276d0: 3d31 295d 0a20 2020 2020 2020 206c 6f67  =1)].        log
+000276e0: 6765 722e 7761 726e 696e 6728 6622 436f  ger.warning(f"Co
+000276f0: 756c 6420 6e6f 7420 6d61 6b65 2049 6e74  uld not make Int
+00027700: 6572 7661 6c49 6e64 6578 2062 6563 6175  ervalIndex becau
+00027710: 7365 206f 6620 6d69 7373 696e 6720 7661  se of missing va
+00027720: 6c75 6573 3a5c 6e7b 6d69 7373 696e 677d  lues:\n{missing}
+00027730: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00027740: 6e0a 2020 2020 7472 793a 0a20 2020 2020  n.    try:.     
+00027750: 2020 206c 6566 7420 3d20 6466 5b70 6f73     left = df[pos
+00027760: 6974 696f 6e5f 636f 6c5d 2e61 7374 7970  ition_col].astyp
+00027770: 6528 666c 6f61 7429 0a20 2020 2020 2020  e(float).       
+00027780: 2072 6967 6874 203d 2028 6c65 6674 202b   right = (left +
+00027790: 2064 665b 6475 7261 7469 6f6e 5f63 6f6c   df[duration_col
+000277a0: 5d29 2e61 7374 7970 6528 666c 6f61 7429  ]).astype(float)
+000277b0: 0a20 2020 2020 2020 2069 6620 726f 756e  .        if roun
+000277c0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+000277d0: 2020 2020 2020 2020 2020 206c 6566 742c             left,
+000277e0: 2072 6967 6874 203d 206c 6566 742e 726f   right = left.ro
+000277f0: 756e 6428 726f 756e 6429 2c20 7269 6768  und(round), righ
+00027800: 742e 726f 756e 6428 726f 756e 6429 0a20  t.round(round). 
+00027810: 2020 2020 2020 2072 6574 7572 6e20 7064         return pd
+00027820: 2e49 6e74 6572 7661 6c49 6e64 6578 2e66  .IntervalIndex.f
+00027830: 726f 6d5f 6172 7261 7973 286c 6566 743d  rom_arrays(left=
+00027840: 6c65 6674 2c20 7269 6768 743d 7269 6768  left, right=righ
+00027850: 742c 2063 6c6f 7365 643d 636c 6f73 6564  t, closed=closed
+00027860: 2c20 6e61 6d65 3d6e 616d 6529 0a20 2020  , name=name).   
+00027870: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00027880: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00027890: 6c6f 6767 6572 2e77 6172 6e69 6e67 2866  logger.warning(f
+000278a0: 2243 7265 6174 696e 6720 496e 7465 7276  "Creating Interv
+000278b0: 616c 496e 6465 7820 6661 696c 6564 2077  alIndex failed w
+000278c0: 6974 6820 6578 6365 7074 696f 6e20 7b65  ith exception {e
+000278d0: 7d2e 2229 0a0a 4066 756e 6374 696f 6e5f  }.")..@function_
+000278e0: 6c6f 6767 6572 0a64 6566 2072 6570 6c61  logger.def repla
+000278f0: 6365 5f69 6e64 6578 5f62 795f 696e 7465  ce_index_by_inte
+00027900: 7276 616c 7328 6466 2c20 706f 7369 7469  rvals(df, positi
+00027910: 6f6e 5f63 6f6c 3d27 7175 6172 7465 7262  on_col='quarterb
+00027920: 6561 7473 272c 2064 7572 6174 696f 6e5f  eats', duration_
+00027930: 636f 6c3d 2764 7572 6174 696f 6e5f 7162  col='duration_qb
+00027940: 272c 2063 6c6f 7365 643d 276c 6566 7427  ', closed='left'
+00027950: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00027960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027970: 2066 696c 7465 725f 7a65 726f 5f64 7572   filter_zero_dur
+00027980: 6174 696f 6e3d 4661 6c73 652c 2072 6f75  ation=False, rou
+00027990: 6e64 3d4e 6f6e 652c 206e 616d 653d 2769  nd=None, name='i
+000279a0: 6e74 6572 7661 6c27 293a 0a20 2020 2022  nterval'):.    "
+000279b0: 2222 4769 7665 6e20 616e 2061 6e6e 6f74  ""Given an annot
+000279c0: 6174 696f 6e73 2074 6162 6c65 2077 6974  ations table wit
+000279d0: 6820 706f 7369 7469 6f6e 7320 616e 6420  h positions and 
+000279e0: 6475 7261 7469 6f6e 732c 2072 6570 6c61  durations, repla
+000279f0: 6365 7320 6974 7320 696e 6465 7820 7769  ces its index wi
+00027a00: 7468 2061 6e20 3a6f 626a 3a60 7061 6e64  th an :obj:`pand
+00027a10: 6173 2e49 6e74 6572 7661 6c49 6e64 6578  as.IntervalIndex
+00027a20: 602e 0a20 2020 2055 6e64 6572 7370 6563  `..    Underspec
+00027a30: 6966 6965 6420 726f 7773 2061 7265 2072  ified rows are r
+00027a40: 656d 6f76 6564 2e0a 0a20 2020 2050 6172  emoved...    Par
+00027a50: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00027a60: 2d2d 2d2d 2d2d 0a20 2020 2064 6620 3a20  ------.    df : 
+00027a70: 3a6f 626a 3a60 7061 6e64 6173 2e44 6174  :obj:`pandas.Dat
+00027a80: 6146 7261 6d65 600a 2020 2020 2020 2020  aFrame`.        
+00027a90: 416e 6e6f 7461 7469 6f6e 2074 6162 6c65  Annotation table
+00027aa0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00027ab0: 636f 6c75 6d6e 7320 6f66 2060 6070 6f73  columns of ``pos
+00027ac0: 6974 696f 6e5f 636f 6c60 6020 2864 6566  ition_col`` (def
+00027ad0: 6175 6c74 3a20 2771 7561 7274 6572 6265  ault: 'quarterbe
+00027ae0: 6174 7327 2920 616e 6420 6060 6475 7261  ats') and ``dura
+00027af0: 7469 6f6e 5f63 6f6c 6060 0a20 2020 2020  tion_col``.     
+00027b00: 2020 2064 6566 6175 6c74 3a20 2764 7572     default: 'dur
+00027b10: 6174 696f 6e5f 7162 2729 2e0a 2020 2020  ation_qb')..    
+00027b20: 706f 7369 7469 6f6e 5f63 6f6c 203a 203a  position_col : :
+00027b30: 6f62 6a3a 6073 7472 602c 206f 7074 696f  obj:`str`, optio
+00027b40: 6e61 6c0a 2020 2020 2020 2020 4e61 6d65  nal.        Name
+00027b50: 206f 6620 7468 6520 636f 6c75 6d6e 2063   of the column c
+00027b60: 6f6e 7461 696e 696e 6720 706f 7369 7469  ontaining positi
+00027b70: 6f6e 732e 0a20 2020 2064 7572 6174 696f  ons..    duratio
+00027b80: 6e5f 636f 6c20 3a20 3a6f 626a 3a60 7374  n_col : :obj:`st
+00027b90: 7260 2c20 6f70 7469 6f6e 616c 0a20 2020  r`, optional.   
+00027ba0: 2020 2020 204e 616d 6520 6f66 2074 6865       Name of the
+00027bb0: 2063 6f6c 756d 6e20 636f 6e74 6169 6e69   column containi
+00027bc0: 6e67 2064 7572 6174 696f 6e73 2e0a 2020  ng durations..  
+00027bd0: 2020 636c 6f73 6564 203a 203a 6f62 6a3a    closed : :obj:
+00027be0: 6073 7472 602c 206f 7074 696f 6e61 6c0a  `str`, optional.
+00027bf0: 2020 2020 2020 2020 276c 6566 7427 2c20          'left', 
+00027c00: 2772 6967 6874 2720 6f72 2027 626f 7468  'right' or 'both
+00027c10: 2720 3c2d 2064 6566 696e 696e 6720 7468  ' <- defining th
+00027c20: 6520 696e 7465 7276 616c 2062 6f75 6e64  e interval bound
+00027c30: 6172 6965 730a 2020 2020 6669 6c74 6572  aries.    filter
+00027c40: 5f7a 6572 6f5f 6475 7261 7469 6f6e 203a  _zero_duration :
+00027c50: 203a 6f62 6a3a 6062 6f6f 6c60 2c20 6f70   :obj:`bool`, op
+00027c60: 7469 6f6e 616c 0a20 2020 2020 2020 2044  tional.        D
+00027c70: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00027c80: 2c20 6d65 616e 696e 6720 7468 6174 2072  , meaning that r
+00027c90: 6f77 7320 7769 7468 207a 6572 6f20 6475  ows with zero du
+00027ca0: 7261 7469 6f6e 7320 6172 6520 6d61 696e  rations are main
+00027cb0: 7461 696e 6564 2e20 5061 7373 2054 7275  tained. Pass Tru
+00027cc0: 6520 746f 2072 656d 6f76 6520 7468 656d  e to remove them
+00027cd0: 2e0a 2020 2020 726f 756e 6420 3a20 3a6f  ..    round : :o
+00027ce0: 626a 3a60 696e 7460 2c20 6f70 7469 6f6e  bj:`int`, option
+00027cf0: 616c 0a20 2020 2020 2020 2054 6f20 686f  al.        To ho
+00027d00: 7720 6d61 6e79 2064 6563 696d 616c 2070  w many decimal p
+00027d10: 6c61 6365 7320 746f 2072 6f75 6e64 2074  laces to round t
+00027d20: 6865 2069 6e74 6572 7661 6c73 2720 626f  he intervals' bo
+00027d30: 756e 6461 7279 2076 616c 7565 732e 0a20  undary values.. 
+00027d40: 2020 206e 616d 6520 3a20 3a6f 626a 3a60     name : :obj:`
+00027d50: 7374 7260 2c20 6f70 7469 6f6e 616c 0a20  str`, optional. 
+00027d60: 2020 2020 2020 204e 616d 6520 6f66 2074         Name of t
+00027d70: 6865 2063 7265 6174 6564 2069 6e64 6578  he created index
+00027d80: 2e20 4465 6661 756c 7473 2074 6f20 2769  . Defaults to 'i
+00027d90: 6e74 6572 7661 6c27 2e0a 0a20 2020 2052  nterval'...    R
+00027da0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00027db0: 2d2d 0a20 2020 203a 6f62 6a3a 6070 616e  --.    :obj:`pan
+00027dc0: 6461 732e 4461 7461 4672 616d 6560 0a20  das.DataFrame`. 
+00027dd0: 2020 2020 2020 2041 2063 6f70 7920 6f66         A copy of
+00027de0: 2060 6064 6660 6020 7769 7468 2074 6865   ``df`` with the
+00027df0: 206f 7269 6769 6e61 6c20 696e 6465 7820   original index 
+00027e00: 7265 706c 6163 6564 2061 6e64 2075 6e64  replaced and und
+00027e10: 6572 7370 6563 6966 6965 6420 726f 7773  erspecified rows
+00027e20: 2072 656d 6f76 6564 2028 7468 6f73 6520   removed (those 
+00027e30: 7768 6572 6520 6e6f 2069 6e74 6572 7661  where no interva
+00027e40: 6c0a 2020 2020 2020 2020 636f 756c 6420  l.        could 
+00027e50: 6265 2063 6f6d 7075 7465 6429 2e0a 2020  be computed)..  
+00027e60: 2020 2222 220a 2020 2020 6966 206e 6f74    """.    if not
+00027e70: 2061 6c6c 2863 2069 6e20 6466 2e63 6f6c   all(c in df.col
+00027e80: 756d 6e73 2066 6f72 2063 2069 6e20 2870  umns for c in (p
+00027e90: 6f73 6974 696f 6e5f 636f 6c2c 2064 7572  osition_col, dur
+00027ea0: 6174 696f 6e5f 636f 6c29 293a 0a20 2020  ation_col)):.   
+00027eb0: 2020 2020 206d 6973 7369 6e67 203d 205b       missing = [
+00027ec0: 6320 666f 7220 6320 696e 2028 706f 7369  c for c in (posi
+00027ed0: 7469 6f6e 5f63 6f6c 2c20 6475 7261 7469  tion_col, durati
+00027ee0: 6f6e 5f63 6f6c 2920 6966 2063 206e 6f74  on_col) if c not
+00027ef0: 2069 6e20 6466 2e63 6f6c 756d 6e73 5d0a   in df.columns].
+00027f00: 2020 2020 2020 2020 706c 7572 616c 203d          plural =
+00027f10: 2027 7327 2069 6620 6c65 6e28 6d69 7373   's' if len(miss
+00027f20: 696e 6729 203e 2031 2065 6c73 6520 2727  ing) > 1 else ''
+00027f30: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00027f40: 7761 726e 696e 6728 6622 436f 6c75 6d6e  warning(f"Column
+00027f50: 7b70 6c75 7261 6c7d 206e 6f74 2070 7265  {plural} not pre
+00027f60: 7365 6e74 2069 6e20 4461 7461 4672 616d  sent in DataFram
+00027f70: 653a 207b 272c 2027 2e6a 6f69 6e28 6d69  e: {', '.join(mi
+00027f80: 7373 696e 6729 7d22 290a 2020 2020 2020  ssing)}").      
+00027f90: 2020 7265 7475 726e 2064 660a 2020 2020    return df.    
+00027fa0: 6d61 736b 203d 2064 665b 706f 7369 7469  mask = df[positi
+00027fb0: 6f6e 5f63 6f6c 5d2e 6e6f 746e 6128 2920  on_col].notna() 
+00027fc0: 2620 2864 665b 706f 7369 7469 6f6e 5f63  & (df[position_c
+00027fd0: 6f6c 5d20 213d 2027 2729 2026 2064 665b  ol] != '') & df[
+00027fe0: 6475 7261 7469 6f6e 5f63 6f6c 5d2e 6e6f  duration_col].no
+00027ff0: 746e 6128 290a 2020 2020 6e5f 6472 6f70  tna().    n_drop
+00028000: 7065 6420 3d20 287e 6d61 736b 292e 7375  ped = (~mask).su
+00028010: 6d28 290a 2020 2020 6966 2066 696c 7465  m().    if filte
+00028020: 725f 7a65 726f 5f64 7572 6174 696f 6e3a  r_zero_duration:
+00028030: 0a20 2020 2020 2020 206d 6173 6b20 263d  .        mask &=
+00028040: 2028 6466 5b64 7572 6174 696f 6e5f 636f   (df[duration_co
+00028050: 6c5d 203e 2030 290a 2020 2020 656c 6966  l] > 0).    elif
+00028060: 206e 5f64 726f 7070 6564 203e 2030 3a0a   n_dropped > 0:.
+00028070: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00028080: 6e66 6f28 6622 4861 6420 746f 2064 726f  nfo(f"Had to dro
+00028090: 7020 7b6e 5f64 726f 7070 6564 7d20 726f  p {n_dropped} ro
+000280a0: 7773 2066 6f72 2063 7265 6174 696e 6720  ws for creating 
+000280b0: 7468 6520 496e 7465 7276 616c 496e 6465  the IntervalInde
+000280c0: 783a 5c6e 7b64 665b 7e6d 6173 6b5d 7d22  x:\n{df[~mask]}"
+000280d0: 290a 2020 2020 6466 203d 2064 665b 6d61  ).    df = df[ma
+000280e0: 736b 5d2e 636f 7079 2829 0a20 2020 2069  sk].copy().    i
+000280f0: 765f 696e 6465 7820 3d20 6d61 6b65 5f69  v_index = make_i
+00028100: 6e74 6572 7661 6c5f 696e 6465 785f 6672  nterval_index_fr
+00028110: 6f6d 5f64 7572 6174 696f 6e73 2864 662c  om_durations(df,
+00028120: 2070 6f73 6974 696f 6e5f 636f 6c3d 706f   position_col=po
+00028130: 7369 7469 6f6e 5f63 6f6c 2c20 6475 7261  sition_col, dura
+00028140: 7469 6f6e 5f63 6f6c 3d64 7572 6174 696f  tion_col=duratio
+00028150: 6e5f 636f 6c2c 0a20 2020 2020 2020 2020  n_col,.         
+00028160: 2020 2020 2020 2020 2020 2063 6c6f 7365             close
+00028170: 643d 636c 6f73 6564 2c20 726f 756e 643d  d=closed, round=
+00028180: 726f 756e 642c 206e 616d 653d 6e61 6d65  round, name=name
+00028190: 2c20 6c6f 6767 6572 3d6c 6f67 6765 7229  , logger=logger)
+000281a0: 0a20 2020 2069 6620 6466 5b64 7572 6174  .    if df[durat
+000281b0: 696f 6e5f 636f 6c5d 2e64 7479 7065 2021  ion_col].dtype !
+000281c0: 3d20 666c 6f61 743a 0a20 2020 2020 2020  = float:.       
+000281d0: 2077 6974 6820 7761 726e 696e 6773 2e63   with warnings.c
+000281e0: 6174 6368 5f77 6172 6e69 6e67 7328 293a  atch_warnings():
+000281f0: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
+00028200: 6574 7469 6e67 2076 616c 7565 7320 696e  etting values in
+00028210: 2d70 6c61 6365 2069 7320 6669 6e65 2c20  -place is fine, 
+00028220: 6967 6e6f 7265 2074 6865 2077 6172 6e69  ignore the warni
+00028230: 6e67 2069 6e20 5061 6e64 6173 203e 3d20  ng in Pandas >= 
+00028240: 312e 352e 300a 2020 2020 2020 2020 2020  1.5.0.          
+00028250: 2020 2320 5468 6973 2063 616e 2062 6520    # This can be 
+00028260: 7265 6d6f 7665 642c 2069 6620 5061 6e64  removed, if Pand
+00028270: 6173 2031 2e35 2e30 2064 6f65 7320 6e6f  as 1.5.0 does no
+00028280: 7420 6e65 6564 2074 6f20 6265 2073 7570  t need to be sup
+00028290: 706f 7274 6564 2061 6e79 206c 6f6e 6765  ported any longe
+000282a0: 722e 0a20 2020 2020 2020 2020 2020 2023  r..            #
+000282b0: 2053 6565 2061 6c73 6f3a 2068 7474 7073   See also: https
+000282c0: 3a2f 2f73 7461 636b 6f76 6572 666c 6f77  ://stackoverflow
+000282d0: 2e63 6f6d 2f71 2f37 3430 3537 3336 372f  .com/q/74057367/
+000282e0: 3835 3935 3931 0a20 2020 2020 2020 2020  859591.         
+000282f0: 2020 2077 6172 6e69 6e67 732e 6669 6c74     warnings.filt
+00028300: 6572 7761 726e 696e 6773 280a 2020 2020  erwarnings(.    
+00028310: 2020 2020 2020 2020 2020 2020 2269 676e              "ign
+00028320: 6f72 6522 2c0a 2020 2020 2020 2020 2020  ore",.          
+00028330: 2020 2020 2020 6361 7465 676f 7279 3d46        category=F
+00028340: 7574 7572 6557 6172 6e69 6e67 2c0a 2020  utureWarning,.  
+00028350: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00028360: 7373 6167 653d 280a 2020 2020 2020 2020  ssage=(.        
+00028370: 2020 2020 2020 2020 2020 2020 222e 2a77              ".*w
+00028380: 696c 6c20 6174 7465 6d70 7420 746f 2073  ill attempt to s
+00028390: 6574 2074 6865 2076 616c 7565 7320 696e  et the values in
+000283a0: 706c 6163 6520 696e 7374 6561 6420 6f66  place instead of
+000283b0: 2061 6c77 6179 7320 7365 7474 696e 6720   always setting 
+000283c0: 6120 6e65 7720 6172 7261 792e 2022 0a20  a new array. ". 
+000283d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000283e0: 2020 2022 546f 2072 6574 6169 6e20 7468     "To retain th
+000283f0: 6520 6f6c 6420 6265 6861 7669 6f72 2c20  e old behavior, 
+00028400: 7573 6520 6569 7468 6572 2e2a 220a 2020  use either.*".  
+00028410: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00028420: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00028430: 2020 2020 2020 2020 2020 2064 662e 6c6f             df.lo
+00028440: 635b 3a2c 2064 7572 6174 696f 6e5f 636f  c[:, duration_co
+00028450: 6c5d 203d 2070 642e 746f 5f6e 756d 6572  l] = pd.to_numer
+00028460: 6963 2864 665b 6475 7261 7469 6f6e 5f63  ic(df[duration_c
+00028470: 6f6c 5d29 0a20 2020 2069 6620 6976 5f69  ol]).    if iv_i
+00028480: 6e64 6578 2069 7320 4e6f 6e65 3a0a 2020  ndex is None:.  
+00028490: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+000284a0: 6e69 6e67 2822 4372 6561 7469 6e67 2049  ning("Creating I
+000284b0: 6e74 6572 7661 6c49 6e64 6578 2066 6169  ntervalIndex fai
+000284c0: 6c65 642e 2229 0a20 2020 2020 2020 2072  led.").        r
+000284d0: 6574 7572 6e20 6466 0a20 2020 2064 662e  eturn df.    df.
+000284e0: 696e 6465 7820 3d20 6976 5f69 6e64 6578  index = iv_index
+000284f0: 0a20 2020 2072 6574 7572 6e20 6466 0a0a  .    return df..
+00028500: 6465 6620 626f 6f6c 6561 6e5f 6d6f 6465  def boolean_mode
+00028510: 5f63 6f6c 3273 7472 696e 6773 2853 2920  _col2strings(S) 
+00028520: 2d3e 2070 642e 5365 7269 6573 3a0a 2020  -> pd.Series:.  
+00028530: 2020 2222 2254 7572 6e20 7468 6520 626f    """Turn the bo
+00028540: 6f6c 6561 6e20 6973 5f6d 696e 6f72 2063  olean is_minor c
+00028550: 6f6c 756d 6e73 2069 6e74 6f20 7374 7269  olumns into stri
+00028560: 6e67 2063 6f6c 756d 6e73 2073 7563 6820  ng columns such 
+00028570: 7468 6174 2054 7275 6520 3d3e 2027 6d69  that True => 'mi
+00028580: 6e6f 7227 2c20 4661 6c73 6520 3d3e 2027  nor', False => '
+00028590: 6d61 6a6f 7227 2e22 2222 0a20 2020 2072  major'.""".    r
+000285a0: 6574 7572 6e20 532e 6d61 7028 7b54 7275  eturn S.map({Tru
+000285b0: 653a 2027 6d69 6e6f 7227 2c20 4661 6c73  e: 'minor', Fals
+000285c0: 653a 2027 6d61 6a6f 7227 7d29 0a0a 6465  e: 'major'})..de
+000285d0: 6620 7265 706c 6163 655f 626f 6f6c 6561  f replace_boolea
+000285e0: 6e5f 6d6f 6465 5f62 795f 7374 7269 6e67  n_mode_by_string
+000285f0: 7328 6466 2920 2d3e 2070 642e 4461 7461  s(df) -> pd.Data
+00028600: 4672 616d 653a 0a20 2020 2022 2222 5265  Frame:.    """Re
+00028610: 706c 6163 6573 2062 6f6f 6c65 616e 2027  places boolean '
+00028620: 5f69 735f 6d69 6e6f 7227 2063 6f6c 756d  _is_minor' colum
+00028630: 6e73 2077 6974 6820 7374 7269 6e67 2063  ns with string c
+00028640: 6f6c 756d 6e73 2072 656e 616d 6564 2074  olumns renamed t
+00028650: 6f20 275f 6d6f 6465 272e 0a20 2020 2045  o '_mode'..    E
+00028660: 7861 6d70 6c65 3a20 6466 5b27 736f 6d65  xample: df['some
+00028670: 5f63 6f6c 272c 2027 736f 6d65 5f6e 616d  _col', 'some_nam
+00028680: 655f 6973 5f6d 696e 6f72 275d 203d 3e20  e_is_minor'] => 
+00028690: 6466 5b27 736f 6d65 5f63 6f6c 272c 2027  df['some_col', '
+000286a0: 736f 6d65 5f6e 616d 655f 6d6f 6465 275d  some_name_mode']
+000286b0: 0a20 2020 2022 2222 0a20 2020 2062 6f6f  .    """.    boo
+000286c0: 6c5f 636f 6c73 203d 205b 636f 6c20 666f  l_cols = [col fo
+000286d0: 7220 636f 6c20 696e 2064 662e 636f 6c75  r col in df.colu
+000286e0: 6d6e 7320 6966 2063 6f6c 2e65 6e64 7377  mns if col.endsw
+000286f0: 6974 6828 275f 6973 5f6d 696e 6f72 2729  ith('_is_minor')
+00028700: 5d0a 2020 2020 6966 206c 656e 2862 6f6f  ].    if len(boo
+00028710: 6c5f 636f 6c73 2920 3d3d 2030 3a0a 2020  l_cols) == 0:.  
+00028720: 2020 2020 2020 7265 7475 726e 2064 660a        return df.
+00028730: 2020 2020 6466 203d 2064 662e 636f 7079      df = df.copy
+00028740: 2829 0a20 2020 2072 656e 616d 696e 6720  ().    renaming 
+00028750: 3d20 7b7d 0a20 2020 2066 6f72 2063 6f6c  = {}.    for col
+00028760: 5f6e 616d 6520 696e 2062 6f6f 6c5f 636f  _name in bool_co
+00028770: 6c73 3a0a 2020 2020 2020 2020 6e75 6d65  ls:.        nume
+00028780: 7261 6c5f 6e61 6d65 203d 2063 6f6c 5f6e  ral_name = col_n
+00028790: 616d 655b 3a2d 6c65 6e28 275f 6973 5f6d  ame[:-len('_is_m
+000287a0: 696e 6f72 2729 5d0a 2020 2020 2020 2020  inor')].        
+000287b0: 6966 2063 6f6c 5f6e 616d 6520 696e 2064  if col_name in d
+000287c0: 662e 636f 6c75 6d6e 733a 0a20 2020 2020  f.columns:.     
+000287d0: 2020 2020 2020 206e 6577 5f63 6f6c 5f6e         new_col_n
+000287e0: 616d 6520 3d20 6622 7b6e 756d 6572 616c  ame = f"{numeral
+000287f0: 5f6e 616d 657d 5f6d 6f64 6522 0a20 2020  _name}_mode".   
+00028800: 2020 2020 2020 2020 206e 6577 5f63 6f6c           new_col
+00028810: 203d 2062 6f6f 6c65 616e 5f6d 6f64 655f   = boolean_mode_
+00028820: 636f 6c32 7374 7269 6e67 7328 6466 5b63  col2strings(df[c
+00028830: 6f6c 5f6e 616d 655d 290a 2020 2020 2020  ol_name]).      
+00028840: 2020 2020 2020 6466 2e6c 6f63 5b3a 2c63        df.loc[:,c
+00028850: 6f6c 5f6e 616d 655d 203d 206e 6577 5f63  ol_name] = new_c
+00028860: 6f6c 0a20 2020 2020 2020 2020 2020 2072  ol.            r
+00028870: 656e 616d 696e 675b 636f 6c5f 6e61 6d65  enaming[col_name
+00028880: 5d20 3d20 6e65 775f 636f 6c5f 6e61 6d65  ] = new_col_name
+00028890: 0a20 2020 2064 662e 7265 6e61 6d65 2863  .    df.rename(c
+000288a0: 6f6c 756d 6e73 3d72 656e 616d 696e 672c  olumns=renaming,
+000288b0: 2069 6e70 6c61 6365 3d54 7275 6529 0a20   inplace=True). 
+000288c0: 2020 2072 6574 7572 6e20 6466 0a0a 4066     return df..@f
+000288d0: 756e 6374 696f 6e5f 6c6f 6767 6572 0a64  unction_logger.d
+000288e0: 6566 2072 6573 6f6c 7665 5f72 656c 6174  ef resolve_relat
+000288f0: 6976 655f 6b65 7973 2872 656c 6174 6976  ive_keys(relativ
+00028900: 6572 6f6f 742c 206d 696e 6f72 3d46 616c  eroot, minor=Fal
+00028910: 7365 293a 0a20 2020 2022 2222 2052 6573  se):.    """ Res
+00028920: 6f6c 7665 206e 6573 7465 6420 7265 6c61  olve nested rela
+00028930: 7469 7665 206b 6579 732c 2065 2e67 2e20  tive keys, e.g. 
+00028940: 2756 2f56 2f56 2720 3d3e 2027 5649 272e  'V/V/V' => 'VI'.
+00028950: 0a0a 2020 2020 5573 6573 3a20 3a70 793a  ..    Uses: :py:
+00028960: 6675 6e63 3a60 7265 6c32 6162 735f 6b65  func:`rel2abs_ke
+00028970: 7960 2c20 3a70 793a 6675 6e63 3a60 7374  y`, :py:func:`st
+00028980: 725f 6973 5f6d 696e 6f72 600a 0a20 2020  r_is_minor`..   
+00028990: 2072 656c 6174 6976 6572 6f6f 7420 3a20   relativeroot : 
+000289a0: 3a6f 626a 3a60 7374 7260 0a20 2020 2020  :obj:`str`.     
+000289b0: 2020 204f 6e65 206f 7220 7365 7665 7261     One or severa
+000289c0: 6c20 7265 6c61 7469 7665 206b 6579 732c  l relative keys,
+000289d0: 2065 2e67 2e20 6976 2f76 2f56 4920 2866   e.g. iv/v/VI (f
+000289e0: 6f75 7274 6820 7363 616c 6520 6465 6772  ourth scale degr
+000289f0: 6565 206f 6620 7468 6520 6669 6674 6820  ee of the fifth 
+00028a00: 7363 616c 6520 6465 6772 6565 206f 6620  scale degree of 
+00028a10: 7468 6520 7369 7874 6820 7363 616c 6520  the sixth scale 
+00028a20: 6465 6772 6565 290a 2020 2020 6d69 6e6f  degree).    mino
+00028a30: 7220 3a20 3a6f 626a 3a60 626f 6f6c 602c  r : :obj:`bool`,
+00028a40: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00028a50: 2020 5061 7373 2054 7275 6520 6966 2074    Pass True if t
+00028a60: 6865 206c 6173 7420 6f66 2074 6865 2072  he last of the r
+00028a70: 656c 6174 6976 6520 6b65 7973 2069 7320  elative keys is 
+00028a80: 746f 2062 6520 696e 7465 7270 7265 7465  to be interprete
+00028a90: 6420 7769 7468 696e 2061 206d 696e 6f72  d within a minor
+00028aa0: 2063 6f6e 7465 7874 2e0a 2020 2020 2222   context..    ""
+00028ab0: 220a 2020 2020 6966 2070 642e 6973 6e75  ".    if pd.isnu
+00028ac0: 6c6c 2872 656c 6174 6976 6572 6f6f 7429  ll(relativeroot)
+00028ad0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00028ae0: 2072 656c 6174 6976 6572 6f6f 740a 2020   relativeroot.  
+00028af0: 2020 7370 6c20 3d20 7265 6c61 7469 7665    spl = relative
+00028b00: 726f 6f74 2e73 706c 6974 2827 2f27 290a  root.split('/').
+00028b10: 2020 2020 6966 206c 656e 2873 706c 2920      if len(spl) 
+00028b20: 3c20 323a 0a20 2020 2020 2020 2072 6574  < 2:.        ret
+00028b30: 7572 6e20 7265 6c61 7469 7665 726f 6f74  urn relativeroot
+00028b40: 0a20 2020 2069 6620 6c65 6e28 7370 6c29  .    if len(spl)
+00028b50: 203d 3d20 323a 0a20 2020 2020 2020 2061   == 2:.        a
+00028b60: 7070 6c69 6564 2c20 746f 203d 2073 706c  pplied, to = spl
+00028b70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00028b80: 7265 6c32 6162 735f 6b65 7928 6170 706c  rel2abs_key(appl
+00028b90: 6965 642c 2074 6f2c 206d 696e 6f72 2c20  ied, to, minor, 
+00028ba0: 6c6f 6767 6572 3d6c 6f67 6765 7229 0a20  logger=logger). 
+00028bb0: 2020 2070 7265 7669 6f75 732c 206c 6173     previous, las
+00028bc0: 7420 3d20 272f 272e 6a6f 696e 2873 706c  t = '/'.join(spl
+00028bd0: 5b3a 2d31 5d29 2c20 7370 6c5b 2d31 5d0a  [:-1]), spl[-1].
+00028be0: 2020 2020 7265 7475 726e 2072 656c 3261      return rel2a
+00028bf0: 6273 5f6b 6579 2872 6573 6f6c 7665 5f72  bs_key(resolve_r
+00028c00: 656c 6174 6976 655f 6b65 7973 2870 7265  elative_keys(pre
+00028c10: 7669 6f75 732c 2073 7472 5f69 735f 6d69  vious, str_is_mi
+00028c20: 6e6f 7228 6c61 7374 2c20 6973 5f6e 616d  nor(last, is_nam
+00028c30: 653d 4661 6c73 6529 292c 206c 6173 742c  e=False)), last,
+00028c40: 206d 696e 6f72 290a 0a0a 6465 6620 7365   minor)...def se
+00028c50: 7269 6573 5f69 735f 6d69 6e6f 7228 532c  ries_is_minor(S,
+00028c60: 2069 735f 6e61 6d65 3d54 7275 6529 3a0a   is_name=True):.
+00028c70: 2020 2020 2222 2220 5265 7475 726e 7320      """ Returns 
+00028c80: 626f 6f6c 6561 6e20 5365 7269 6573 2077  boolean Series w
+00028c90: 6865 7265 2065 7665 7279 2076 616c 7565  here every value
+00028ca0: 2069 6e20 6060 5360 6020 7265 7072 6573   in ``S`` repres
+00028cb0: 656e 7469 6e67 2061 206d 696e 6f72 206b  enting a minor k
+00028cc0: 6579 2f63 686f 7264 2069 7320 5472 7565  ey/chord is True
+00028cd0: 2e22 2222 0a20 2020 2023 2072 6567 6578  .""".    # regex
+00028ce0: 203d 2072 2728 5b41 2d47 612d 675d 295b   = r'([A-Ga-g])[
+00028cf0: 237c 625d 2a27 2069 6620 6973 5f6e 616d  #|b]*' if is_nam
+00028d00: 6520 656c 7365 2027 5b23 7c62 5d2a 285c  e else '[#|b]*(\
+00028d10: 772b 2927 0a20 2020 2023 2072 6574 7572  w+)'.    # retur
+00028d20: 6e20 532e 7374 722e 7265 706c 6163 6528  n S.str.replace(
+00028d30: 7265 6765 782c 206c 616d 6264 6120 6d3a  regex, lambda m:
+00028d40: 206d 2e67 726f 7570 2831 2929 2e73 7472   m.group(1)).str
+00028d50: 2e69 736c 6f77 6572 2829 0a20 2020 2072  .islower().    r
+00028d60: 6574 7572 6e20 532e 7374 722e 6973 6c6f  eturn S.str.islo
+00028d70: 7765 7228 2920 2023 2061 7320 736f 6f6e  wer()  # as soon
+00028d80: 2061 7320 6f6e 6520 6368 6172 6163 7465   as one characte
+00028d90: 7220 6973 206e 6f74 206c 6f77 6572 6361  r is not lowerca
+00028da0: 7365 2c20 6974 2073 686f 756c 6420 6265  se, it should be
+00028db0: 206d 616a 6f72 0a0a 0a64 6566 2073 7472   major...def str
+00028dc0: 5f69 735f 6d69 6e6f 7228 746f 6e65 2c20  _is_minor(tone, 
+00028dd0: 6973 5f6e 616d 653d 5472 7565 293a 0a20  is_name=True):. 
+00028de0: 2020 2022 2222 2052 6574 7572 6e73 2054     """ Returns T
+00028df0: 7275 6520 6966 2060 6074 6f6e 6560 6020  rue if ``tone`` 
+00028e00: 7265 7072 6573 656e 7473 2061 206d 696e  represents a min
+00028e10: 6f72 206b 6579 206f 7220 6368 6f72 642e  or key or chord.
+00028e20: 2222 220a 2020 2020 2320 7265 6765 7820  """.    # regex 
+00028e30: 3d20 7227 285b 412d 4761 2d67 5d29 5b23  = r'([A-Ga-g])[#
+00028e40: 7c62 5d2a 2720 6966 2069 735f 6e61 6d65  |b]*' if is_name
+00028e50: 2065 6c73 6520 275b 237c 625d 2a28 5c77   else '[#|b]*(\w
+00028e60: 2b29 270a 2020 2020 2320 6d20 3d20 7265  +)'.    # m = re
+00028e70: 2e6d 6174 6368 2872 6567 6578 2c20 746f  .match(regex, to
+00028e80: 6e65 290a 2020 2020 2320 6966 206d 2069  ne).    # if m i
+00028e90: 7320 4e6f 6e65 3a0a 2020 2020 2320 2020  s None:.    #   
+00028ea0: 2020 7265 7475 726e 206d 0a20 2020 2023    return m.    #
+00028eb0: 2072 6574 7572 6e20 6d2e 6772 6f75 7028   return m.group(
+00028ec0: 3129 2e69 736c 6f77 6572 2829 0a20 2020  1).islower().   
+00028ed0: 2072 6574 7572 6e20 746f 6e65 2e69 736c   return tone.isl
+00028ee0: 6f77 6572 2829 0a0a 0a40 6675 6e63 7469  ower()...@functi
+00028ef0: 6f6e 5f6c 6f67 6765 720a 6465 6620 7472  on_logger.def tr
+00028f00: 616e 7370 6f73 655f 6368 616e 6765 7328  anspose_changes(
+00028f10: 6368 616e 6765 732c 206f 6c64 5f6e 756d  changes, old_num
+00028f20: 2c20 6e65 775f 6e75 6d2c 206f 6c64 5f6d  , new_num, old_m
+00028f30: 696e 6f72 3d46 616c 7365 2c20 6e65 775f  inor=False, new_
+00028f40: 6d69 6e6f 723d 4661 6c73 6529 3a0a 2020  minor=False):.  
+00028f50: 2020 2222 220a 2020 2020 5369 6e63 6520    """.    Since 
+00028f60: 7468 6520 696e 7465 7276 616c 2073 697a  the interval siz
+00028f70: 6573 2065 7870 7265 7373 6564 2062 7920  es expressed by 
+00028f80: 7468 6520 6368 616e 6765 7320 6f66 2074  the changes of t
+00028f90: 6865 2044 434d 4c20 6861 726d 6f6e 7920  he DCML harmony 
+00028fa0: 7379 6e74 6178 0a20 2020 2064 6570 656e  syntax.    depen
+00028fb0: 6420 6f6e 2074 6865 206e 756d 6572 616c  d on the numeral
+00028fc0: 2773 2070 6f73 6974 696f 6e20 696e 2074  's position in t
+00028fd0: 6865 2073 6361 6c65 2c20 7468 6573 6520  he scale, these 
+00028fe0: 6d61 7920 6368 616e 6765 2069 6620 7468  may change if th
+00028ff0: 6520 6e75 6d65 7261 6c0a 2020 2020 6973  e numeral.    is
+00029000: 2074 7261 6e73 706f 7365 642e 2054 6869   transposed. Thi
+00029010: 7320 6675 6e63 7469 6f6e 2065 7870 7265  s function expre
+00029020: 7373 6573 2074 6865 2073 616d 6520 6368  sses the same ch
+00029030: 616e 6765 7320 666f 7220 7468 6520 6e65  anges for the ne
+00029040: 7720 706f 7369 7469 6f6e 2e0a 2020 2020  w position..    
+00029050: 4368 6f72 6420 746f 6e65 2061 6c74 6572  Chord tone alter
+00029060: 6174 696f 6e73 2028 6f66 2033 2061 6e64  ations (of 3 and
+00029070: 2035 2920 7374 6179 2075 6e74 6f75 6368   5) stay untouch
+00029080: 6564 2e0a 0a20 2020 2055 7365 733a 203a  ed...    Uses: :
+00029090: 7079 3a66 756e 633a 6063 6861 6e67 6573  py:func:`changes
+000290a0: 3274 7063 600a 0a20 2020 2050 6172 616d  2tpc`..    Param
+000290b0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000290c0: 2d2d 2d2d 0a20 2020 2063 6861 6e67 6573  ----.    changes
+000290d0: 203a 203a 6f62 6a3a 6073 7472 600a 2020   : :obj:`str`.  
+000290e0: 2020 2020 2020 4120 7374 7269 6e67 206f        A string o
+000290f0: 6620 6368 616e 6765 7320 666f 6c6c 6f77  f changes follow
+00029100: 696e 6720 7468 6520 4443 4d4c 2068 6172  ing the DCML har
+00029110: 6d6f 6e79 2073 7461 6e64 6172 642e 0a20  mony standard.. 
+00029120: 2020 206f 6c64 5f6e 756d 2c20 6e65 775f     old_num, new_
+00029130: 6e75 6d20 3a20 3a6f 626a 3a60 7374 7260  num : :obj:`str`
+00029140: 3a0a 2020 2020 2020 2020 4f6c 6420 6e75  :.        Old nu
+00029150: 6d65 7261 6c2c 206e 6577 206e 756d 6572  meral, new numer
+00029160: 616c 2e0a 2020 2020 6f6c 645f 6d69 6e6f  al..    old_mino
+00029170: 722c 206e 6577 5f6d 696e 6f72 203a 203a  r, new_minor : :
+00029180: 6f62 6a3a 6062 6f6f 6c60 2c20 6f70 7469  obj:`bool`, opti
+00029190: 6f6e 616c 0a20 2020 2020 2020 2046 6f72  onal.        For
+000291a0: 2065 6163 6820 6e75 6d65 7261 6c2c 2070   each numeral, p
+000291b0: 6173 7320 5472 7565 2069 6620 6974 206f  ass True if it o
+000291c0: 6363 7572 7320 696e 2061 206d 696e 6f72  ccurs in a minor
+000291d0: 2063 6f6e 7465 7874 2e0a 2020 2020 2222   context..    ""
+000291e0: 220a 2020 2020 6966 2070 642e 6973 6e75  ".    if pd.isnu
+000291f0: 6c6c 2863 6861 6e67 6573 293a 0a20 2020  ll(changes):.   
+00029200: 2020 2020 2072 6574 7572 6e20 6368 616e       return chan
+00029210: 6765 730a 2020 2020 6f6c 6420 3d20 6368  ges.    old = ch
+00029220: 616e 6765 7332 7470 6328 6368 616e 6765  anges2tpc(change
+00029230: 732c 206f 6c64 5f6e 756d 2c20 6d69 6e6f  s, old_num, mino
+00029240: 723d 6f6c 645f 6d69 6e6f 722c 2072 6f6f  r=old_minor, roo
+00029250: 745f 616c 7465 7261 7469 6f6e 733d 5472  t_alterations=Tr
+00029260: 7565 290a 2020 2020 6e65 7720 3d20 6368  ue).    new = ch
+00029270: 616e 6765 7332 7470 6328 6368 616e 6765  anges2tpc(change
+00029280: 732c 206e 6577 5f6e 756d 2c20 6d69 6e6f  s, new_num, mino
+00029290: 723d 6e65 775f 6d69 6e6f 722c 2072 6f6f  r=new_minor, roo
+000292a0: 745f 616c 7465 7261 7469 6f6e 733d 5472  t_alterations=Tr
+000292b0: 7565 290a 2020 2020 7265 7320 3d20 5b5d  ue).    res = []
+000292c0: 0a20 2020 2067 6574 5f61 6363 203d 206c  .    get_acc = l
+000292d0: 616d 6264 6120 6e3a 206e 202a 2027 2327  ambda n: n * '#'
+000292e0: 2069 6620 6e20 3e20 3020 656c 7365 202d   if n > 0 else -
+000292f0: 6e20 2a20 2762 270a 2020 2020 666f 7220  n * 'b'.    for 
+00029300: 2866 756c 6c2c 2061 6464 6564 2c20 6163  (full, added, ac
+00029310: 632c 2063 686f 7264 5f69 6e74 6572 7661  c, chord_interva
+00029320: 6c2c 2069 7631 292c 2028 5f2c 205f 2c20  l, iv1), (_, _, 
+00029330: 5f2c 205f 2c20 6976 3229 2069 6e20 7a69  _, _, iv2) in zi
+00029340: 7028 6f6c 642c 206e 6577 293a 0a20 2020  p(old, new):.   
+00029350: 2020 2020 2069 6620 6976 3120 6973 204e       if iv1 is N
+00029360: 6f6e 6520 6f72 2069 7631 203d 3d20 6976  one or iv1 == iv
+00029370: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
+00029380: 6573 2e61 7070 656e 6428 6675 6c6c 290a  es.append(full).
+00029390: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000293a0: 2020 2020 2020 2020 2020 6420 3d20 6976            d = iv
+000293b0: 3220 2d20 6976 310a 2020 2020 2020 2020  2 - iv1.        
+000293c0: 2020 2020 6966 2064 2025 2037 203e 2030      if d % 7 > 0
+000293d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000293e0: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
+000293f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00029400: 2020 2020 2020 6622 5468 6520 6469 6666        f"The diff
+00029410: 6572 656e 6365 2062 6574 7765 656e 2074  erence between t
+00029420: 6865 2069 6e74 6572 7661 6c73 206f 6620  he intervals of 
+00029430: 7b66 756c 6c7d 2069 6e20 7b6f 6c64 5f6e  {full} in {old_n
+00029440: 756d 7d20 616e 6420 7b6e 6577 5f6e 756d  um} and {new_num
+00029450: 7d20 2869 6e20 7b27 6d69 6e6f 7227 2069  } (in {'minor' i
+00029460: 6620 6d69 6e6f 7220 656c 7365 2027 6d61  f minor else 'ma
+00029470: 6a6f 7227 7d29 2064 6f6e 2774 2064 6966  jor'}) don't dif
+00029480: 6665 7220 6279 2063 6872 6f6d 6174 6963  fer by chromatic
+00029490: 2073 656d 6974 6f6e 6573 2e22 290a 2020   semitones.").  
+000294a0: 2020 2020 2020 2020 2020 6e5f 6163 6320            n_acc 
+000294b0: 3d20 6163 632e 636f 756e 7428 2723 2729  = acc.count('#')
+000294c0: 202d 2061 6363 2e63 6f75 6e74 2827 6227   - acc.count('b'
+000294d0: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
+000294e0: 775f 6163 6320 3d20 6765 745f 6163 6328  w_acc = get_acc(
+000294f0: 6e5f 6163 6320 2d20 6420 2f2f 2037 290a  n_acc - d // 7).
+00029500: 2020 2020 2020 2020 2020 2020 7265 732e              res.
+00029510: 6170 7065 6e64 2861 6464 6564 202b 206e  append(added + n
+00029520: 6577 5f61 6363 202b 2063 686f 7264 5f69  ew_acc + chord_i
+00029530: 6e74 6572 7661 6c29 0a20 2020 2072 6574  nterval).    ret
+00029540: 7572 6e20 2727 2e6a 6f69 6e28 7265 7329  urn ''.join(res)
+00029550: 0a0a 0a40 6675 6e63 7469 6f6e 5f6c 6f67  ...@function_log
+00029560: 6765 720a 6465 6620 6665 6174 7572 6573  ger.def features
+00029570: 3274 7063 7328 6e75 6d65 7261 6c2c 2066  2tpcs(numeral, f
+00029580: 6f72 6d3d 4e6f 6e65 2c20 6669 6762 6173  orm=None, figbas
+00029590: 733d 4e6f 6e65 2c20 6368 616e 6765 733d  s=None, changes=
+000295a0: 4e6f 6e65 2c20 7265 6c61 7469 7665 726f  None, relativero
+000295b0: 6f74 3d4e 6f6e 652c 206b 6579 3d27 4327  ot=None, key='C'
+000295c0: 2c20 6d69 6e6f 723d 4e6f 6e65 2c0a 2020  , minor=None,.  
+000295d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000295e0: 6d65 7267 655f 746f 6e65 733d 5472 7565  merge_tones=True
+000295f0: 2c20 6261 7373 5f6f 6e6c 793d 4661 6c73  , bass_only=Fals
+00029600: 652c 206d 633d 4e6f 6e65 293a 0a20 2020  e, mc=None):.   
+00029610: 2022 2222 0a20 2020 2047 6976 656e 2074   """.    Given t
+00029620: 6865 2066 6561 7475 7265 7320 6f66 2061  he features of a
+00029630: 2063 686f 7264 206c 6162 656c 2c20 7468   chord label, th
+00029640: 6973 2066 756e 6374 696f 6e20 7265 7475  is function retu
+00029650: 726e 7320 7468 6520 6368 6f72 6420 746f  rns the chord to
+00029660: 6e65 730a 2020 2020 696e 2074 6865 206f  nes.    in the o
+00029670: 7264 6572 206f 6620 7468 6520 696e 7665  rder of the inve
+00029680: 7273 696f 6e2c 2073 7461 7274 696e 6720  rsion, starting 
+00029690: 6672 6f6d 2074 6865 2062 6173 7320 6e6f  from the bass no
+000296a0: 7465 2e20 5468 6520 746f 6e65 7320 6172  te. The tones ar
+000296b0: 650a 2020 2020 6578 7072 6573 7365 6420  e.    expressed 
+000296c0: 6173 2074 6f6e 616c 2070 6974 6368 2063  as tonal pitch c
+000296d0: 6c61 7373 6573 2c20 7768 6572 6520 2d31  lasses, where -1
+000296e0: 3d46 2c20 303d 432c 2031 3d47 2065 7463  =F, 0=C, 1=G etc
+000296f0: 2e0a 0a20 2020 2055 7365 733a 203a 7079  ...    Uses: :py
+00029700: 3a66 756e 633a 607e 2e75 7469 6c73 2e63  :func:`~.utils.c
+00029710: 6861 6e67 6573 326c 6973 7460 2c20 3a70  hanges2list`, :p
+00029720: 793a 6675 6e63 3a60 7e2e 7574 696c 732e  y:func:`~.utils.
+00029730: 6e61 6d65 3266 6966 7468 7360 2c20 3a70  name2fifths`, :p
+00029740: 793a 6675 6e63 3a60 7e2e 7574 696c 732e  y:func:`~.utils.
+00029750: 7265 736f 6c76 655f 7265 6c61 7469 7665  resolve_relative
+00029760: 5f6b 6579 7360 2c20 3a70 793a 6675 6e63  _keys`, :py:func
+00029770: 3a60 7e2e 7574 696c 732e 726f 6d61 6e5f  :`~.utils.roman_
+00029780: 6e75 6d65 7261 6c32 6669 6674 6873 602c  numeral2fifths`,
+00029790: 0a20 2020 203a 7079 3a66 756e 633a 607e  .    :py:func:`~
+000297a0: 2e75 7469 6c73 2e73 6f72 745f 7470 6373  .utils.sort_tpcs
+000297b0: 602c 203a 7079 3a66 756e 633a 607e 2e75  `, :py:func:`~.u
+000297c0: 7469 6c73 2e73 7472 5f69 735f 6d69 6e6f  tils.str_is_mino
+000297d0: 7260 0a0a 2020 2020 5061 7261 6d65 7465  r`..    Paramete
+000297e0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+000297f0: 2d0a 2020 2020 6e75 6d65 7261 6c3a 203a  -.    numeral: :
+00029800: 6f62 6a3a 6073 7472 600a 2020 2020 2020  obj:`str`.      
+00029810: 2020 526f 6d61 6e20 6e75 6d65 7261 6c20    Roman numeral 
+00029820: 6f66 2074 6865 2063 686f 7264 2773 2072  of the chord's r
+00029830: 6f6f 740a 2020 2020 666f 726d 3a20 7b4e  oot.    form: {N
+00029840: 6f6e 652c 2027 4d27 2c20 276f 272c 2027  one, 'M', 'o', '
+00029850: 2b27 2027 2527 7d2c 206f 7074 696f 6e61  +' '%'}, optiona
+00029860: 6c0a 2020 2020 2020 2020 496e 6469 6361  l.        Indica
+00029870: 7465 7320 7468 6520 6368 6f72 6420 7479  tes the chord ty
+00029880: 7065 2069 6620 6e6f 7420 6120 6d61 6a6f  pe if not a majo
+00029890: 7220 6f72 206d 696e 6f72 2074 7269 6164  r or minor triad
+000298a0: 2028 666f 7220 7768 6963 6820 6060 666f   (for which ``fo
+000298b0: 726d 6060 2069 7320 4e6f 6e65 292e 0a20  rm`` is None).. 
+000298c0: 2020 2020 2020 2027 2527 2061 6e64 2027         '%' and '
+000298d0: 4d27 2063 616e 206f 6e6c 7920 6f63 6375  M' can only occu
+000298e0: 7220 6173 2074 6574 7261 6473 2c20 6e6f  r as tetrads, no
+000298f0: 7420 6173 2074 7269 6164 732e 0a20 2020  t as triads..   
+00029900: 2066 6967 6261 7373 3a20 7b4e 6f6e 652c   figbass: {None,
+00029910: 2027 3627 2c20 2736 3427 2c20 2737 272c   '6', '64', '7',
+00029920: 2027 3635 272c 2027 3433 272c 2027 3227   '65', '43', '2'
+00029930: 7d2c 206f 7074 696f 6e61 6c0a 2020 2020  }, optional.    
+00029940: 2020 2020 496e 6469 6361 7465 7320 6368      Indicates ch
+00029950: 6f72 6427 7320 696e 7665 7273 696f 6e2e  ord's inversion.
+00029960: 2050 6173 7320 4e6f 6e65 2066 6f72 2074   Pass None for t
+00029970: 7269 6164 2072 6f6f 7420 706f 7369 7469  riad root positi
+00029980: 6f6e 2e0a 2020 2020 6368 616e 6765 733a  on..    changes:
+00029990: 203a 6f62 6a3a 6073 7472 602c 206f 7074   :obj:`str`, opt
+000299a0: 696f 6e61 6c0a 2020 2020 2020 2020 4164  ional.        Ad
+000299b0: 6465 6420 7374 6570 7320 7375 6368 2061  ded steps such a
+000299c0: 7320 272b 3627 206f 7220 7375 7370 656e  s '+6' or suspen
+000299d0: 7369 6f6e 7320 7375 6368 2061 7320 2734  sions such as '4
+000299e0: 2720 6f72 2061 6e79 2063 6f6d 6269 6e61  ' or any combina
+000299f0: 7469 6f6e 2073 7563 6820 6173 2028 392b  tion such as (9+
+00029a00: 3634 292e 0a20 2020 2020 2020 204e 756d  64)..        Num
+00029a10: 6265 7273 206e 6565 6420 746f 2062 6520  bers need to be 
+00029a20: 696e 2064 6573 6365 6e64 696e 6720 6f72  in descending or
+00029a30: 6465 722e 0a20 2020 2072 656c 6174 6976  der..    relativ
+00029a40: 6572 6f6f 743a 203a 6f62 6a3a 6073 7472  eroot: :obj:`str
+00029a50: 602c 206f 7074 696f 6e61 6c0a 2020 2020  `, optional.    
+00029a60: 2020 2020 5061 7373 2061 2052 6f6d 616e      Pass a Roman
+00029a70: 2073 6361 6c65 2064 6567 7265 6520 6966   scale degree if
+00029a80: 2060 6e75 6d65 7261 6c60 2069 7320 746f   `numeral` is to
+00029a90: 2062 6520 6170 706c 6965 6420 746f 2061   be applied to a
+00029aa0: 2064 6966 6665 7265 6e74 2073 6361 6c65   different scale
+00029ab0: 0a20 2020 2020 2020 2064 6567 7265 6520  .        degree 
+00029ac0: 6f66 2074 6865 206c 6f63 616c 206b 6579  of the local key
+00029ad0: 2c20 6173 2069 6e20 2756 3635 2f56 270a  , as in 'V65/V'.
+00029ae0: 2020 2020 6b65 7920 3a20 3a6f 626a 3a60      key : :obj:`
+00029af0: 7374 7260 206f 7220 3a6f 626a 3a60 696e  str` or :obj:`in
+00029b00: 7460 2c20 6f70 7469 6f6e 616c 0a20 2020  t`, optional.   
+00029b10: 2020 2020 2054 6865 206c 6f63 616c 206b       The local k
+00029b20: 6579 2065 7870 7265 7373 6564 2061 7320  ey expressed as 
+00029b30: 7468 6520 726f 6f74 2773 206e 6f74 6520  the root's note 
+00029b40: 6e61 6d65 206f 7220 6120 746f 6e61 6c20  name or a tonal 
+00029b50: 7069 7463 6820 636c 6173 732e 0a20 2020  pitch class..   
+00029b60: 2020 2020 2049 6620 6974 2069 7320 6120       If it is a 
+00029b70: 6e61 6d65 2061 6e64 2060 6d69 6e6f 7260  name and `minor`
+00029b80: 2069 7320 604e 6f6e 6560 2c20 7570 7065   is `None`, uppe
+00029b90: 7263 6173 6520 6d65 616e 7320 6d61 6a6f  rcase means majo
+00029ba0: 7220 616e 6420 6c6f 7765 7263 6173 6520  r and lowercase 
+00029bb0: 6d69 6e6f 722e 0a20 2020 2020 2020 2049  minor..        I
+00029bc0: 6620 6974 2069 7320 6120 746f 6e61 6c20  f it is a tonal 
+00029bd0: 7069 7463 6820 636c 6173 732c 2060 6d69  pitch class, `mi
+00029be0: 6e6f 7260 206e 6565 6473 2074 6f20 6265  nor` needs to be
+00029bf0: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
+00029c00: 6d69 6e6f 7220 3a20 3a6f 626a 3a60 626f  minor : :obj:`bo
+00029c10: 6f6c 602c 206f 7074 696f 6e61 6c0a 2020  ol`, optional.  
+00029c20: 2020 2020 2020 5061 7373 2054 7275 6520        Pass True 
+00029c30: 666f 7220 6d69 6e6f 7220 616e 6420 4661  for minor and Fa
+00029c40: 6c73 6520 666f 7220 6d61 6a6f 722e 2043  lse for major. C
+00029c50: 616e 2062 6520 6f6d 6974 7465 6420 6966  an be omitted if
+00029c60: 2060 6b65 7960 2069 7320 6120 6e6f 7465   `key` is a note
+00029c70: 206e 616d 652e 0a20 2020 2020 2020 2054   name..        T
+00029c80: 6869 7320 6166 6665 6374 7320 6361 6c63  his affects calc
+00029c90: 756c 6174 696f 6e20 6f66 2063 686f 7264  ulation of chord
+00029ca0: 7320 7265 6c61 7465 6420 746f 2049 4949  s related to III
+00029cb0: 2c20 5649 2061 6e64 2056 4949 2e0a 2020  , VI and VII..  
+00029cc0: 2020 6d65 7267 655f 746f 6e65 7320 3a20    merge_tones : 
+00029cd0: 3a6f 626a 3a60 626f 6f6c 602c 206f 7074  :obj:`bool`, opt
+00029ce0: 696f 6e61 6c0a 2020 2020 2020 2020 5061  ional.        Pa
+00029cf0: 7373 2046 616c 7365 2069 6620 796f 7520  ss False if you 
+00029d00: 7761 6e74 2074 6865 2066 756e 6374 696f  want the functio
+00029d10: 6e20 746f 2072 6574 7572 6e20 7477 6f20  n to return two 
+00029d20: 7475 706c 6573 2c20 6f6e 6520 7769 7468  tuples, one with
+00029d30: 2028 706f 7465 6e74 6961 6c6c 7920 7375   (potentially su
+00029d40: 7370 656e 6465 6429 0a20 2020 2020 2020  spended).       
+00029d50: 2063 686f 7264 2074 6f6e 6573 2061 6e64   chord tones and
+00029d60: 206f 6e65 2077 6974 6820 6164 6465 6420   one with added 
+00029d70: 6e6f 7465 732e 0a20 2020 2062 6173 735f  notes..    bass_
+00029d80: 6f6e 6c79 203a 203a 6f62 6a3a 6062 6f6f  only : :obj:`boo
+00029d90: 6c60 2c20 6f70 7469 6f6e 616c 0a20 2020  l`, optional.   
+00029da0: 2020 2020 2052 6574 7572 6e20 6f6e 6c79       Return only
+00029db0: 2074 6865 2062 6173 7320 6e6f 7465 2069   the bass note i
+00029dc0: 6e73 7465 6164 206f 6620 616c 6c20 6368  nstead of all ch
+00029dd0: 6f72 6420 746f 6e65 732e 0a20 2020 206d  ord tones..    m
+00029de0: 6320 3a20 696e 7420 6f72 2073 7472 0a20  c : int or str. 
+00029df0: 2020 2020 2020 2050 6173 7320 6d65 6173         Pass meas
+00029e00: 7572 6520 636f 756e 7420 746f 2064 6973  ure count to dis
+00029e10: 706c 6179 2069 7420 696e 2077 6172 6e69  play it in warni
+00029e20: 6e67 732e 0a0a 2020 2020 2222 220a 2020  ngs...    """.  
+00029e30: 2020 6966 2070 642e 6973 6e75 6c6c 286e    if pd.isnull(n
+00029e40: 756d 6572 616c 2920 6f72 206e 756d 6572  umeral) or numer
+00029e50: 616c 203d 3d20 2740 6e6f 6e65 273a 0a20  al == '@none':. 
+00029e60: 2020 2020 2020 2069 6620 6261 7373 5f6f         if bass_o
+00029e70: 6e6c 7920 6f72 206d 6572 6765 5f74 6f6e  nly or merge_ton
+00029e80: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00029e90: 7265 7475 726e 2070 642e 4e41 0a20 2020  return pd.NA.   
+00029ea0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00029eb0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+00029ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ed0: 2763 686f 7264 5f74 6f6e 6573 273a 2070  'chord_tones': p
+00029ee0: 642e 4e41 2c0a 2020 2020 2020 2020 2020  d.NA,.          
+00029ef0: 2020 2020 2020 2761 6464 6564 5f74 6f6e        'added_ton
+00029f00: 6573 273a 2070 642e 4e41 2c0a 2020 2020  es': pd.NA,.    
+00029f10: 2020 2020 2020 2020 2020 2020 2772 6f6f              'roo
+00029f20: 7427 3a20 7064 2e4e 412c 0a20 2020 2020  t': pd.NA,.     
+00029f30: 2020 2020 2020 207d 0a20 2020 2066 6f72         }.    for
+00029f40: 6d2c 2066 6967 6261 7373 2c20 6368 616e  m, figbass, chan
+00029f50: 6765 732c 2072 656c 6174 6976 6572 6f6f  ges, relativeroo
+00029f60: 7420 3d20 7475 706c 6528 0a20 2020 2020  t = tuple(.     
+00029f70: 2020 2027 2720 6966 2070 642e 6973 6e75     '' if pd.isnu
+00029f80: 6c6c 2876 616c 2920 656c 7365 2076 616c  ll(val) else val
+00029f90: 2066 6f72 2076 616c 2069 6e20 2866 6f72   for val in (for
+00029fa0: 6d2c 2066 6967 6261 7373 2c20 6368 616e  m, figbass, chan
+00029fb0: 6765 732c 2072 656c 6174 6976 6572 6f6f  ges, relativeroo
+00029fc0: 7429 290a 2020 2020 6c61 6265 6c20 3d20  t)).    label = 
+00029fd0: 6622 7b6e 756d 6572 616c 7d7b 666f 726d  f"{numeral}{form
+00029fe0: 7d7b 6669 6762 6173 737d 7b27 2827 202b  }{figbass}{'(' +
+00029ff0: 2063 6861 6e67 6573 202b 2027 2927 2069   changes + ')' i
+0002a000: 6620 6368 616e 6765 7320 213d 2027 2720  f changes != '' 
+0002a010: 656c 7365 2027 277d 7b27 2f27 202b 2072  else ''}{'/' + r
+0002a020: 656c 6174 6976 6572 6f6f 7420 6966 2072  elativeroot if r
+0002a030: 656c 6174 6976 6572 6f6f 7420 213d 2027  elativeroot != '
+0002a040: 2720 656c 7365 2027 277d 220a 2020 2020  ' else ''}".    
+0002a050: 4d43 203d 2027 2720 6966 206d 6320 6973  MC = '' if mc is
+0002a060: 204e 6f6e 6520 656c 7365 2066 274d 4320   None else f'MC 
+0002a070: 7b6d 637d 3a20 270a 2020 2020 6966 206d  {mc}: '.    if m
+0002a080: 696e 6f72 2069 7320 4e6f 6e65 3a0a 2020  inor is None:.  
+0002a090: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0002a0a0: 2020 2020 2020 206d 696e 6f72 203d 2073         minor = s
+0002a0b0: 7472 5f69 735f 6d69 6e6f 7228 6b65 792c  tr_is_minor(key,
+0002a0c0: 2069 735f 6e61 6d65 3d54 7275 6529 0a20   is_name=True). 
+0002a0d0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0002a0e0: 722e 6465 6275 6728 6622 4d6f 6465 2069  r.debug(f"Mode i
+0002a0f0: 6e66 6572 7265 6420 6672 6f6d 207b 6b65  nferred from {ke
+0002a100: 797d 2e22 290a 2020 2020 2020 2020 6578  y}.").        ex
+0002a110: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
+0002a120: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0002a130: 6520 5661 6c75 6545 7272 6f72 2866 2249  e ValueError(f"I
+0002a140: 6620 7061 7261 6d65 7465 7220 276d 696e  f parameter 'min
+0002a150: 6f72 2720 6973 206e 6f74 2073 7065 6369  or' is not speci
+0002a160: 6669 6564 2c20 276b 6579 2720 6e65 6564  fied, 'key' need
+0002a170: 7320 746f 2062 6520 6120 7374 7269 6e67  s to be a string
+0002a180: 2c20 6e6f 7420 7b6b 6579 7d22 290a 0a20  , not {key}").. 
+0002a190: 2020 206b 6579 203d 206e 616d 6532 6669     key = name2fi
+0002a1a0: 6674 6873 286b 6579 2c20 6c6f 6767 6572  fths(key, logger
+0002a1b0: 3d6c 6f67 6765 7229 0a0a 2020 2020 6966  =logger)..    if
+0002a1c0: 2066 6f72 6d20 696e 205b 2725 272c 2027   form in ['%', '
+0002a1d0: 4d27 2c20 272b 4d27 5d3a 0a20 2020 2020  M', '+M']:.     
+0002a1e0: 2020 2061 7373 6572 7420 6669 6762 6173     assert figbas
+0002a1f0: 7320 696e 205b 2737 272c 2027 3635 272c  s in ['7', '65',
+0002a200: 2027 3433 272c 0a20 2020 2020 2020 2020   '43',.         
+0002a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a220: 2020 2732 275d 2c20 6622 7b4d 437d 7b6c    '2'], f"{MC}{l
+0002a230: 6162 656c 7d3a 207b 666f 726d 7d20 7265  abel}: {form} re
+0002a240: 7175 6972 6573 2066 6967 6261 7373 2028  quires figbass (
+0002a250: 372c 2036 352c 2034 332c 206f 7220 3229  7, 65, 43, or 2)
+0002a260: 2073 696e 6365 2069 7420 7370 6563 6966   since it specif
+0002a270: 6965 7320 6120 6368 6f72 6427 7320 7365  ies a chord's se
+0002a280: 7665 6e74 682e 220a 0a20 2020 2069 6620  venth."..    if 
+0002a290: 7265 6c61 7469 7665 726f 6f74 2021 3d20  relativeroot != 
+0002a2a0: 2727 3a0a 2020 2020 2020 2020 7265 736f  '':.        reso
+0002a2b0: 6c76 6564 203d 2072 6573 6f6c 7665 5f72  lved = resolve_r
+0002a2c0: 656c 6174 6976 655f 6b65 7973 2872 656c  elative_keys(rel
+0002a2d0: 6174 6976 6572 6f6f 742c 206d 696e 6f72  ativeroot, minor
+0002a2e0: 2c20 6c6f 6767 6572 3d6c 6f67 6765 7229  , logger=logger)
+0002a2f0: 0a20 2020 2020 2020 2072 656c 5f6d 696e  .        rel_min
+0002a300: 6f72 203d 2073 7472 5f69 735f 6d69 6e6f  or = str_is_mino
+0002a310: 7228 7265 736f 6c76 6564 2c20 6973 5f6e  r(resolved, is_n
+0002a320: 616d 653d 4661 6c73 6529 0a20 2020 2020  ame=False).     
+0002a330: 2020 2074 7261 6e73 7020 3d20 726f 6d61     transp = roma
+0002a340: 6e5f 6e75 6d65 7261 6c32 6669 6674 6873  n_numeral2fifths
+0002a350: 2872 6573 6f6c 7665 642c 206d 696e 6f72  (resolved, minor
+0002a360: 2c20 6c6f 6767 6572 3d6c 6f67 6765 7229  , logger=logger)
+0002a370: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0002a380: 6465 6275 6728 0a20 2020 2020 2020 2020  debug(.         
+0002a390: 2020 2066 227b 4d43 7d43 686f 7264 2061     f"{MC}Chord a
+0002a3a0: 7070 6c69 6564 2074 6f20 7b72 656c 6174  pplied to {relat
+0002a3b0: 6976 6572 6f6f 747d 2e20 5468 6572 6566  iveroot}. Theref
+0002a3c0: 6f72 6520 7472 616e 7370 6f73 696e 6720  ore transposing 
+0002a3d0: 6974 2062 7920 7b74 7261 6e73 707d 2066  it by {transp} f
+0002a3e0: 6966 7468 732e 2229 0a20 2020 2020 2020  ifths.").       
+0002a3f0: 2072 6574 7572 6e20 6665 6174 7572 6573   return features
+0002a400: 3274 7063 7328 6e75 6d65 7261 6c3d 6e75  2tpcs(numeral=nu
+0002a410: 6d65 7261 6c2c 2066 6f72 6d3d 666f 726d  meral, form=form
+0002a420: 2c20 6669 6762 6173 733d 6669 6762 6173  , figbass=figbas
+0002a430: 732c 2072 656c 6174 6976 6572 6f6f 743d  s, relativeroot=
+0002a440: 4e6f 6e65 2c20 6368 616e 6765 733d 6368  None, changes=ch
+0002a450: 616e 6765 732c 0a20 2020 2020 2020 2020  anges,.         
+0002a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a470: 2020 2020 6b65 793d 6b65 7920 2b20 7472      key=key + tr
+0002a480: 616e 7370 2c20 6d69 6e6f 723d 7265 6c5f  ansp, minor=rel_
+0002a490: 6d69 6e6f 722c 206d 6572 6765 5f74 6f6e  minor, merge_ton
+0002a4a0: 6573 3d6d 6572 6765 5f74 6f6e 6573 2c20  es=merge_tones, 
+0002a4b0: 6261 7373 5f6f 6e6c 793d 6261 7373 5f6f  bass_only=bass_o
+0002a4c0: 6e6c 792c 206d 633d 6d63 2c0a 2020 2020  nly, mc=mc,.    
+0002a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a4e0: 2020 2020 2020 2020 206c 6f67 6765 723d           logger=
+0002a4f0: 6c6f 6767 6572 290a 0a20 2020 2069 6620  logger)..    if 
+0002a500: 6e75 6d65 7261 6c2e 6c6f 7765 7228 2920  numeral.lower() 
+0002a510: 3d3d 2027 2376 6969 2720 616e 6420 6e6f  == '#vii' and no
+0002a520: 7420 6d69 6e6f 723a 0a20 2020 2020 2020  t minor:.       
+0002a530: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+0002a540: 6622 7b4d 437d 7b6e 756d 6572 616c 7d20  f"{MC}{numeral} 
+0002a550: 696e 206d 616a 6f72 2063 6f6e 7465 7874  in major context
+0002a560: 2063 6f72 7265 6374 6564 2074 6f20 7b6e   corrected to {n
+0002a570: 756d 6572 616c 5b31 3a5d 7d2e 222c 0a20  umeral[1:]}.",. 
+0002a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a590: 2020 2020 2020 6578 7472 613d 7b27 6d65        extra={'me
+0002a5a0: 7373 6167 655f 6964 273a 2028 3237 2c20  ssage_id': (27, 
+0002a5b0: 4d43 297d 290a 2020 2020 2020 2020 6e75  MC)}).        nu
+0002a5c0: 6d65 7261 6c20 3d20 6e75 6d65 7261 6c5b  meral = numeral[
+0002a5d0: 313a 5d0a 0a20 2020 2072 6f6f 745f 616c  1:]..    root_al
+0002a5e0: 7465 7261 7469 6f6e 2c20 6e75 6d5f 6465  teration, num_de
+0002a5f0: 6772 6565 203d 2073 706c 6974 5f73 6361  gree = split_sca
+0002a600: 6c65 5f64 6567 7265 6528 6e75 6d65 7261  le_degree(numera
+0002a610: 6c2c 2063 6f75 6e74 3d54 7275 652c 206c  l, count=True, l
+0002a620: 6f67 6765 723d 6c6f 6767 6572 290a 0a20  ogger=logger).. 
+0002a630: 2020 2023 2062 7569 6c64 2032 2d6f 6374     # build 2-oct
+0002a640: 6176 6520 6469 6174 6f6e 6963 2073 6361  ave diatonic sca
+0002a650: 6c65 206f 6e20 4320 6d61 6a6f 722f 6d69  le on C major/mi
+0002a660: 6e6f 720a 2020 2020 726f 6f74 203d 205b  nor.    root = [
+0002a670: 2749 272c 2027 4949 272c 2027 4949 4927  'I', 'II', 'III'
+0002a680: 2c20 2749 5627 2c20 2756 272c 2027 5649  , 'IV', 'V', 'VI
+0002a690: 272c 2027 5649 4927 5d2e 696e 6465 7828  ', 'VII'].index(
+0002a6a0: 6e75 6d5f 6465 6772 6565 2e75 7070 6572  num_degree.upper
+0002a6b0: 2829 290a 2020 2020 7470 6373 203d 2032  ()).    tpcs = 2
+0002a6c0: 202a 205b 6920 2b20 6b65 7920 666f 7220   * [i + key for 
+0002a6d0: 6920 696e 2028 302c 2032 2c20 2d33 2c20  i in (0, 2, -3, 
+0002a6e0: 2d31 2c20 312c 202d 342c 202d 3229 5d20  -1, 1, -4, -2)] 
+0002a6f0: 6966 206d 696e 6f72 2065 6c73 6520 3220  if minor else 2 
+0002a700: 2a20 5b69 202b 206b 6579 2066 6f72 2069  * [i + key for i
+0002a710: 2069 6e20 2830 2c20 322c 2034 2c20 2d31   in (0, 2, 4, -1
+0002a720: 2c20 312c 2033 2c20 3529 5d0a 2020 2020  , 1, 3, 5)].    
+0002a730: 2320 7374 6172 7469 6e67 2074 6865 2073  # starting the s
+0002a740: 6361 6c65 2066 726f 6d20 6368 6f72 6420  cale from chord 
+0002a750: 726f 6f74 2c20 692e 652e 2072 6f6f 7420  root, i.e. root 
+0002a760: 7769 6c6c 2062 6520 7470 6373 5b30 5d2c  will be tpcs[0],
+0002a770: 2074 6865 2063 686f 7264 2773 2073 6576   the chord's sev
+0002a780: 656e 7468 2074 7063 735b 365d 2065 7463  enth tpcs[6] etc
+0002a790: 2e0a 2020 2020 7470 6373 203d 2074 7063  ..    tpcs = tpc
+0002a7a0: 735b 726f 6f74 3a5d 202b 2074 7063 735b  s[root:] + tpcs[
+0002a7b0: 3a72 6f6f 745d 0a20 2020 2072 6f6f 7420  :root].    root 
+0002a7c0: 3d20 7470 6373 5b30 5d20 2b20 3720 2a20  = tpcs[0] + 7 * 
+0002a7d0: 726f 6f74 5f61 6c74 6572 6174 696f 6e0a  root_alteration.
+0002a7e0: 2020 2020 7470 6373 5b30 5d20 3d20 726f      tpcs[0] = ro
+0002a7f0: 6f74 2020 2320 6f63 7461 7665 2073 7461  ot  # octave sta
+0002a800: 7973 2064 6961 746f 6e69 632c 2069 7320  ys diatonic, is 
+0002a810: 6e6f 7420 616c 7465 7265 640a 2020 2020  not altered.    
+0002a820: 236c 6f67 6765 722e 6465 6275 6728 6622  #logger.debug(f"
+0002a830: 7b6e 756d 5f64 6567 7265 657d 3a20 5468  {num_degree}: Th
+0002a840: 6520 7b27 6d69 6e6f 7227 2069 6620 6d69  e {'minor' if mi
+0002a850: 6e6f 7220 656c 7365 2027 6d61 6a6f 7227  nor else 'major'
+0002a860: 7d20 7363 616c 6520 7374 6172 7469 6e67  } scale starting
+0002a870: 2066 726f 6d20 7468 6520 726f 6f74 3a20   from the root: 
+0002a880: 7b74 7063 737d 2229 0a0a 2020 2020 6465  {tpcs}")..    de
+0002a890: 6620 7365 745f 6976 2863 686f 7264 5f69  f set_iv(chord_i
+0002a8a0: 6e74 6572 7661 6c2c 2069 6e74 6572 7661  nterval, interva
+0002a8b0: 6c5f 7369 7a65 293a 0a20 2020 2020 2020  l_size):.       
+0002a8c0: 2022 2222 2041 6464 2074 6f20 7468 6520   """ Add to the 
+0002a8d0: 696e 7465 7276 616c 206f 6620 6120 6769  interval of a gi
+0002a8e0: 7665 6e20 6368 6f72 6420 696e 7465 7276  ven chord interv
+0002a8f0: 616c 2069 6e20 6074 7063 7360 2028 626f  al in `tpcs` (bo
+0002a900: 7468 2076 6965 7765 6420 6672 6f6d 2074  th viewed from t
+0002a910: 6865 2072 6f6f 7420 6e6f 7465 292e 0a0a  he root note)...
+0002a920: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0002a930: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0002a940: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6368  -----.        ch
+0002a950: 6f72 645f 696e 7465 7276 616c 203a 203a  ord_interval : :
+0002a960: 6f62 6a3a 6069 6e74 600a 2020 2020 2020  obj:`int`.      
+0002a970: 2020 2020 2020 5061 7373 2030 2066 6f72        Pass 0 for
+0002a980: 2074 6865 2072 6f6f 7420 6e6f 7465 2c20   the root note, 
+0002a990: 3220 666f 7220 7468 6520 7468 6972 642c  2 for the third,
+0002a9a0: 2038 2066 6f72 2074 6865 206e 696e 7468   8 for the ninth
+0002a9b0: 2065 7463 2e0a 2020 2020 2020 2020 696e   etc..        in
+0002a9c0: 7465 7276 616c 5f73 697a 6520 3a20 3a6f  terval_size : :o
+0002a9d0: 626a 3a60 696e 7460 0a20 2020 2020 2020  bj:`int`.       
+0002a9e0: 2020 2020 2053 7461 636b 2d6f 662d 6669       Stack-of-fi
+0002a9f0: 6674 6873 2069 6e74 6572 7661 6c2e 0a20  fths interval.. 
+0002aa00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0002aa10: 2020 206e 6f6e 6c6f 6361 6c20 7470 6373     nonlocal tpcs
+0002aa20: 2c20 726f 6f74 0a20 2020 2020 2020 2069  , root.        i
+0002aa30: 7620 3d20 726f 6f74 202b 2069 6e74 6572  v = root + inter
+0002aa40: 7661 6c5f 7369 7a65 0a20 2020 2020 2020  val_size.       
+0002aa50: 2074 7063 735b 6368 6f72 645f 696e 7465   tpcs[chord_inte
+0002aa60: 7276 616c 5d20 3d20 6976 0a20 2020 2020  rval] = iv.     
+0002aa70: 2020 2074 7063 735b 6368 6f72 645f 696e     tpcs[chord_in
+0002aa80: 7465 7276 616c 202b 2037 5d20 3d20 6976  terval + 7] = iv
+0002aa90: 0a0a 2020 2020 6973 5f74 7269 6164 203d  ..    is_triad =
+0002aaa0: 2066 6967 6261 7373 2069 6e20 5b27 272c   figbass in ['',
+0002aab0: 2027 3627 2c20 2736 3427 5d0a 2020 2020   '6', '64'].    
+0002aac0: 6973 5f73 6576 656e 7468 5f63 686f 7264  is_seventh_chord
+0002aad0: 203d 2066 6967 6261 7373 2069 6e20 5b27   = figbass in ['
+0002aae0: 3727 2c20 2736 3527 2c20 2734 3327 2c20  7', '65', '43', 
+0002aaf0: 2732 275d 0a20 2020 2069 6620 6e6f 7420  '2'].    if not 
+0002ab00: 6973 5f74 7269 6164 2061 6e64 206e 6f74  is_triad and not
+0002ab10: 2069 735f 7365 7665 6e74 685f 6368 6f72   is_seventh_chor
+0002ab20: 643a 0a20 2020 2020 2020 2072 6169 7365  d:.        raise
+0002ab30: 2056 616c 7565 4572 726f 7228 6622 7b4d   ValueError(f"{M
+0002ab40: 437d 7b66 6967 6261 7373 7d20 6973 206e  C}{figbass} is n
+0002ab50: 6f74 2061 2076 616c 6964 2063 686f 7264  ot a valid chord
+0002ab60: 2069 6e76 6572 7369 6f6e 2e22 290a 0a20   inversion.").. 
+0002ab70: 2020 2069 6620 666f 726d 203d 3d20 276f     if form == 'o
+0002ab80: 273a 0a20 2020 2020 2020 2073 6574 5f69  ':.        set_i
+0002ab90: 7628 322c 202d 3329 0a20 2020 2020 2020  v(2, -3).       
+0002aba0: 2073 6574 5f69 7628 342c 202d 3629 0a20   set_iv(4, -6). 
+0002abb0: 2020 2020 2020 2069 6620 6973 5f73 6576         if is_sev
+0002abc0: 656e 7468 5f63 686f 7264 3a0a 2020 2020  enth_chord:.    
+0002abd0: 2020 2020 2020 2020 7365 745f 6976 2836          set_iv(6
+0002abe0: 2c20 2d39 290a 2020 2020 656c 6966 2066  , -9).    elif f
+0002abf0: 6f72 6d20 3d3d 2027 2527 3a0a 2020 2020  orm == '%':.    
+0002ac00: 2020 2020 7365 745f 6976 2832 2c20 2d33      set_iv(2, -3
+0002ac10: 290a 2020 2020 2020 2020 7365 745f 6976  ).        set_iv
+0002ac20: 2834 2c20 2d36 290a 2020 2020 2020 2020  (4, -6).        
+0002ac30: 7365 745f 6976 2836 2c20 2d32 290a 2020  set_iv(6, -2).  
+0002ac40: 2020 656c 6966 2066 6f72 6d20 3d3d 2027    elif form == '
+0002ac50: 2b27 3a0a 2020 2020 2020 2020 7365 745f  +':.        set_
+0002ac60: 6976 2832 2c20 3429 0a20 2020 2020 2020  iv(2, 4).       
+0002ac70: 2073 6574 5f69 7628 342c 2038 290a 2020   set_iv(4, 8).  
+0002ac80: 2020 2020 2020 6966 2069 735f 7365 7665        if is_seve
+0002ac90: 6e74 685f 6368 6f72 643a 0a20 2020 2020  nth_chord:.     
+0002aca0: 2020 2020 2020 2073 6574 5f69 7628 362c         set_iv(6,
+0002acb0: 202d 3229 0a20 2020 2065 6c69 6620 666f   -2).    elif fo
+0002acc0: 726d 203d 3d20 272b 4d27 3a0a 2020 2020  rm == '+M':.    
+0002acd0: 2020 2020 7365 745f 6976 2832 2c20 3429      set_iv(2, 4)
+0002ace0: 0a20 2020 2020 2020 2073 6574 5f69 7628  .        set_iv(
+0002acf0: 342c 2038 290a 2020 2020 2020 2020 7365  4, 8).        se
+0002ad00: 745f 6976 2836 2c20 3529 0a20 2020 2065  t_iv(6, 5).    e
+0002ad10: 6c73 653a 2020 2320 7472 6961 6420 7769  lse:  # triad wi
+0002ad20: 7468 206f 7220 7769 7468 6f75 7420 6d61  th or without ma
+0002ad30: 6a6f 7220 6f72 206d 696e 6f72 2073 6576  jor or minor sev
+0002ad40: 656e 0a20 2020 2020 2020 2073 6574 5f69  en.        set_i
+0002ad50: 7628 342c 2031 290a 2020 2020 2020 2020  v(4, 1).        
+0002ad60: 6966 206e 756d 5f64 6567 7265 652e 6973  if num_degree.is
+0002ad70: 7570 7065 7228 293a 0a20 2020 2020 2020  upper():.       
+0002ad80: 2020 2020 2073 6574 5f69 7628 322c 2034       set_iv(2, 4
+0002ad90: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0002ada0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+0002adb0: 6976 2832 2c20 2d33 290a 2020 2020 2020  iv(2, -3).      
+0002adc0: 2020 6966 2066 6f72 6d20 3d3d 2027 4d27    if form == 'M'
+0002add0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002ade0: 745f 6976 2836 2c20 3529 0a20 2020 2020  t_iv(6, 5).     
+0002adf0: 2020 2065 6c69 6620 6973 5f73 6576 656e     elif is_seven
+0002ae00: 7468 5f63 686f 7264 3a0a 2020 2020 2020  th_chord:.      
+0002ae10: 2020 2020 2020 7365 745f 6976 2836 2c20        set_iv(6, 
+0002ae20: 2d32 290a 0a20 2020 2074 6f6e 655f 6675  -2)..    tone_fu
+0002ae30: 6e63 7469 6f6e 7320 3d20 2830 2c20 322c  nctions = (0, 2,
+0002ae40: 2034 2c20 3629 2069 6620 6973 5f73 6576   4, 6) if is_sev
+0002ae50: 656e 7468 5f63 686f 7264 2065 6c73 6520  enth_chord else 
+0002ae60: 2830 2c20 322c 2034 290a 2020 2020 726f  (0, 2, 4).    ro
+0002ae70: 6f74 5f70 6f73 6974 696f 6e20 3d20 7b69  ot_position = {i
+0002ae80: 3a20 5b74 7063 735b 695d 5d20 666f 7220  : [tpcs[i]] for 
+0002ae90: 6920 696e 2074 6f6e 655f 6675 6e63 7469  i in tone_functi
+0002aea0: 6f6e 737d 0a20 2020 2072 6570 6c61 6365  ons}.    replace
+0002aeb0: 6d65 6e74 7320 203d 207b 693a 205b 5d20  ments  = {i: [] 
+0002aec0: 666f 7220 6920 696e 2074 6f6e 655f 6675  for i in tone_fu
+0002aed0: 6e63 7469 6f6e 737d 0a0a 2020 2020 6465  nctions}..    de
+0002aee0: 6620 7265 706c 6163 655f 6368 6f72 645f  f replace_chord_
+0002aef0: 746f 6e65 2877 6869 6368 2c20 6279 293a  tone(which, by):
+0002af00: 0a20 2020 2020 2020 206e 6f6e 6c6f 6361  .        nonloca
+0002af10: 6c20 726f 6f74 5f70 6f73 6974 696f 6e2c  l root_position,
+0002af20: 2072 6570 6c61 6365 6d65 6e74 730a 2020   replacements.  
+0002af30: 2020 2020 2020 6966 2077 6869 6368 2069        if which i
+0002af40: 6e20 726f 6f74 5f70 6f73 6974 696f 6e3a  n root_position:
+0002af50: 0a20 2020 2020 2020 2020 2020 2072 6f6f  .            roo
+0002af60: 745f 706f 7369 7469 6f6e 5b77 6869 6368  t_position[which
+0002af70: 5d20 3d20 5b5d 0a20 2020 2020 2020 2020  ] = [].         
+0002af80: 2020 2072 6570 6c61 6365 6d65 6e74 735b     replacements[
+0002af90: 7768 6963 685d 2e69 6e73 6572 7428 302c  which].insert(0,
+0002afa0: 2062 7929 0a20 2020 2020 2020 2065 6c73   by).        els
+0002afb0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+0002afc0: 6f67 6765 722e 7761 726e 696e 6728 6622  ogger.warning(f"
+0002afd0: 4f6e 6c79 2063 686f 7264 2074 6f6e 6573  Only chord tones
+0002afe0: 205b 302c 322c 342c 2836 295d 2063 616e   [0,2,4,(6)] can
+0002aff0: 2062 6520 7265 706c 6163 6564 2c20 6e6f   be replaced, no
+0002b000: 7420 7b77 6869 6368 7d22 290a 0a20 2020  t {which}")..   
+0002b010: 2023 2061 7070 6c79 2063 6861 6e67 6573   # apply changes
+0002b020: 0a20 2020 2061 6c74 7320 3d20 6368 616e  .    alts = chan
+0002b030: 6765 7332 6c69 7374 2863 6861 6e67 6573  ges2list(changes
+0002b040: 2c20 736f 7274 3d46 616c 7365 290a 2020  , sort=False).  
+0002b050: 2020 6164 6465 645f 6e6f 7465 7320 3d20    added_notes = 
+0002b060: 5b5d 0a20 2020 2066 6f72 2066 756c 6c2c  [].    for full,
+0002b070: 2061 6464 5f72 656d 6f76 652c 2061 6363   add_remove, acc
+0002b080: 2c20 6368 6f72 645f 696e 7465 7276 616c  , chord_interval
+0002b090: 2069 6e20 616c 7473 3a0a 2020 2020 2020   in alts:.      
+0002b0a0: 2020 6164 6465 6420 3d20 6164 645f 7265    added = add_re
+0002b0b0: 6d6f 7665 203d 3d20 272b 270a 2020 2020  move == '+'.    
+0002b0c0: 2020 2020 7375 6273 7472 6163 7465 6420      substracted 
+0002b0d0: 3d20 6164 645f 7265 6d6f 7665 203d 3d20  = add_remove == 
+0002b0e0: 272d 270a 2020 2020 2020 2020 7265 706c  '-'.        repl
+0002b0f0: 6163 696e 675f 7570 7065 7220 3d20 6164  acing_upper = ad
+0002b100: 645f 7265 6d6f 7665 203d 3d20 275e 270a  d_remove == '^'.
+0002b110: 2020 2020 2020 2020 7265 706c 6163 696e          replacin
+0002b120: 675f 6c6f 7765 7220 3d20 6164 645f 7265  g_lower = add_re
+0002b130: 6d6f 7665 203d 3d20 2776 270a 2020 2020  move == 'v'.    
+0002b140: 2020 2020 6368 6f72 645f 696e 7465 7276      chord_interv
+0002b150: 616c 203d 2069 6e74 2863 686f 7264 5f69  al = int(chord_i
+0002b160: 6e74 6572 7661 6c29 202d 2031 0a20 2020  nterval) - 1.   
+0002b170: 2020 2020 2023 2323 2046 726f 6d20 6865       ### From he
+0002b180: 7265 206f 6e2c 2060 6368 6f72 645f 696e  re on, `chord_in
+0002b190: 7465 7276 616c 6020 6973 2064 6563 7265  terval` is decre
+0002b1a0: 6d65 6e74 6564 2c20 692e 652e 2074 6865  mented, i.e. the
+0002b1b0: 2072 6f6f 7420 6973 2030 2c20 7468 6520   root is 0, the 
+0002b1c0: 7365 7665 6e74 6820 6973 2036 2065 7463  seventh is 6 etc
+0002b1d0: 2e20 286a 7573 7420 6c69 6b65 2069 6e20  . (just like in 
+0002b1e0: 6074 7063 7360 290a 2020 2020 2020 2020  `tpcs`).        
+0002b1f0: 6966 2028 6368 6f72 645f 696e 7465 7276  if (chord_interv
+0002b200: 616c 203d 3d20 3020 616e 6420 6e6f 7420  al == 0 and not 
+0002b210: 7375 6273 7472 6163 7465 6429 206f 7220  substracted) or 
+0002b220: 6368 6f72 645f 696e 7465 7276 616c 203e  chord_interval >
+0002b230: 2031 333a 0a20 2020 2020 2020 2020 2020   13:.           
+0002b240: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+0002b250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b260: 2066 227b 4d43 7d43 6861 6e67 6520 7b66   f"{MC}Change {f
+0002b270: 756c 6c7d 2069 7320 6d65 616e 696e 676c  ull} is meaningl
+0002b280: 6573 7320 616e 6420 6967 6e6f 7265 6420  ess and ignored 
+0002b290: 6265 6361 7573 6520 6974 2063 6f6e 6365  because it conce
+0002b2a0: 726e 7320 6368 6f72 6420 746f 6e65 207b  rns chord tone {
+0002b2b0: 6368 6f72 645f 696e 7465 7276 616c 202b  chord_interval +
+0002b2c0: 2031 7d2e 2229 0a20 2020 2020 2020 2020   1}.").         
+0002b2d0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+0002b2e0: 2020 2020 6e65 7874 5f6f 6374 6176 6520      next_octave 
+0002b2f0: 3d20 6368 6f72 645f 696e 7465 7276 616c  = chord_interval
+0002b300: 203e 2037 0a20 2020 2020 2020 2073 6869   > 7.        shi
+0002b310: 6674 203d 2037 202a 2028 6163 632e 636f  ft = 7 * (acc.co
+0002b320: 756e 7428 2723 2729 202d 2061 6363 2e63  unt('#') - acc.c
+0002b330: 6f75 6e74 2827 6227 2929 0a20 2020 2020  ount('b')).     
+0002b340: 2020 206e 6577 5f76 616c 203d 2074 7063     new_val = tpc
+0002b350: 735b 6368 6f72 645f 696e 7465 7276 616c  s[chord_interval
+0002b360: 5d20 2b20 7368 6966 740a 2020 2020 2020  ] + shift.      
+0002b370: 2020 6966 2073 7562 7374 7261 6374 6564    if substracted
+0002b380: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0002b390: 2063 686f 7264 5f69 6e74 6572 7661 6c20   chord_interval 
+0002b3a0: 6e6f 7420 696e 2074 6f6e 655f 6675 6e63  not in tone_func
+0002b3b0: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+0002b3c0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+0002b3d0: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+0002b3e0: 2020 2020 2020 2020 2020 2066 227b 4d43             f"{MC
+0002b3f0: 7d54 6865 2063 6861 6e67 6520 7b66 756c  }The change {ful
+0002b400: 6c7d 2068 6173 206e 6f20 6566 6665 6374  l} has no effect
+0002b410: 2062 6563 6175 7365 2069 7420 636f 6e63   because it conc
+0002b420: 6572 6e73 2061 6e20 696e 7465 7276 616c  erns an interval
+0002b430: 2077 6869 6368 2069 7320 6e6f 7420 696d   which is not im
+0002b440: 706c 6965 6420 6279 207b 6e75 6d65 7261  plied by {numera
+0002b450: 6c7d 7b66 6f72 6d7d 7b66 6967 6261 7373  l}{form}{figbass
+0002b460: 7d2e 2229 0a20 2020 2020 2020 2020 2020  }.").           
+0002b470: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0002b480: 2020 2020 2020 2072 6f6f 745f 706f 7369         root_posi
+0002b490: 7469 6f6e 5b63 686f 7264 5f69 6e74 6572  tion[chord_inter
+0002b4a0: 7661 6c5d 203d 205b 5d0a 2020 2020 2020  val] = [].      
+0002b4b0: 2020 656c 6966 2061 6464 6564 3a0a 2020    elif added:.  
+0002b4c0: 2020 2020 2020 2020 2020 6164 6465 645f            added_
+0002b4d0: 6e6f 7465 732e 6170 7065 6e64 286e 6577  notes.append(new
+0002b4e0: 5f76 616c 290a 2020 2020 2020 2020 656c  _val).        el
+0002b4f0: 6966 206e 6578 745f 6f63 7461 7665 3a0a  if next_octave:.
+0002b500: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0002b510: 6e79 2828 7265 706c 6163 696e 675f 6c6f  ny((replacing_lo
+0002b520: 7765 722c 2072 6570 6c61 6369 6e67 5f75  wer, replacing_u
+0002b530: 7070 6572 2c20 7375 6273 7472 6163 7465  pper, substracte
+0002b540: 6429 293a 0a20 2020 2020 2020 2020 2020  d)):.           
+0002b550: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0002b560: 2866 227b 4d43 7d7b 6675 6c6c 5b30 5d7d  (f"{MC}{full[0]}
+0002b570: 2068 6173 206e 6f20 6566 6665 6374 2069   has no effect i
+0002b580: 6e20 7b66 756c 6c7d 2020 6265 6361 7573  n {full}  becaus
+0002b590: 6520 7468 6520 696e 7465 7276 616c 2069  e the interval i
+0002b5a0: 7320 6c61 7267 6572 2074 6861 6e20 616e  s larger than an
+0002b5b0: 206f 6374 6176 652e 2229 0a20 2020 2020   octave.").     
+0002b5c0: 2020 2020 2020 2061 6464 6564 5f6e 6f74         added_not
+0002b5d0: 6573 2e61 7070 656e 6428 6e65 775f 7661  es.append(new_va
+0002b5e0: 6c29 0a20 2020 2020 2020 2065 6c69 6620  l).        elif 
+0002b5f0: 6368 6f72 645f 696e 7465 7276 616c 2069  chord_interval i
+0002b600: 6e20 5b31 2c20 332c 2035 5d3a 2020 2320  n [1, 3, 5]:  # 
+0002b610: 7468 6573 6520 6172 6520 6368 616e 6765  these are change
+0002b620: 7320 746f 2073 6361 6c65 2064 6567 7265  s to scale degre
+0002b630: 6520 322c 2034 2c20 3620 7468 6174 2072  e 2, 4, 6 that r
+0002b640: 6570 6c61 6365 2074 6865 206c 6f77 6572  eplace the lower
+0002b650: 206e 6569 6768 626f 7572 2075 6e6c 6573   neighbour unles
+0002b660: 7320 7468 6579 2068 6176 6520 6120 2320  s they have a # 
+0002b670: 6f72 205e 0a20 2020 2020 2020 2020 2020  or ^.           
+0002b680: 2069 6620 2723 2720 696e 2061 6363 206f   if '#' in acc o
+0002b690: 7220 7265 706c 6163 696e 675f 7570 7065  r replacing_uppe
+0002b6a0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0002b6b0: 2020 2069 6620 2723 2720 696e 2061 6363     if '#' in acc
+0002b6c0: 2061 6e64 2072 6570 6c61 6369 6e67 5f75   and replacing_u
+0002b6d0: 7070 6572 3a0a 2020 2020 2020 2020 2020  pper:.          
+0002b6e0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0002b6f0: 2e69 6e66 6f28 6622 7b4d 437d 5e20 6973  .info(f"{MC}^ is
+0002b700: 2072 6564 756e 6461 6e74 2069 6e20 7b66   redundant in {f
+0002b710: 756c 6c7d 2e22 290a 2020 2020 2020 2020  ull}.").        
+0002b720: 2020 2020 2020 2020 6966 2063 686f 7264          if chord
+0002b730: 5f69 6e74 6572 7661 6c20 3d3d 2035 2061  _interval == 5 a
+0002b740: 6e64 2069 735f 7472 6961 643a 2020 2320  nd is_triad:  # 
+0002b750: 6c65 6164 696e 6720 746f 6e65 2074 6f20  leading tone to 
+0002b760: 3720 6275 7420 6e6f 7420 696e 2073 6576  7 but not in sev
+0002b770: 656e 7468 2063 686f 7264 0a20 2020 2020  enth chord.     
+0002b780: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0002b790: 6464 6564 5f6e 6f74 6573 2e61 7070 656e  dded_notes.appen
+0002b7a0: 6428 6e65 775f 7661 6c29 0a20 2020 2020  d(new_val).     
+0002b7b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0002b7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b7d0: 2020 2020 2072 6570 6c61 6365 5f63 686f       replace_cho
+0002b7e0: 7264 5f74 6f6e 6528 6368 6f72 645f 696e  rd_tone(chord_in
+0002b7f0: 7465 7276 616c 202b 2031 2c20 6e65 775f  terval + 1, new_
+0002b800: 7661 6c29 0a20 2020 2020 2020 2020 2020  val).           
+0002b810: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0002b820: 2020 2020 2020 2069 6620 7265 706c 6163         if replac
+0002b830: 696e 675f 6c6f 7765 723a 0a20 2020 2020  ing_lower:.     
+0002b840: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0002b850: 6f67 6765 722e 696e 666f 2866 227b 4d43  ogger.info(f"{MC
+0002b860: 7d76 2069 7320 7265 6475 6e64 616e 7420  }v is redundant 
+0002b870: 696e 207b 6675 6c6c 7d2e 2229 0a20 2020  in {full}.").   
+0002b880: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+0002b890: 6c61 6365 5f63 686f 7264 5f74 6f6e 6528  lace_chord_tone(
+0002b8a0: 6368 6f72 645f 696e 7465 7276 616c 202d  chord_interval -
+0002b8b0: 2031 2c20 6e65 775f 7661 6c29 0a20 2020   1, new_val).   
+0002b8c0: 2020 2020 2065 6c73 653a 2020 2320 6368       else:  # ch
+0002b8d0: 6f72 6420 746f 6e65 2061 6c74 6572 6174  ord tone alterat
+0002b8e0: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
+0002b8f0: 2069 6620 7265 706c 6163 696e 675f 6c6f   if replacing_lo
+0002b900: 7765 723a 0a20 2020 2020 2020 2020 2020  wer:.           
+0002b910: 2020 2020 2023 2054 4f44 4f3a 2054 6869       # TODO: Thi
+0002b920: 7320 6d75 7374 2062 6520 706f 7373 6962  s must be possib
+0002b930: 6c65 2c20 652e 672e 2056 2836 7635 2920  le, e.g. V(6v5) 
+0002b940: 7768 6572 6520 3520 6973 2073 7573 7065  where 5 is suspe
+0002b950: 6e73 696f 6e20 6f66 2034 0a20 2020 2020  nsion of 4.     
+0002b960: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0002b970: 722e 696e 666f 2866 227b 4d43 7d7b 6675  r.info(f"{MC}{fu
+0002b980: 6c6c 7d20 2d3e 2063 686f 7264 2074 6f6e  ll} -> chord ton
+0002b990: 6573 2063 616e 6e6f 7420 7265 706c 6163  es cannot replac
+0002b9a0: 6520 6e65 6967 6862 6f75 7273 2c20 7573  e neighbours, us
+0002b9b0: 6520 2b20 696e 7374 6561 642e 2229 0a20  e + instead."). 
+0002b9c0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0002b9d0: 6368 6f72 645f 696e 7465 7276 616c 203d  chord_interval =
+0002b9e0: 3d20 3620 616e 6420 6669 6762 6173 7320  = 6 and figbass 
+0002b9f0: 213d 2027 3727 3a20 2023 2037 7468 2061  != '7':  # 7th a
+0002ba00: 7265 2061 2073 7065 6369 616c 2063 6173  re a special cas
+0002ba10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0002ba20: 2020 2069 6620 6669 6762 6173 7320 3d3d     if figbass ==
+0002ba30: 2027 273a 2020 2320 696e 2072 6f6f 7420   '':  # in root 
+0002ba40: 706f 7369 7469 6f6e 2074 7269 6164 7320  position triads 
+0002ba50: 7468 6579 2061 7265 2061 6464 6564 0a20  they are added. 
+0002ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ba70: 2020 2023 2054 4f44 4f3a 2054 6865 2073     # TODO: The s
+0002ba80: 7461 6e64 6172 6420 6973 206c 6163 6b69  tandard is lacki
+0002ba90: 6e67 2061 2064 6973 7469 6e63 7469 6f6e  ng a distinction
+0002baa0: 2c20 6265 6361 7573 6520 7468 6520 726f  , because the ro
+0002bab0: 6f74 2069 6e20 726f 6f74 2070 6f73 2e20  ot in root pos. 
+0002bac0: 6361 6e20 616c 736f 2062 6520 7265 706c  can also be repl
+0002bad0: 6163 6564 2066 726f 6d20 6265 6c6f 7721  aced from below!
+0002bae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002baf0: 2020 2020 2061 6464 6564 5f6e 6f74 6573       added_notes
+0002bb00: 2e61 7070 656e 6428 6e65 775f 7661 6c29  .append(new_val)
+0002bb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002bb20: 2065 6c69 6620 6669 6762 6173 7320 696e   elif figbass in
+0002bb30: 205b 2736 272c 2027 3634 275d 206f 7220   ['6', '64'] or 
+0002bb40: 2723 2720 696e 2061 6363 3a20 2023 2069  '#' in acc:  # i
+0002bb50: 6e20 696e 7665 7274 6564 2074 7269 6164  n inverted triad
+0002bb60: 7320 7468 6579 2072 6570 6c61 6365 2074  s they replace t
+0002bb70: 6865 2072 6f6f 742c 2061 7320 646f 6573  he root, as does
+0002bb80: 2023 370a 2020 2020 2020 2020 2020 2020   #7.            
+0002bb90: 2020 2020 2020 2020 7265 706c 6163 655f          replace_
+0002bba0: 6368 6f72 645f 746f 6e65 2830 2c20 6e65  chord_tone(0, ne
+0002bbb0: 775f 7661 6c29 0a20 2020 2020 2020 2020  w_val).         
+0002bbc0: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
+0002bbd0: 6f74 6865 7277 6973 6520 7468 6579 2061  otherwise they a
+0002bbe0: 7265 2075 6e63 6c65 6172 0a20 2020 2020  re unclear.     
+0002bbf0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0002bc00: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
+0002bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bc20: 2020 2020 2020 2066 227b 4d43 7d49 6e20         f"{MC}In 
+0002bc30: 7365 7665 6e74 6820 6368 6f72 6473 2c20  seventh chords, 
+0002bc40: 7375 6368 2061 7320 7b6c 6162 656c 7d2c  such as {label},
+0002bc50: 2069 7420 6973 206e 6f74 2063 6c65 6172   it is not clear
+0002bc60: 2077 6865 7468 6572 2074 6865 207b 6675   whether the {fu
+0002bc70: 6c6c 7d20 616c 7465 7273 2074 6865 2037  ll} alters the 7
+0002bc80: 206f 7220 7265 706c 6163 6573 2074 6865   or replaces the
+0002bc90: 2038 2061 6e64 2073 686f 756c 6420 6e6f   8 and should no
+0002bca0: 7420 6265 2075 7365 642e 222c 0a20 2020  t be used.",.   
+0002bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bcc0: 2020 2020 2065 7874 7261 3d7b 226d 6573       extra={"mes
+0002bcd0: 7361 6765 5f69 6422 3a20 2831 382c 2029  sage_id": (18, )
+0002bce0: 7d29 0a20 2020 2020 2020 2020 2020 2065  }).            e
+0002bcf0: 6c69 6620 7470 6373 5b63 686f 7264 5f69  lif tpcs[chord_i
+0002bd00: 6e74 6572 7661 6c5d 203d 3d20 6e65 775f  nterval] == new_
+0002bd10: 7661 6c3a 0a20 2020 2020 2020 2020 2020  val:.           
+0002bd20: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0002bd30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0002bd40: 2020 2020 2020 6622 7b4d 437d 5468 6520        f"{MC}The 
+0002bd50: 6368 616e 6765 207b 6675 6c6c 7d20 6861  change {full} ha
+0002bd60: 7320 6e6f 2065 6666 6563 7420 696e 207b  s no effect in {
+0002bd70: 6e75 6d65 7261 6c7d 7b66 6f72 6d7d 7b66  numeral}{form}{f
+0002bd80: 6967 6261 7373 7d22 290a 2020 2020 2020  igbass}").      
+0002bd90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0002bda0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+0002bdb0: 5f70 6f73 6974 696f 6e5b 6368 6f72 645f  _position[chord_
+0002bdc0: 696e 7465 7276 616c 5d20 3d20 5b6e 6577  interval] = [new
+0002bdd0: 5f76 616c 5d0a 0a20 2020 2066 6967 6261  _val]..    figba
+0002bde0: 7373 3262 6173 7320 3d20 7b0a 2020 2020  ss2bass = {.    
+0002bdf0: 2020 2020 2727 3a20 302c 0a20 2020 2020      '': 0,.     
+0002be00: 2020 2027 3727 3a20 302c 0a20 2020 2020     '7': 0,.     
+0002be10: 2020 2027 3627 3a20 312c 0a20 2020 2020     '6': 1,.     
+0002be20: 2020 2027 3635 273a 2031 2c0a 2020 2020     '65': 1,.    
+0002be30: 2020 2020 2736 3427 3a20 322c 0a20 2020      '64': 2,.   
+0002be40: 2020 2020 2027 3433 273a 2032 2c0a 2020       '43': 2,.  
+0002be50: 2020 2020 2020 2732 273a 2033 0a20 2020        '2': 3.   
+0002be60: 207d 0a20 2020 2062 6173 7320 3d20 6669   }.    bass = fi
+0002be70: 6762 6173 7332 6261 7373 5b66 6967 6261  gbass2bass[figba
+0002be80: 7373 5d0a 2020 2020 6368 6f72 645f 746f  ss].    chord_to
+0002be90: 6e65 7320 3d20 5b5d 0a20 2020 2074 6f6e  nes = [].    ton
+0002bea0: 655f 6675 6e63 7469 6f6e 5f6e 616d 6573  e_function_names
+0002beb0: 203d 207b 0a20 2020 2020 2020 2030 3a20   = {.        0: 
+0002bec0: 2772 6f6f 7427 2c0a 2020 2020 2020 2020  'root',.        
+0002bed0: 323a 2027 3372 6427 2c0a 2020 2020 2020  2: '3rd',.      
+0002bee0: 2020 343a 2027 3574 6827 2c0a 2020 2020    4: '5th',.    
+0002bef0: 2020 2020 363a 2027 3774 6827 2c0a 2020      6: '7th',.  
+0002bf00: 2020 7d0a 2020 2020 666f 7220 7466 2069    }.    for tf i
+0002bf10: 6e20 746f 6e65 5f66 756e 6374 696f 6e73  n tone_functions
+0002bf20: 5b62 6173 733a 5d20 2b20 746f 6e65 5f66  [bass:] + tone_f
+0002bf30: 756e 6374 696f 6e73 5b3a 6261 7373 5d3a  unctions[:bass]:
+0002bf40: 0a20 2020 2020 2020 2063 686f 7264 5f74  .        chord_t
+0002bf50: 6f6e 652c 2072 6570 6c61 6369 6e67 5f74  one, replacing_t
+0002bf60: 6f6e 6573 203d 2072 6f6f 745f 706f 7369  ones = root_posi
+0002bf70: 7469 6f6e 5b74 665d 2c20 7265 706c 6163  tion[tf], replac
+0002bf80: 656d 656e 7473 5b74 665d 0a20 2020 2020  ements[tf].     
+0002bf90: 2020 2069 6620 6368 6f72 645f 746f 6e65     if chord_tone
+0002bfa0: 203d 3d20 7265 706c 6163 696e 675f 746f   == replacing_to
+0002bfb0: 6e65 7320 3d3d 205b 5d3a 0a20 2020 2020  nes == []:.     
+0002bfc0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0002bfd0: 6275 6728 6622 7b4d 437d 7b6c 6162 656c  bug(f"{MC}{label
+0002bfe0: 7d20 7265 7375 6c74 7320 696e 2061 2063  } results in a c
+0002bff0: 686f 7264 2077 6974 686f 7574 207b 746f  hord without {to
+0002c000: 6e65 5f66 756e 6374 696f 6e5f 6e61 6d65  ne_function_name
+0002c010: 735b 7466 5d7d 2e22 290a 2020 2020 2020  s[tf]}.").      
+0002c020: 2020 6966 2063 686f 7264 5f74 6f6e 6520    if chord_tone 
+0002c030: 213d 205b 5d3a 0a20 2020 2020 2020 2020  != []:.         
+0002c040: 2020 2063 686f 7264 5f74 6f6e 6573 2e61     chord_tones.a
+0002c050: 7070 656e 6428 6368 6f72 645f 746f 6e65  ppend(chord_tone
+0002c060: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0002c070: 2069 6620 7265 706c 6163 696e 675f 746f   if replacing_to
+0002c080: 6e65 7320 213d 205b 5d3a 0a20 2020 2020  nes != []:.     
+0002c090: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0002c0a0: 722e 7761 726e 696e 6728 6622 7b4d 437d  r.warning(f"{MC}
+0002c0b0: 7b6c 6162 656c 7d20 7265 7375 6c74 7320  {label} results 
+0002c0c0: 696e 2061 2063 686f 7264 2074 6f6e 6520  in a chord tone 
+0002c0d0: 7b74 6f6e 655f 6675 6e63 7469 6f6e 5f6e  {tone_function_n
+0002c0e0: 616d 6573 5b74 665d 7d20 414e 4420 6974  ames[tf]} AND it
+0002c0f0: 7320 7265 706c 6163 656d 656e 7428 7329  s replacement(s)
+0002c100: 2028 5450 4320 7b72 6570 6c61 6369 6e67   (TPC {replacing
+0002c110: 5f74 6f6e 6573 7d29 2e20 220a 2020 2020  _tones}). ".    
+0002c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c130: 2020 2020 2020 2020 2020 2066 2259 6f75             f"You
+0002c140: 206d 6967 6874 2077 616e 7420 746f 2061   might want to a
+0002c150: 6464 2061 202b 2074 6f20 6469 7374 696e  dd a + to distin
+0002c160: 6775 6973 6820 6672 6f6d 2061 2073 7573  guish from a sus
+0002c170: 7065 6e73 696f 6e2c 206f 7220 6164 6420  pension, or add 
+0002c180: 7468 6973 2077 6172 6e69 6e67 2074 6f20  this warning to 
+0002c190: 4947 4e4f 5245 445f 5741 524e 494e 4753  IGNORED_WARNINGS
+0002c1a0: 2077 6974 6820 6120 636f 6d6d 656e 742e   with a comment.
+0002c1b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0002c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c1d0: 2020 6578 7472 613d 7b22 6d65 7373 6167    extra={"messag
+0002c1e0: 655f 6964 223a 2028 362c 206d 632c 206c  e_id": (6, mc, l
+0002c1f0: 6162 656c 297d 290a 2020 2020 2020 2020  abel)}).        
+0002c200: 6368 6f72 645f 746f 6e65 732e 6578 7465  chord_tones.exte
+0002c210: 6e64 2872 6570 6c61 6369 6e67 5f74 6f6e  nd(replacing_ton
+0002c220: 6573 290a 0a20 2020 2062 6173 735f 7470  es)..    bass_tp
+0002c230: 6320 3d20 6368 6f72 645f 746f 6e65 735b  c = chord_tones[
+0002c240: 305d 0a20 2020 2069 6620 6261 7373 5f6f  0].    if bass_o
+0002c250: 6e6c 793a 0a20 2020 2020 2020 2072 6574  nly:.        ret
+0002c260: 7572 6e20 6261 7373 5f74 7063 0a20 2020  urn bass_tpc.   
+0002c270: 2065 6c69 6620 6d65 7267 655f 746f 6e65   elif merge_tone
+0002c280: 733a 0a20 2020 2020 2020 2072 6574 7572  s:.        retur
+0002c290: 6e20 7475 706c 6528 736f 7274 5f74 7063  n tuple(sort_tpc
+0002c2a0: 7328 6368 6f72 645f 746f 6e65 7320 2b20  s(chord_tones + 
+0002c2b0: 6164 6465 645f 6e6f 7465 732c 2073 7461  added_notes, sta
+0002c2c0: 7274 3d62 6173 735f 7470 6329 290a 2020  rt=bass_tpc)).  
+0002c2d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002c2e0: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
+0002c2f0: 2020 2020 2027 6368 6f72 645f 746f 6e65       'chord_tone
+0002c300: 7327 3a20 7475 706c 6528 6368 6f72 645f  s': tuple(chord_
+0002c310: 746f 6e65 7329 2c0a 2020 2020 2020 2020  tones),.        
+0002c320: 2020 2020 2761 6464 6564 5f74 6f6e 6573      'added_tones
+0002c330: 273a 2074 7570 6c65 2861 6464 6564 5f6e  ': tuple(added_n
+0002c340: 6f74 6573 292c 0a20 2020 2020 2020 2020  otes),.         
+0002c350: 2020 2027 726f 6f74 273a 2072 6f6f 742c     'root': root,
+0002c360: 0a20 2020 2020 2020 207d 0a0a 6465 6620  .        }..def 
+0002c370: 7061 7468 3270 6172 656e 745f 636f 7270  path2parent_corp
+0002c380: 7573 2870 6174 6829 3a0a 2020 2020 2222  us(path):.    ""
+0002c390: 2257 616c 6b20 7570 2074 6865 2070 6174  "Walk up the pat
+0002c3a0: 6820 616e 6420 7265 7475 726e 2074 6865  h and return the
+0002c3b0: 206e 616d 6520 6f66 2074 6865 2066 6972   name of the fir
+0002c3c0: 7374 2073 7570 6572 6469 7265 6374 6f72  st superdirector
+0002c3d0: 7920 7468 6174 2069 7320 6120 6769 7420  y that is a git 
+0002c3e0: 7265 706f 7369 746f 7279 206f 7220 636f  repository or co
+0002c3f0: 6e74 6169 6e73 2061 2027 6d65 7461 6461  ntains a 'metada
+0002c400: 7461 2e74 7376 2720 6669 6c65 2e22 2222  ta.tsv' file."""
+0002c410: 0a20 2020 2069 6620 7061 7468 2069 6e20  .    if path in 
+0002c420: 2827 272c 2027 2f27 293a 0a20 2020 2020  ('', '/'):.     
+0002c430: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+0002c440: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0002c450: 6966 206f 732e 7061 7468 2e69 7364 6972  if os.path.isdir
+0002c460: 2870 6174 6829 3a0a 2020 2020 2020 2020  (path):.        
+0002c470: 2020 2020 6c69 7374 6469 7220 3d20 6f73      listdir = os
+0002c480: 2e6c 6973 7464 6972 2870 6174 6829 0a20  .listdir(path). 
+0002c490: 2020 2020 2020 2020 2020 2069 6620 276d             if 'm
+0002c4a0: 6574 6164 6174 612e 7473 7627 2069 6e20  etadata.tsv' in 
+0002c4b0: 6c69 7374 6469 7220 6f72 2027 2e67 6974  listdir or '.git
+0002c4c0: 2720 696e 206c 6973 7464 6972 3a0a 2020  ' in listdir:.  
+0002c4d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0002c4e0: 7475 726e 2070 6174 680a 2020 2020 2020  turn path.      
+0002c4f0: 2020 7265 7475 726e 2070 6174 6832 7061    return path2pa
+0002c500: 7265 6e74 5f63 6f72 7075 7328 6f73 2e70  rent_corpus(os.p
+0002c510: 6174 682e 6469 726e 616d 6528 7061 7468  ath.dirname(path
+0002c520: 2929 0a20 2020 2065 7863 6570 7420 4578  )).    except Ex
+0002c530: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+0002c540: 2072 6574 7572 6e20 4e6f 6e65 0a0a 0a40   return None...@
+0002c550: 6675 6e63 7469 6f6e 5f6c 6f67 6765 720a  function_logger.
+0002c560: 6465 6620 6368 6f72 6432 7470 6373 2863  def chord2tpcs(c
+0002c570: 686f 7264 2c20 7265 6765 783d 4e6f 6e65  hord, regex=None
+0002c580: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+0002c590: 2022 2222 0a20 2020 2053 706c 6974 2061   """.    Split a
+0002c5a0: 2063 686f 7264 206c 6162 656c 2069 6e74   chord label int
+0002c5b0: 6f20 6974 7320 6665 6174 7572 6573 2061  o its features a
+0002c5c0: 6e64 2061 7070 6c79 2066 6561 7475 7265  nd apply feature
+0002c5d0: 7332 7470 6373 2829 2e0a 0a20 2020 2055  s2tpcs()...    U
+0002c5e0: 7365 733a 2066 6561 7475 7265 7332 7470  ses: features2tp
+0002c5f0: 6373 2829 0a0a 2020 2020 5061 7261 6d65  cs()..    Parame
+0002c600: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0002c610: 2d2d 2d0a 2020 2020 6368 6f72 6420 3a20  ---.    chord : 
+0002c620: 3a6f 626a 3a60 7374 7260 0a20 2020 2020  :obj:`str`.     
+0002c630: 2020 2043 686f 7264 206c 6162 656c 2074     Chord label t
+0002c640: 6861 7420 6361 6e20 6265 2073 706c 6974  hat can be split
+0002c650: 2069 6e74 6f20 7468 6520 6665 6174 7572   into the featur
+0002c660: 6573 205b 276e 756d 6572 616c 272c 2027  es ['numeral', '
+0002c670: 666f 726d 272c 2027 6669 6762 6173 7327  form', 'figbass'
+0002c680: 2c20 2763 6861 6e67 6573 272c 2027 7265  , 'changes', 're
+0002c690: 6c61 7469 7665 726f 6f74 275d 2e0a 2020  lativeroot']..  
+0002c6a0: 2020 7265 6765 7820 3a20 3a6f 626a 3a60    regex : :obj:`
+0002c6b0: 7265 2e50 6174 7465 726e 602c 206f 7074  re.Pattern`, opt
+0002c6c0: 696f 6e61 6c0a 2020 2020 2020 2020 436f  ional.        Co
+0002c6d0: 6d70 696c 6564 2072 6567 6578 2077 6974  mpiled regex wit
+0002c6e0: 6820 6e61 6d65 6420 6772 6f75 7073 2066  h named groups f
+0002c6f0: 6f72 2074 6865 2066 6976 6520 6665 6174  or the five feat
+0002c700: 7572 6573 2e20 4279 2064 6566 6175 6c74  ures. By default
+0002c710: 2c20 7468 6520 6375 7272 656e 7420 7665  , the current ve
+0002c720: 7273 696f 6e20 6f66 2074 6865 2044 434d  rsion of the DCM
+0002c730: 4c20 6861 726d 6f6e 790a 2020 2020 2020  L harmony.      
+0002c740: 2020 616e 6e6f 7461 7469 6f6e 2073 7461    annotation sta
+0002c750: 6e64 6172 6420 6973 2075 7365 642e 0a20  ndard is used.. 
+0002c760: 2020 202a 2a6b 7761 7267 7320 3a0a 2020     **kwargs :.  
+0002c770: 2020 2020 2020 6172 6775 6d65 6e74 7320        arguments 
+0002c780: 666f 7220 6665 6174 7572 6573 3274 7063  for features2tpc
+0002c790: 7320 2870 6173 7320 4d43 2074 6f20 7368  s (pass MC to sh
+0002c7a0: 6f77 2069 7420 696e 2077 6172 6e69 6e67  ow it in warning
+0002c7b0: 7321 290a 2020 2020 2222 220a 2020 2020  s!).    """.    
+0002c7c0: 6966 2072 6567 6578 2069 7320 4e6f 6e65  if regex is None
+0002c7d0: 3a0a 2020 2020 2020 2020 7265 6765 7820  :.        regex 
+0002c7e0: 3d20 4443 4d4c 5f52 4547 4558 0a20 2020  = DCML_REGEX.   
+0002c7f0: 2063 686f 7264 5f66 6561 7475 7265 7320   chord_features 
+0002c800: 3d20 7265 2e6d 6174 6368 2872 6567 6578  = re.match(regex
+0002c810: 2c20 6368 6f72 6429 0a20 2020 2061 7373  , chord).    ass
+0002c820: 6572 7420 6368 6f72 645f 6665 6174 7572  ert chord_featur
+0002c830: 6573 2069 7320 6e6f 7420 4e6f 6e65 2c20  es is not None, 
+0002c840: 6622 7b63 686f 7264 7d20 646f 6573 206e  f"{chord} does n
+0002c850: 6f74 206d 6174 6368 2074 6865 2072 6567  ot match the reg
+0002c860: 6578 2e22 0a20 2020 2063 686f 7264 5f66  ex.".    chord_f
+0002c870: 6561 7475 7265 7320 3d20 6368 6f72 645f  eatures = chord_
+0002c880: 6665 6174 7572 6573 2e67 726f 7570 6469  features.groupdi
+0002c890: 6374 2829 0a20 2020 206e 756d 6572 616c  ct().    numeral
+0002c8a0: 2c20 666f 726d 2c20 6669 6762 6173 732c  , form, figbass,
+0002c8b0: 2063 6861 6e67 6573 2c20 7265 6c61 7469   changes, relati
+0002c8c0: 7665 726f 6f74 203d 2074 7570 6c65 2863  veroot = tuple(c
+0002c8d0: 686f 7264 5f66 6561 7475 7265 735b 665d  hord_features[f]
+0002c8e0: 2066 6f72 2066 2069 6e20 2827 6e75 6d65   for f in ('nume
+0002c8f0: 7261 6c27 2c20 2766 6f72 6d27 2c20 2766  ral', 'form', 'f
+0002c900: 6967 6261 7373 272c 2027 6368 616e 6765  igbass', 'change
+0002c910: 7327 2c20 2772 656c 6174 6976 6572 6f6f  s', 'relativeroo
+0002c920: 7427 2929 0a20 2020 2072 6574 7572 6e20  t')).    return 
+0002c930: 6665 6174 7572 6573 3274 7063 7328 6e75  features2tpcs(nu
+0002c940: 6d65 7261 6c3d 6e75 6d65 7261 6c2c 2066  meral=numeral, f
+0002c950: 6f72 6d3d 666f 726d 2c20 6669 6762 6173  orm=form, figbas
+0002c960: 733d 6669 6762 6173 732c 2063 6861 6e67  s=figbass, chang
+0002c970: 6573 3d63 6861 6e67 6573 2c20 7265 6c61  es=changes, rela
+0002c980: 7469 7665 726f 6f74 3d72 656c 6174 6976  tiveroot=relativ
+0002c990: 6572 6f6f 742c 0a20 2020 2020 2020 2020  eroot,.         
+0002c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c9b0: 6c6f 6767 6572 3d6c 6f67 6765 722c 202a  logger=logger, *
+0002c9c0: 2a6b 7761 7267 7329 0a0a 0a64 6566 2074  *kwargs)...def t
+0002c9d0: 7261 6e73 706f 7365 2865 2c20 6e29 3a0a  ranspose(e, n):.
+0002c9e0: 2020 2020 2222 2220 4164 6420 606e 6020      """ Add `n` 
+0002c9f0: 746f 2061 6c6c 2065 6c65 6d65 6e74 7320  to all elements 
+0002ca00: 6065 6020 7265 6375 7273 6976 656c 792e  `e` recursively.
+0002ca10: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+0002ca20: 7572 6e20 6d61 7032 656c 656d 656e 7473  urn map2elements
+0002ca30: 2865 2c20 6c61 6d62 6461 2078 3a20 7820  (e, lambda x: x 
+0002ca40: 2b20 6e29 0a0a 0a64 6566 2070 6172 7365  + n)...def parse
+0002ca50: 5f69 676e 6f72 6564 5f77 6172 6e69 6e67  _ignored_warning
+0002ca60: 7328 6d65 7373 6167 6573 3a20 436f 6c6c  s(messages: Coll
+0002ca70: 6563 7469 6f6e 5b73 7472 5d29 202d 3e20  ection[str]) -> 
+0002ca80: 4974 6572 6174 6f72 5b54 7570 6c65 5b73  Iterator[Tuple[s
+0002ca90: 7472 2c20 5475 706c 655b 696e 745d 5d5d  tr, Tuple[int]]]
+0002caa0: 3a0a 2020 2020 2222 2254 7572 6e73 2061  :.    """Turns a
+0002cab0: 206c 6973 7420 6f66 206c 6f67 206d 6573   list of log mes
+0002cac0: 7361 6765 7320 696e 746f 2061 6e20 6974  sages into an it
+0002cad0: 6572 6174 6f72 206f 6620 286c 6f67 6765  erator of (logge
+0002cae0: 725f 6e61 6d65 2c20 286d 6573 7361 6765  r_name, (message
+0002caf0: 5f69 6e66 6f2c 202e 2e2e 2929 2070 6169  _info, ...)) pai
+0002cb00: 7273 2e0a 2020 2020 4c6f 6720 6d65 7373  rs..    Log mess
+0002cb10: 6167 6573 2063 6f6e 7369 7374 206f 6620  ages consist of 
+0002cb20: 6120 6865 6164 6572 206f 6620 7468 6520  a header of the 
+0002cb30: 7368 6170 6520 5741 524e 494e 475f 454e  shape WARNING_EN
+0002cb40: 554d 5f4d 454d 4245 5220 2865 6e75 6d5f  UM_MEMBER (enum_
+0002cb50: 7661 6c75 652c 205b 6d63 2c20 6d6f 7265  value, [mc, more
+0002cb60: 5f69 6e66 6f2e 2e2e 5d29 206d 7333 2e28  _info...]) ms3.(
+0002cb70: 5061 7273 657c 436f 7270 7573 292e 636f  Parse|Corpus).co
+0002cb80: 7270 7573 2e66 6e61 6d65 205b 2d2d 2070  rpus.fname [-- p
+0002cb90: 6f74 656e 7469 616c 6c79 206d 6f72 652c  otentially more,
+0002cba0: 2069 7272 656c 6576 616e 7420 7374 7566   irrelevant stuf
+0002cbb0: 665d 2e0a 2020 2020 5468 6520 6865 6164  f]..    The head
+0002cbc0: 6572 206d 6967 6874 2062 6520 666f 6c6c  er might be foll
+0002cbd0: 6f77 6564 2062 7920 7365 7665 7261 6c20  owed by several 
+0002cbe0: 6c69 6e65 7320 6f66 2063 6f6d 6d65 6e74  lines of comment
+0002cbf0: 732c 2065 6163 6820 6265 6769 6e6e 696e  s, each beginnin
+0002cc00: 6720 7769 7468 2061 2073 7061 6365 206f  g with a space o
+0002cc10: 7220 7461 622e 0a20 2020 2022 2222 0a20  r tab..    """. 
+0002cc20: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0002cc30: 286d 6573 7361 6765 732c 2073 7472 293a  (messages, str):
+0002cc40: 0a20 2020 2020 2020 2079 6965 6c64 2066  .        yield f
+0002cc50: 726f 6d20 7061 7273 655f 6967 6e6f 7265  rom parse_ignore
+0002cc60: 645f 7761 726e 696e 6773 285b 6d65 7373  d_warnings([mess
+0002cc70: 6167 6573 5d29 0a20 2020 2065 6c73 653a  ages]).    else:
+0002cc80: 0a20 2020 2020 2020 2066 6f72 206d 6573  .        for mes
+0002cc90: 7361 6765 2069 6e20 6d65 7373 6167 6573  sage in messages
+0002cca0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0002ccb0: 2027 5c6e 2720 696e 206d 6573 7361 6765   '\n' in message
+0002ccc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002ccd0: 2020 7969 656c 6420 6672 6f6d 2070 6172    yield from par
+0002cce0: 7365 5f69 676e 6f72 6564 5f77 6172 6e69  se_ignored_warni
+0002ccf0: 6e67 7328 6d65 7373 6167 652e 7370 6c69  ngs(message.spli
+0002cd00: 7428 275c 6e27 2929 0a20 2020 2020 2020  t('\n')).       
+0002cd10: 2020 2020 2065 6c69 6620 6d65 7373 6167       elif messag
+0002cd20: 6520 3d3d 2027 273a 0a20 2020 2020 2020  e == '':.       
+0002cd30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0002cd40: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+0002cd50: 6966 206d 6573 7361 6765 5b30 5d20 696e  if message[0] in
+0002cd60: 2028 2720 272c 2027 5c74 272c 2027 2327   (' ', '\t', '#'
+0002cd70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002cd80: 2020 2023 2069 6620 7365 7665 7261 6c20     # if several 
+0002cd90: 6c69 6e65 7320 6f66 2061 2077 6172 6e69  lines of a warni
+0002cda0: 6e67 2077 6572 6520 636f 7069 6564 2c20  ng were copied, 
+0002cdb0: 7573 6520 6f6e 6c79 2074 6865 2066 6972  use only the fir
+0002cdc0: 7374 206f 6e65 0a20 2020 2020 2020 2020  st one.         
+0002cdd0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0002cde0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0002cdf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002ce00: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0002ce10: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+0002ce20: 7468 6520 616e 6e6f 7461 746f 7220 636f  the annotator co
+0002ce30: 7069 6564 2074 6f6f 206d 7563 682c 2063  pied too much, c
+0002ce40: 7574 206f 6666 2074 6865 2072 6564 756e  ut off the redun
+0002ce50: 6461 6e74 2069 6e66 6f72 6d61 7469 6f6e  dant information
+0002ce60: 2061 7420 7468 6520 656e 640a 2020 2020   at the end.    
+0002ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ce80: 7265 6475 6e64 616e 7420 3d20 206d 6573  redundant =  mes
+0002ce90: 7361 6765 2e69 6e64 6578 2827 202d 2d20  sage.index(' -- 
+0002cea0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+0002ceb0: 2020 2020 2020 206d 6573 7361 6765 203d         message =
+0002cec0: 206d 6573 7361 6765 5b3a 7265 6475 6e64   message[:redund
+0002ced0: 616e 745d 0a20 2020 2020 2020 2020 2020  ant].           
+0002cee0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+0002cef0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+0002cf00: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0002cf10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002cf20: 206d 6573 7361 6765 203d 206d 6573 7361   message = messa
+0002cf30: 6765 2e73 7472 6970 2829 0a20 2020 2020  ge.strip().     
+0002cf40: 2020 2020 2020 2020 2020 2073 706c 6974             split
+0002cf50: 5f72 6520 3d20 7222 5e28 2e2a 2920 285c  _re = r"^(.*) (\
+0002cf60: 532b 2924 220a 2020 2020 2020 2020 2020  S+)$".          
+0002cf70: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0002cf80: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002cf90: 7367 2c20 6c6f 6767 6572 5f6e 616d 6520  sg, logger_name 
+0002cfa0: 3d20 7265 2e6d 6174 6368 2873 706c 6974  = re.match(split
+0002cfb0: 5f72 652c 206d 6573 7361 6765 292e 6772  _re, message).gr
+0002cfc0: 6f75 7073 2829 0a20 2020 2020 2020 2020  oups().         
+0002cfd0: 2020 2020 2020 2065 7863 6570 7420 4174         except At
+0002cfe0: 7472 6962 7574 6545 7272 6f72 3a0a 2020  tributeError:.  
+0002cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d000: 2020 7072 696e 7428 6622 5468 6520 666f    print(f"The fo
+0002d010: 6c6c 6f77 696e 6720 6d65 7373 6167 6520  llowing message 
+0002d020: 636f 756c 6420 6e6f 7420 6265 2073 706c  could not be spl
+0002d030: 6974 2c20 6170 7061 7265 6e74 6c79 2069  it, apparently i
+0002d040: 7420 646f 6573 206e 6f74 2065 6e64 2077  t does not end w
+0002d050: 6974 6820 7468 6520 6c6f 6767 6572 5f6e  ith the logger_n
+0002d060: 616d 653a 207b 6d65 7373 6167 657d 2229  ame: {message}")
+0002d070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002d080: 2020 2020 2072 6169 7365 0a20 2020 2020       raise.     
+0002d090: 2020 2020 2020 2020 2020 2069 6620 6d73             if ms
+0002d0a0: 675b 2d31 5d20 213d 2027 2927 3a0a 2020  g[-1] != ')':.  
+0002d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d0c0: 2020 6966 2061 6e79 286d 7367 2e73 7461    if any(msg.sta
+0002d0d0: 7274 7377 6974 6828 6c65 7665 6c29 2066  rtswith(level) f
+0002d0e0: 6f72 206c 6576 656c 2069 6e20 2827 4445  or level in ('DE
+0002d0f0: 4255 4727 2c20 2749 4e46 4f27 2c20 2757  BUG', 'INFO', 'W
+0002d100: 4152 4e49 4e47 272c 2027 4552 524f 5227  ARNING', 'ERROR'
+0002d110: 2c20 2743 5249 5449 4341 4c27 2929 3a0a  , 'CRITICAL')):.
+0002d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d130: 2020 2020 2020 2020 2320 6d65 7373 6167          # messag
+0002d140: 655f 6964 2068 6173 206e 6f74 2028 7965  e_id has not (ye
+0002d150: 7429 2073 7065 6369 6669 6564 2066 6f72  t) specified for
+0002d160: 2074 6869 7320 6c6f 6720 6d65 7373 6167   this log messag
+0002d170: 6520 616e 6420 6973 2069 676e 6f72 6564  e and is ignored
+0002d180: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+0002d190: 2020 2020 2020 2020 2020 2320 6120 7761            # a wa
+0002d1a0: 726e 696e 6720 636f 756c 6420 6265 2069  rning could be i
+0002d1b0: 6d70 6c65 6d65 6e74 6564 2061 7420 7468  mplemented at th
+0002d1c0: 6973 2070 6f69 6e74 0a20 2020 2020 2020  is point.       
+0002d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d1e0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+0002d1f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0002d200: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002d210: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0002d220: 6520 5661 6c75 6545 7272 6f72 2866 2255  e ValueError(f"U
+0002d230: 6e65 7870 6563 7465 6420 6c6f 6720 6d65  nexpected log me
+0002d240: 7373 6167 6520 666f 726d 6174 3a20 7b6d  ssage format: {m
+0002d250: 7367 7d22 290a 2020 2020 2020 2020 2020  sg}").          
+0002d260: 2020 2020 2020 7475 706c 655f 7374 6172        tuple_star
+0002d270: 7420 3d20 6d73 672e 696e 6465 7828 2728  t = msg.index('(
+0002d280: 2729 202b 2031 0a20 2020 2020 2020 2020  ') + 1.         
+0002d290: 2020 2020 2020 2074 7570 6c65 5f73 7472         tuple_str
+0002d2a0: 203d 206d 7367 5b74 7570 6c65 5f73 7461   = msg[tuple_sta
+0002d2b0: 7274 3a2d 315d 0a20 2020 2020 2020 2020  rt:-1].         
+0002d2c0: 2020 2020 2020 2069 6e66 6f20 3d20 7374         info = st
+0002d2d0: 7232 696e 7474 7570 6c65 2874 7570 6c65  r2inttuple(tuple
+0002d2e0: 5f73 7472 2c20 7374 7269 6374 3d46 616c  _str, strict=Fal
+0002d2f0: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+0002d300: 2020 2020 7969 656c 6420 6c6f 6767 6572      yield logger
+0002d310: 5f6e 616d 652c 2069 6e66 6f0a 0a64 6566  _name, info..def
+0002d320: 2069 676e 6f72 6564 5f77 6172 6e69 6e67   ignored_warning
+0002d330: 7332 6469 6374 286d 6573 7361 6765 733a  s2dict(messages:
+0002d340: 2043 6f6c 6c65 6374 696f 6e5b 7374 725d   Collection[str]
+0002d350: 2920 2d3e 2044 6963 745b 7374 722c 204c  ) -> Dict[str, L
+0002d360: 6973 745b 5475 706c 655b 696e 745d 5d5d  ist[Tuple[int]]]
+0002d370: 3a0a 2020 2020 2222 220a 0a20 2020 2041  :.    """..    A
+0002d380: 7267 733a 0a20 2020 2020 206d 6573 7361  rgs:.      messa
+0002d390: 6765 733a 0a0a 2020 2020 5265 7475 726e  ges:..    Return
+0002d3a0: 733a 0a20 2020 2020 207b 6c6f 6767 6572  s:.      {logger
+0002d3b0: 5f6e 616d 6520 2d3e 205b 6967 6e6f 7265  _name -> [ignore
+0002d3c0: 645f 7761 726e 696e 6773 5d7d 2064 6963  d_warnings]} dic
+0002d3d0: 742e 0a20 2020 2022 2222 0a20 2020 2069  t..    """.    i
+0002d3e0: 676e 6f72 6564 5f77 6172 6e69 6e67 7320  gnored_warnings 
+0002d3f0: 3d20 6465 6661 756c 7464 6963 7428 6c69  = defaultdict(li
+0002d400: 7374 290a 2020 2020 666f 7220 6c6f 6767  st).    for logg
+0002d410: 6572 5f6e 616d 652c 2069 6e66 6f20 696e  er_name, info in
+0002d420: 2070 6172 7365 5f69 676e 6f72 6564 5f77   parse_ignored_w
+0002d430: 6172 6e69 6e67 7328 6d65 7373 6167 6573  arnings(messages
+0002d440: 293a 0a20 2020 2020 2020 2069 676e 6f72  ):.        ignor
+0002d450: 6564 5f77 6172 6e69 6e67 735b 6c6f 6767  ed_warnings[logg
+0002d460: 6572 5f6e 616d 655d 2e61 7070 656e 6428  er_name].append(
+0002d470: 696e 666f 290a 2020 2020 7265 7475 726e  info).    return
+0002d480: 2064 6963 7428 6967 6e6f 7265 645f 7761   dict(ignored_wa
+0002d490: 726e 696e 6773 290a 0a64 6566 2070 6172  rnings)..def par
+0002d4a0: 7365 5f69 676e 6f72 6564 5f77 6172 6e69  se_ignored_warni
+0002d4b0: 6e67 735f 6669 6c65 2870 6174 683a 2073  ngs_file(path: s
+0002d4c0: 7472 2920 2d3e 2044 6963 745b 7374 722c  tr) -> Dict[str,
+0002d4d0: 204c 6973 745b 5475 706c 655b 696e 742c   List[Tuple[int,
+0002d4e0: 2054 7570 6c65 5b69 6e74 5d5d 5d5d 3a0a   Tuple[int]]]]:.
+0002d4f0: 2020 2020 2222 2250 6172 7365 2066 696c      """Parse fil
+0002d500: 6520 7769 7468 206c 6f67 206d 6573 7361  e with log messa
+0002d510: 6765 7320 7468 6174 2068 6176 6520 746f  ges that have to
+0002d520: 2062 6520 6967 6e6f 7265 6420 746f 2074   be ignored to t
+0002d530: 6865 2064 6963 742e 0a20 2020 2054 6865  he dict..    The
+0002d540: 2065 7870 6563 7465 6420 7374 7275 6374   expected struct
+0002d550: 7572 6520 6f66 206d 6573 7361 6765 3a20  ure of message: 
+0002d560: 7761 726e 696e 675f 7479 7065 2028 7761  warning_type (wa
+0002d570: 726e 696e 675f 7479 7065 5f69 642c 202a  rning_type_id, *
+0002d580: 696e 7465 6765 7273 2920 6669 6c65 0a20  integers) file. 
+0002d590: 2020 2045 7861 6d70 6c65 206f 6620 6d65     Example of me
+0002d5a0: 7373 6167 653a 2049 4e43 4f52 5245 4354  ssage: INCORRECT
+0002d5b0: 5f56 4f4c 5441 5f4d 4e5f 5741 524e 494e  _VOLTA_MN_WARNIN
+0002d5c0: 4720 2832 2c20 3934 2920 6d73 332e 5061  G (2, 94) ms3.Pa
+0002d5d0: 7273 652e 6d69 7865 645f 6669 6c65 732e  rse.mixed_files.
+0002d5e0: 4469 6430 334d 2d53 6f6e 5f72 6567 696e  Did03M-Son_regin
+0002d5f0: 612d 3137 3632 2d53 6172 7469 2e6d 7363  a-1762-Sarti.msc
+0002d600: 782e 4d65 6173 7572 654c 6973 740a 0a20  x.MeasureList.. 
+0002d610: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0002d620: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0002d630: 206b 6579 203a 203a 6f62 6a3a 6073 7472   key : :obj:`str
+0002d640: 600a 2020 2020 2020 2020 7c20 5061 7468  `.        | Path
+0002d650: 2074 6f20 4947 4e4f 5245 445f 5741 524e   to IGNORED_WARN
+0002d660: 494e 4753 0a0a 2020 2020 5265 7475 726e  INGS..    Return
+0002d670: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+0002d680: 2020 3a6f 626a 3a20 6469 6374 0a20 2020    :obj: dict.   
+0002d690: 2020 2020 207b 6c6f 6767 6572 5f6e 616d       {logger_nam
+0002d6a0: 653a 205b 286d 6573 7361 6765 5f69 642c  e: [(message_id,
+0002d6b0: 206c 6162 656c 5f6f 665f 6d65 7373 6167   label_of_messag
+0002d6c0: 6529 2c20 286d 6573 7361 6765 5f69 642c  e), (message_id,
+0002d6d0: 206c 6162 656c 5f6f 665f 6d65 7373 6167   label_of_messag
+0002d6e0: 6529 2c20 2e2e 2e5d 7d2e 0a20 2020 2022  e), ...]}..    "
+0002d6f0: 2222 0a20 2020 2070 6174 6820 3d20 7265  "".    path = re
+0002d700: 736f 6c76 655f 6469 7228 7061 7468 290a  solve_dir(path).
+0002d710: 2020 2020 6d65 7373 6167 6573 203d 206f      messages = o
+0002d720: 7065 6e28 7061 7468 2c20 2772 272c 2065  pen(path, 'r', e
+0002d730: 6e63 6f64 696e 673d 2775 7466 2d38 2729  ncoding='utf-8')
+0002d740: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
+0002d750: 2072 6574 7572 6e20 6967 6e6f 7265 645f   return ignored_
+0002d760: 7761 726e 696e 6773 3264 6963 7428 6d65  warnings2dict(me
+0002d770: 7373 6167 6573 290a 0a0a 6465 6620 6f76  ssages)...def ov
+0002d780: 6572 6c61 7070 696e 675f 6368 756e 6b5f  erlapping_chunk_
+0002d790: 7065 725f 696e 7465 7276 616c 2864 663a  per_interval(df:
+0002d7a0: 2070 642e 4461 7461 4672 616d 652c 0a20   pd.DataFrame,. 
 0002d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d7c0: 2020 2020 2020 2020 2020 7472 756e 6361            trunca
-0002d7d0: 7465 3a20 626f 6f6c 203d 2054 7275 6529  te: bool = True)
-0002d7e0: 202d 3e20 4469 6374 5b70 642e 496e 7465   -> Dict[pd.Inte
-0002d7f0: 7276 616c 2c20 7064 2e44 6174 6146 7261  rval, pd.DataFra
-0002d800: 6d65 5d3a 0a20 2020 2022 2222 2046 6f72  me]:.    """ For
-0002d810: 2065 6163 6820 696e 7465 7276 616c 2c20   each interval, 
-0002d820: 6372 6561 7465 2061 2063 6875 6e6b 206f  create a chunk o
-0002d830: 6620 7468 6520 6769 7665 6e20 4461 7461  f the given Data
-0002d840: 4672 616d 6520 6261 7365 6420 6f6e 2069  Frame based on i
-0002d850: 7473 2049 6e74 6572 7661 6c49 6e64 6578  ts IntervalIndex
-0002d860: 2e0a 2020 2020 5468 6973 2069 7320 616e  ..    This is an
-0002d870: 206f 7074 696d 697a 6564 2061 6c67 6f72   optimized algor
-0002d880: 6974 686d 2063 6f6d 7061 7265 6420 746f  ithm compared to
-0002d890: 2063 616c 6c69 6e67 2049 6e74 6572 7661   calling Interva
-0002d8a0: 6c49 6e64 6578 2e6f 7665 726c 6170 7328  lIndex.overlaps(
-0002d8b0: 696e 7465 7276 616c 2920 666f 7220 6561  interval) for ea
-0002d8c0: 6368 0a20 2020 2067 6976 656e 2069 6e74  ch.    given int
-0002d8d0: 6572 7661 6c2c 2077 6974 6820 7468 6520  erval, with the 
-0002d8e0: 6164 6469 7469 6f6e 616c 2061 6476 616e  additional advan
-0002d8f0: 7461 6765 2074 6861 7420 6974 2077 696c  tage that it wil
-0002d900: 6c20 6e6f 7420 6469 7363 6172 6420 726f  l not discard ro
-0002d910: 7773 2077 6865 7265 2074 6865 0a20 2020  ws where the.   
-0002d920: 2069 6e74 6572 7661 6c20 6973 207a 6572   interval is zer
-0002d930: 6f2c 2073 7563 6820 6173 205b 3235 2e30  o, such as [25.0
-0002d940: 2c20 3235 2e30 292e 0a0a 2020 2020 5061  , 25.0)...    Pa
-0002d950: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0002d960: 2d2d 2d2d 2d2d 2d0a 2020 2020 6466 203a  -------.    df :
-0002d970: 203a 6f62 6a3a 6070 616e 6461 732e 4461   :obj:`pandas.Da
-0002d980: 7461 4672 616d 6560 0a20 2020 2020 2020  taFrame`.       
-0002d990: 2054 6865 2044 6174 6146 7261 6d65 2069   The DataFrame i
-0002d9a0: 7320 6578 7065 6374 6564 2074 6f20 636f  s expected to co
-0002d9b0: 6d65 2077 6974 6820 616e 2049 6e74 6572  me with an Inter
-0002d9c0: 7661 6c49 6e64 6578 2061 6e64 2063 6f6e  valIndex and con
-0002d9d0: 7461 696e 2074 6865 2063 6f6c 756d 6e73  tain the columns
-0002d9e0: 2027 7175 6172 7465 7262 6561 7473 2720   'quarterbeats' 
-0002d9f0: 616e 6420 2764 7572 6174 696f 6e5f 7162  and 'duration_qb
-0002da00: 272e 0a20 2020 2020 2020 2054 686f 7365  '..        Those
-0002da10: 2063 616e 2062 6520 6f62 7461 696e 6564   can be obtained
-0002da20: 2074 6872 6f75 6768 2060 6050 6172 7365   through ``Parse
-0002da30: 2e67 6574 5f6c 6973 7473 2869 6e74 6572  .get_lists(inter
-0002da40: 7661 6c5f 696e 6465 783d 5472 7565 2960  val_index=True)`
-0002da50: 6020 6f72 0a20 2020 2020 2020 2060 6050  ` or.        ``P
-0002da60: 6172 7365 2e69 7465 725f 7472 616e 7366  arse.iter_transf
-0002da70: 6f72 6d65 6428 696e 7465 7276 616c 5f69  ormed(interval_i
-0002da80: 6e64 6578 3d54 7275 6529 6060 2e0a 2020  ndex=True)``..  
-0002da90: 2020 696e 7465 7276 616c 7320 3a20 3a6f    intervals : :o
-0002daa0: 626a 3a60 6c69 7374 6020 6f66 203a 6f62  bj:`list` of :ob
-0002dab0: 6a3a 6070 642e 496e 7465 7276 616c 600a  j:`pd.Interval`.
-0002dac0: 2020 2020 2020 2020 5468 6520 696e 7465          The inte
-0002dad0: 7276 616c 7320 6465 6669 6e69 6e67 2074  rvals defining t
-0002dae0: 6865 2063 6875 6e6b 7327 2064 696d 656e  he chunks' dimen
-0002daf0: 7369 6f6e 732e 2045 7870 6563 7465 6420  sions. Expected 
-0002db00: 746f 2062 6520 6e6f 6e2d 6f76 6572 6c61  to be non-overla
-0002db10: 7070 696e 6720 616e 6420 6d6f 6e6f 746f  pping and monoto
-0002db20: 6e69 6361 6c6c 7920 696e 6372 6561 7369  nically increasi
-0002db30: 6e67 2e0a 2020 2020 7472 756e 6361 7465  ng..    truncate
-0002db40: 203a 203a 6f62 6a3a 6062 6f6f 6c60 2c20   : :obj:`bool`, 
-0002db50: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0002db60: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-0002db70: 652c 206d 6561 6e69 6e67 2074 6861 7420  e, meaning that 
-0002db80: 7468 6520 696e 7465 7276 616c 2069 6e64  the interval ind
-0002db90: 6578 2061 6e64 2074 6865 2027 6475 7261  ex and the 'dura
-0002dba0: 7469 6f6e 5f71 6227 2077 696c 6c20 6265  tion_qb' will be
-0002dbb0: 2061 6461 7074 6564 2066 6f72 206f 7665   adapted for ove
-0002dbc0: 726c 6170 7069 6e67 2069 6e74 6572 7661  rlapping interva
-0002dbd0: 6c73 2e0a 2020 2020 2020 2020 5061 7373  ls..        Pass
-0002dbe0: 2046 616c 7365 2074 6f20 6765 7420 6368   False to get ch
-0002dbf0: 756e 6b73 2077 6974 6820 616c 6c20 6f76  unks with all ov
-0002dc00: 6572 6c61 7070 696e 6720 696e 7465 7276  erlapping interv
-0002dc10: 616c 7320 6173 2074 6865 7920 6172 652e  als as they are.
-0002dc20: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0002dc30: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 3a6f    -------.    :o
-0002dc40: 626a 3a60 6469 6374 600a 2020 2020 2020  bj:`dict`.      
-0002dc50: 2020 7b69 6e74 6572 7661 6c20 2d3e 2063    {interval -> c
-0002dc60: 6875 6e6b 7d0a 2020 2020 2222 220a 2020  hunk}.    """.  
-0002dc70: 2020 6c65 6674 7320 3d20 6466 2e69 6e64    lefts = df.ind
-0002dc80: 6578 2e6c 6566 742e 7661 6c75 6573 2020  ex.left.values  
-0002dc90: 2020 2320 6c65 6674 7320 616e 6420 7269    # lefts and ri
-0002dca0: 6768 7473 2077 696c 6c20 6765 7420 7368  ghts will get sh
-0002dcb0: 6f72 7465 7220 2870 6f74 656e 7469 616c  orter (potential
-0002dcc0: 6c79 2920 7769 7468 2065 7665 7279 0a20  ly) with every. 
-0002dcd0: 2020 2072 6967 6874 7320 3d20 6466 2e69     rights = df.i
-0002dce0: 6e64 6578 2e72 6967 6874 2e76 616c 7565  ndex.right.value
-0002dcf0: 7320 2023 2069 6e74 6572 7661 6c2c 2069  s  # interval, i
-0002dd00: 6e20 6f72 6465 7220 746f 2072 6564 7563  n order to reduc
-0002dd10: 6520 7468 6520 7469 6d65 2066 6f72 2063  e the time for c
-0002dd20: 6f6d 7061 7269 6e67 2076 616c 7565 730a  omparing values.
-0002dd30: 2020 2020 6368 756e 6b73 203d 207b 7d0a      chunks = {}.
-0002dd40: 2020 2020 6375 7272 656e 745f 7374 6172      current_star
-0002dd50: 745f 6d61 736b 203d 206e 702e 6f6e 6573  t_mask = np.ones
-0002dd60: 286c 656e 2864 662e 696e 6465 7829 2c20  (len(df.index), 
-0002dd70: 6474 7970 6520 3d20 626f 6f6c 2920 2320  dtype = bool) # 
-0002dd80: 6c65 6e67 7468 2072 656d 6169 6e73 2074  length remains t
-0002dd90: 6865 2073 616d 650a 2020 2020 666f 7220  he same.    for 
-0002dda0: 6976 2069 6e20 696e 7465 7276 616c 733a  iv in intervals:
-0002ddb0: 0a20 2020 2020 2020 2023 2061 7373 756d  .        # assum
-0002ddc0: 6573 2069 6e74 6572 7661 6c73 2061 7265  es intervals are
-0002ddd0: 206e 6f6e 2d6f 7665 726c 6170 7069 6e67   non-overlapping
-0002dde0: 2061 6e64 206d 6f6e 6f74 6f6e 6963 616c   and monotonical
-0002ddf0: 6c79 2069 6e63 7265 6173 696e 670a 2020  ly increasing.  
-0002de00: 2020 2020 2020 6c2c 2072 203d 2069 762e        l, r = iv.
-0002de10: 6c65 6674 2c20 6976 2e72 6967 6874 0a20  left, iv.right. 
-0002de20: 2020 2020 2020 2023 206e 6576 6572 2061         # never a
-0002de30: 6761 696e 2063 6865 636b 2065 7665 6e74  gain check event
-0002de40: 7320 656e 6469 6e67 2062 6566 6f72 6520  s ending before 
-0002de50: 7468 6520 6375 7272 656e 7420 696e 7465  the current inte
-0002de60: 7276 616c 2773 2073 7461 7274 0a20 2020  rval's start.   
-0002de70: 2020 2020 206e 6f74 5f65 6e64 696e 675f       not_ending_
-0002de80: 6265 666f 7265 5f6c 203d 2028 7269 6768  before_l = (righ
-0002de90: 7473 203e 3d20 6c29 0a20 2020 2020 2020  ts >= l).       
-0002dea0: 206c 6566 7473 203d 206c 6566 7473 5b6e   lefts = lefts[n
-0002deb0: 6f74 5f65 6e64 696e 675f 6265 666f 7265  ot_ending_before
-0002dec0: 5f6c 5d0a 2020 2020 2020 2020 7269 6768  _l].        righ
-0002ded0: 7473 203d 2072 6967 6874 735b 6e6f 745f  ts = rights[not_
-0002dee0: 656e 6469 6e67 5f62 6566 6f72 655f 6c5d  ending_before_l]
-0002def0: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-0002df00: 5f73 7461 7274 5f6d 6173 6b5b 6375 7272  _start_mask[curr
-0002df10: 656e 745f 7374 6172 745f 6d61 736b 5d20  ent_start_mask] 
-0002df20: 3d20 6e6f 745f 656e 6469 6e67 5f62 6566  = not_ending_bef
-0002df30: 6f72 655f 6c0a 2020 2020 2020 2020 7374  ore_l.        st
-0002df40: 6172 7469 6e67 5f62 6566 6f72 655f 7220  arting_before_r 
-0002df50: 3d20 2872 203e 206c 6566 7473 290a 2020  = (r > lefts).  
-0002df60: 2020 2020 2020 6e6f 745f 656e 6469 6e67        not_ending
-0002df70: 5f6f 6e5f 6c5f 6578 6365 7074 5f65 6d70  _on_l_except_emp
-0002df80: 7479 203d 2028 7269 6768 7473 2021 3d20  ty = (rights != 
-0002df90: 6c29 207c 2028 6c65 6674 7320 3d3d 206c  l) | (lefts == l
-0002dfa0: 290a 2020 2020 2020 2020 6f76 6572 6c61  ).        overla
-0002dfb0: 7070 696e 6720 3d20 2873 7461 7274 696e  pping = (startin
-0002dfc0: 675f 6265 666f 7265 5f72 2026 206e 6f74  g_before_r & not
-0002dfd0: 5f65 6e64 696e 675f 6f6e 5f6c 5f65 7863  _ending_on_l_exc
-0002dfe0: 6570 745f 656d 7074 7929 0a20 2020 2020  ept_empty).     
-0002dff0: 2020 2062 6f6f 6c5f 6d61 736b 203d 2063     bool_mask = c
-0002e000: 7572 7265 6e74 5f73 7461 7274 5f6d 6173  urrent_start_mas
-0002e010: 6b2e 636f 7079 2829 0a20 2020 2020 2020  k.copy().       
-0002e020: 2062 6f6f 6c5f 6d61 736b 5b63 7572 7265   bool_mask[curre
-0002e030: 6e74 5f73 7461 7274 5f6d 6173 6b5d 203d  nt_start_mask] =
-0002e040: 206f 7665 726c 6170 7069 6e67 0a20 2020   overlapping.   
-0002e050: 2020 2020 2063 6875 6e6b 203d 2064 665b       chunk = df[
-0002e060: 626f 6f6c 5f6d 6173 6b5d 2e63 6f70 7928  bool_mask].copy(
-0002e070: 290a 2020 2020 2020 2020 6966 2074 7275  ).        if tru
-0002e080: 6e63 6174 653a 0a20 2020 2020 2020 2020  ncate:.         
-0002e090: 2020 206e 6577 5f6c 6566 7473 2c20 6e65     new_lefts, ne
-0002e0a0: 775f 7269 6768 7473 203d 206c 6566 7473  w_rights = lefts
-0002e0b0: 5b6f 7665 726c 6170 7069 6e67 5d2c 2072  [overlapping], r
-0002e0c0: 6967 6874 735b 6f76 6572 6c61 7070 696e  ights[overlappin
-0002e0d0: 675d 0a20 2020 2020 2020 2020 2020 2073  g].            s
-0002e0e0: 7461 7274 696e 675f 6265 666f 7265 5f6c  tarting_before_l
-0002e0f0: 2c20 656e 6469 6e67 5f61 6674 6572 5f72  , ending_after_r
-0002e100: 203d 2028 6e65 775f 6c65 6674 7320 3c20   = (new_lefts < 
-0002e110: 6c29 2c20 286e 6577 5f72 6967 6874 7320  l), (new_rights 
-0002e120: 3e20 7229 0a20 2020 2020 2020 2020 2020  > r).           
-0002e130: 2069 6620 7374 6172 7469 6e67 5f62 6566   if starting_bef
-0002e140: 6f72 655f 6c2e 7375 6d28 2920 3e20 3020  ore_l.sum() > 0 
-0002e150: 6f72 2065 6e64 696e 675f 6166 7465 725f  or ending_after_
-0002e160: 722e 7375 6d28 2920 3e20 303a 0a20 2020  r.sum() > 0:.   
-0002e170: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0002e180: 5f6c 6566 7473 5b73 7461 7274 696e 675f  _lefts[starting_
-0002e190: 6265 666f 7265 5f6c 5d20 3d20 6c0a 2020  before_l] = l.  
-0002e1a0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0002e1b0: 775f 7269 6768 7473 5b65 6e64 696e 675f  w_rights[ending_
-0002e1c0: 6166 7465 725f 725d 203d 2072 0a20 2020  after_r] = r.   
-0002e1d0: 2020 2020 2020 2020 2020 2020 2063 6875               chu
-0002e1e0: 6e6b 2e69 6e64 6578 203d 2070 642e 496e  nk.index = pd.In
-0002e1f0: 7465 7276 616c 496e 6465 782e 6672 6f6d  tervalIndex.from
-0002e200: 5f61 7272 6179 7328 6e65 775f 6c65 6674  _arrays(new_left
-0002e210: 732c 206e 6577 5f72 6967 6874 732c 2063  s, new_rights, c
-0002e220: 6c6f 7365 643d 276c 6566 7427 290a 2020  losed='left').  
-0002e230: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-0002e240: 756e 6b2e 6475 7261 7469 6f6e 5f71 6220  unk.duration_qb 
-0002e250: 3d20 286e 6577 5f72 6967 6874 7320 2d20  = (new_rights - 
-0002e260: 6e65 775f 6c65 6674 7329 0a20 2020 2020  new_lefts).     
-0002e270: 2020 2020 2020 2020 2020 2063 6875 6e6b             chunk
-0002e280: 2e71 7561 7274 6572 6265 6174 7320 3d20  .quarterbeats = 
-0002e290: 6e65 775f 6c65 6674 730a 2020 2020 2020  new_lefts.      
-0002e2a0: 2020 2020 2020 2020 2020 6368 756e 6b2e            chunk.
-0002e2b0: 736f 7274 5f76 616c 7565 7328 5b27 7175  sort_values(['qu
-0002e2c0: 6172 7465 7262 6561 7473 272c 2027 6475  arterbeats', 'du
-0002e2d0: 7261 7469 6f6e 5f71 6227 5d2c 2069 6e70  ration_qb'], inp
-0002e2e0: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
-0002e2f0: 2020 2063 6875 6e6b 735b 6976 5d20 3d20     chunks[iv] = 
-0002e300: 6368 756e 6b0a 2020 2020 7265 7475 726e  chunk.    return
-0002e310: 2063 6875 6e6b 730a 0a0a 6465 6620 696e   chunks...def in
-0002e320: 6665 725f 7473 765f 7479 7065 2864 663a  fer_tsv_type(df:
-0002e330: 2070 642e 4461 7461 4672 616d 6529 202d   pd.DataFrame) -
-0002e340: 3e20 4f70 7469 6f6e 616c 5b73 7472 5d3a  > Optional[str]:
-0002e350: 0a20 2020 2022 2222 496e 6665 7273 2074  .    """Infers t
-0002e360: 6865 2063 6f6e 7465 6e74 7320 6f66 2061  he contents of a
-0002e370: 2044 6174 6146 7261 6d65 2066 726f 6d20   DataFrame from 
-0002e380: 7468 6520 7072 6573 656e 6365 206f 6620  the presence of 
-0002e390: 7061 7274 6963 756c 6172 2063 6f6c 756d  particular colum
-0002e3a0: 6e73 2e22 2222 0a20 2020 2074 7970 6532  ns.""".    type2
-0002e3b0: 636f 6c73 203d 207b 0a20 2020 2020 2020  cols = {.       
-0002e3c0: 2027 6e6f 7465 7327 3a20 5b27 7470 6327   'notes': ['tpc'
-0002e3d0: 2c20 276d 6964 6927 5d2c 0a20 2020 2020  , 'midi'],.     
-0002e3e0: 2020 2027 6576 656e 7473 273a 205b 2743     'events': ['C
-0002e3f0: 686f 7264 2f64 7572 6174 696f 6e54 7970  hord/durationTyp
-0002e400: 6527 2c20 2752 6573 742f 6475 7261 7469  e', 'Rest/durati
-0002e410: 6f6e 5479 7065 275d 2c0a 2020 2020 2020  onType'],.      
-0002e420: 2020 2763 686f 7264 7327 3a20 5b27 6368    'chords': ['ch
-0002e430: 6f72 645f 6964 275d 2c0a 2020 2020 2020  ord_id'],.      
-0002e440: 2020 2772 6573 7473 273a 205b 276e 6f6d    'rests': ['nom
-0002e450: 696e 616c 5f64 7572 6174 696f 6e27 5d2c  inal_duration'],
-0002e460: 0a20 2020 2020 2020 2027 6578 7061 6e64  .        'expand
-0002e470: 6564 273a 205b 276e 756d 6572 616c 275d  ed': ['numeral']
-0002e480: 2c0a 2020 2020 2020 2020 276c 6162 656c  ,.        'label
-0002e490: 7327 3a20 5b27 6861 726d 6f6e 795f 6c61  s': ['harmony_la
-0002e4a0: 7965 7227 2c20 276c 6162 656c 272c 2027  yer', 'label', '
-0002e4b0: 6c61 6265 6c5f 7479 7065 275d 2c0a 2020  label_type'],.  
-0002e4c0: 2020 2020 2020 276d 6561 7375 7265 7327        'measures'
-0002e4d0: 3a20 5b27 6163 745f 6475 7227 5d2c 0a20  : ['act_dur'],. 
-0002e4e0: 2020 2020 2020 2027 6361 6465 6e63 6573         'cadences
-0002e4f0: 273a 205b 2763 6164 656e 6365 275d 2c0a  ': ['cadence'],.
-0002e500: 2020 2020 2020 2020 276d 6574 6164 6174          'metadat
-0002e510: 6127 3a20 5b27 666e 616d 6527 5d2c 0a20  a': ['fname'],. 
-0002e520: 2020 2020 2020 2027 666f 726d 5f6c 6162         'form_lab
-0002e530: 656c 7327 3a20 5b27 666f 726d 5f6c 6162  els': ['form_lab
-0002e540: 656c 272c 2027 6127 5d2c 0a20 2020 207d  el', 'a'],.    }
-0002e550: 0a20 2020 2066 6f72 2074 2c20 636f 6c75  .    for t, colu
-0002e560: 6d6e 7320 696e 2074 7970 6532 636f 6c73  mns in type2cols
-0002e570: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-0002e580: 2020 6966 2061 6e79 2863 2069 6e20 6466    if any(c in df
-0002e590: 2e63 6f6c 756d 6e73 2066 6f72 2063 2069  .columns for c i
-0002e5a0: 6e20 636f 6c75 6d6e 7329 3a0a 2020 2020  n columns):.    
-0002e5b0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-0002e5c0: 0a20 2020 2069 6620 616e 7928 6320 696e  .    if any(c in
-0002e5d0: 2064 662e 636f 6c75 6d6e 7320 666f 7220   df.columns for 
-0002e5e0: 6320 696e 205b 276d 6327 2c20 276d 6e27  c in ['mc', 'mn'
-0002e5f0: 5d29 3a0a 2020 2020 2020 2020 7265 7475  ]):.        retu
-0002e600: 726e 2027 6c61 6265 6c73 270a 2020 2020  rn 'labels'.    
-0002e610: 7265 7475 726e 2027 756e 6b6e 6f77 6e27  return 'unknown'
-0002e620: 0a0a 0a64 6566 2072 6564 7563 655f 6461  ...def reduce_da
-0002e630: 7461 6672 616d 655f 6475 7261 7469 6f6e  taframe_duration
-0002e640: 5f74 6f5f 6669 7273 745f 726f 7728 6466  _to_first_row(df
-0002e650: 3a20 7064 2e44 6174 6146 7261 6d65 2920  : pd.DataFrame) 
-0002e660: 2d3e 2070 642e 4461 7461 4672 616d 653a  -> pd.DataFrame:
-0002e670: 0a20 2020 2022 2222 2052 6564 7563 6573  .    """ Reduces
-0002e680: 2061 2044 6174 6146 7261 6d65 2074 6f20   a DataFrame to 
-0002e690: 6974 7320 726f 7720 616e 6420 7570 6461  its row and upda
-0002e6a0: 7465 7320 7468 6520 6475 7261 7469 6f6e  tes the duration
-0002e6b0: 5f71 6220 636f 6c75 6d6e 2074 6f20 7265  _qb column to re
-0002e6c0: 666c 6563 7420 7468 6520 7265 6475 6365  flect the reduce
-0002e6d0: 6420 6475 7261 7469 6f6e 2e0a 0a20 2020  d duration...   
-0002e6e0: 2041 7267 733a 0a20 2020 2020 2064 663a   Args:.      df:
-0002e6f0: 2044 6174 6166 7261 6d65 206f 6620 7768   Dataframe of wh
-0002e700: 6963 6820 746f 206b 6565 7020 6f6e 6c79  ich to keep only
-0002e710: 2074 6865 2066 6972 7374 2072 6f77 2e20   the first row. 
-0002e720: 4966 2069 7420 6861 7320 616e 2049 6e74  If it has an Int
-0002e730: 6572 7661 6c49 6e64 6578 2c20 7468 6520  ervalIndex, the 
-0002e740: 696e 7465 7276 616c 2069 7320 7570 6461  interval is upda
-0002e750: 7465 6420 746f 0a20 2020 2020 2020 2020  ted to.         
-0002e760: 2072 6566 6c65 6374 2074 6865 2077 686f   reflect the who
-0002e770: 6c65 2064 7572 6174 696f 6e2e 0a0a 2020  le duration...  
-0002e780: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0002e790: 2044 6174 6146 7261 6d65 2077 6974 6820   DataFrame with 
-0002e7a0: 6f6e 6520 726f 772e 0a20 2020 2022 2222  one row..    """
-0002e7b0: 0a20 2020 2069 6620 6c65 6e28 6466 2920  .    if len(df) 
-0002e7c0: 3d3d 2031 3a0a 2020 2020 2020 2020 7265  == 1:.        re
-0002e7d0: 7475 726e 2064 660a 2020 2020 6964 7820  turn df.    idx 
-0002e7e0: 3d20 6466 2e69 6e64 6578 0a20 2020 2066  = df.index.    f
-0002e7f0: 6972 7374 5f6c 6f63 203d 2069 6478 5b30  irst_loc = idx[0
-0002e800: 5d0a 2020 2020 726f 7720 3d20 6466 2e69  ].    row = df.i
-0002e810: 6c6f 635b 5b30 5d5d 0a20 2020 2023 2069  loc[[0]].    # i
-0002e820: 6620 6973 696e 7374 616e 6365 2869 782c  f isinstance(ix,
-0002e830: 2070 642e 496e 7465 7276 616c 2920 6f72   pd.Interval) or
-0002e840: 2028 6973 696e 7374 616e 6365 2869 782c   (isinstance(ix,
-0002e850: 2074 7570 6c65 2920 616e 6420 6973 696e   tuple) and isin
-0002e860: 7374 616e 6365 2869 785b 2d31 5d2c 2070  stance(ix[-1], p
-0002e870: 642e 496e 7465 7276 616c 2929 3a0a 2020  d.Interval)):.  
-0002e880: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0002e890: 6964 782c 2070 642e 496e 7465 7276 616c  idx, pd.Interval
-0002e8a0: 496e 6465 7829 3a0a 2020 2020 2020 2020  Index):.        
-0002e8b0: 7374 6172 7420 3d20 6d69 6e28 6964 782e  start = min(idx.
-0002e8c0: 6c65 6674 290a 2020 2020 2020 2020 656e  left).        en
-0002e8d0: 6420 3d20 6d61 7828 6964 782e 7269 6768  d = max(idx.righ
-0002e8e0: 7429 0a20 2020 2020 2020 2069 7620 3d20  t).        iv = 
-0002e8f0: 7064 2e49 6e74 6572 7661 6c28 7374 6172  pd.Interval(star
-0002e900: 742c 2065 6e64 2c20 636c 6f73 6564 3d69  t, end, closed=i
-0002e910: 6478 2e63 6c6f 7365 6429 0a20 2020 2020  dx.closed).     
-0002e920: 2020 2072 6f77 2e69 6e64 6578 203d 2070     row.index = p
-0002e930: 642e 496e 7465 7276 616c 496e 6465 7828  d.IntervalIndex(
-0002e940: 5b69 765d 290a 2020 2020 2020 2020 726f  [iv]).        ro
-0002e950: 772e 6c6f 635b 6976 2c20 2764 7572 6174  w.loc[iv, 'durat
-0002e960: 696f 6e5f 7162 275d 203d 2069 762e 6c65  ion_qb'] = iv.le
-0002e970: 6e67 7468 0a20 2020 2065 6c73 653a 0a20  ngth.    else:. 
-0002e980: 2020 2020 2020 206e 6577 5f64 7572 6174         new_durat
-0002e990: 696f 6e20 3d20 6466 2e64 7572 6174 696f  ion = df.duratio
-0002e9a0: 6e5f 7162 2e73 756d 2829 0a20 2020 2020  n_qb.sum().     
-0002e9b0: 2020 2072 6f77 2e6c 6f63 5b66 6972 7374     row.loc[first
-0002e9c0: 5f6c 6f63 2c20 2764 7572 6174 696f 6e5f  _loc, 'duration_
-0002e9d0: 7162 275d 203d 206e 6577 5f64 7572 6174  qb'] = new_durat
-0002e9e0: 696f 6e0a 2020 2020 7265 7475 726e 2072  ion.    return r
-0002e9f0: 6f77 0a0a 0a40 6461 7461 636c 6173 730a  ow...@dataclass.
-0002ea00: 636c 6173 7320 4669 6c65 3a0a 2020 2020  class File:.    
-0002ea10: 2222 2253 746f 7269 6e67 2070 6174 6820  """Storing path 
-0002ea20: 616e 6420 6669 6c65 206e 616d 6520 696e  and file name in
-0002ea30: 666f 726d 6174 696f 6e20 666f 7220 6f6e  formation for on
-0002ea40: 6520 6669 6c65 2e22 2222 0a20 2020 2069  e file.""".    i
-0002ea50: 783a 2069 6e74 0a20 2020 2022 2222 496e  x: int.    """In
-0002ea60: 6465 7820 696e 7465 6765 7220 2849 4429  dex integer (ID)
-0002ea70: 2222 220a 2020 2020 7479 7065 3a20 7374  """.    type: st
-0002ea80: 720a 2020 2020 2222 2252 6563 6f67 6e69  r.    """Recogni
-0002ea90: 7a65 6420 7479 7065 20e2 8888 203a 6174  zed type ... :at
-0002eaa0: 7472 3a60 6d73 332e 5f74 7970 696e 672e  tr:`ms3._typing.
-0002eab0: 4661 6365 7460 2222 220a 2020 2020 6669  Facet`""".    fi
-0002eac0: 6c65 3a20 7374 720a 2020 2020 2222 2246  le: str.    """F
-0002ead0: 696c 6520 6e61 6d65 2069 6e63 6c75 6469  ile name includi
-0002eae0: 6e67 2065 7874 656e 7369 6f6e 2e22 2222  ng extension."""
-0002eaf0: 0a20 2020 2066 6e61 6d65 3a20 7374 720a  .    fname: str.
-0002eb00: 2020 2020 2222 2266 6e61 6d65 2065 7863      """fname exc
-0002eb10: 6c75 6469 6e67 2074 6865 2073 7566 6669  luding the suffi
-0002eb20: 7820 2861 6674 6572 2072 6567 6973 7465  x (after registe
-0002eb30: 7269 6e67 2074 6865 2066 696c 6520 7769  ring the file wi
-0002eb40: 7468 2061 203a 6f62 6a3a 6050 6965 6365  th a :obj:`Piece
-0002eb50: 6029 2e22 2222 0a20 2020 2066 6578 743a  `).""".    fext:
-0002eb60: 2073 7472 0a20 2020 2022 2222 4669 6c65   str.    """File
-0002eb70: 2065 7874 656e 7369 6f6e 732e 2222 220a   extensions.""".
-0002eb80: 2020 2020 7375 6264 6972 3a20 7374 720a      subdir: str.
-0002eb90: 2020 2020 2222 2244 6972 6563 746f 7279      """Directory
-0002eba0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-0002ebb0: 2063 6f72 7075 7320 7061 7468 2028 652e   corpus path (e.
-0002ebc0: 672e 2027 2e2f 4d53 3327 292e 2222 220a  g. './MS3').""".
-0002ebd0: 2020 2020 636f 7270 7573 5f70 6174 683a      corpus_path:
-0002ebe0: 2073 7472 0a20 2020 2022 2222 4162 736f   str.    """Abso
-0002ebf0: 6c75 7465 2070 6174 6820 6f66 2074 6865  lute path of the
-0002ec00: 2066 696c 6527 7320 7061 7265 6e74 2064   file's parent d
-0002ec10: 6972 6563 746f 7279 2074 6861 7420 6973  irectory that is
-0002ec20: 2063 6f6e 7369 6465 7265 6420 6173 2063   considered as c
-0002ec30: 6f72 7075 7320 6469 7265 6374 6f72 792e  orpus directory.
-0002ec40: 2222 220a 2020 2020 7265 6c5f 7061 7468  """.    rel_path
-0002ec50: 3a20 7374 720a 2020 2020 2222 2246 696c  : str.    """Fil
-0002ec60: 6520 7061 7468 2072 656c 6174 6976 6520  e path relative 
-0002ec70: 746f 2074 6865 2063 6f72 7075 7320 7061  to the corpus pa
-0002ec80: 7468 2e20 4571 7569 7661 6c65 6e74 2074  th. Equivalent t
-0002ec90: 6f20 3c73 7562 6469 723e 2f3c 6669 6c65  o <subdir>/<file
-0002eca0: 3e2e 2222 220a 2020 2020 6675 6c6c 5f70  >.""".    full_p
-0002ecb0: 6174 683a 2073 7472 0a20 2020 2022 2222  ath: str.    """
-0002ecc0: 4162 736f 6c75 7465 2066 696c 6520 7061  Absolute file pa
-0002ecd0: 7468 2e22 2222 0a20 2020 2064 6972 6563  th.""".    direc
-0002ece0: 746f 7279 3a20 7374 720a 2020 2020 2222  tory: str.    ""
-0002ecf0: 2241 6273 6f6c 7574 6520 666f 6c64 6572  "Absolute folder
-0002ed00: 2070 6174 6820 7768 6572 6520 7468 6520   path where the 
-0002ed10: 6669 6c65 2069 7320 6c6f 6361 7465 642e  file is located.
-0002ed20: 2222 220a 2020 2020 7375 6666 6978 3a20  """.    suffix: 
-0002ed30: 7374 7220 3d20 2727 0a20 2020 2022 2222  str = ''.    """
-0002ed40: 5570 6f6e 2072 6567 6973 7465 7269 6e67  Upon registering
-0002ed50: 2074 6865 2046 696c 6520 7769 7468 2061   the File with a
-0002ed60: 203a 6f62 6a3a 6050 6965 6365 602c 2069   :obj:`Piece`, i
-0002ed70: 6620 7468 6520 6375 7272 656e 7420 666e  f the current fn
-0002ed80: 616d 6520 6861 7320 6120 7375 6666 6978  ame has a suffix
-0002ed90: 2063 6f6d 7061 7265 6420 746f 2074 6865   compared to the
-0002eda0: 2050 6965 6365 2773 2066 6e61 6d65 2c20   Piece's fname, 
-0002edb0: 0a20 2020 2073 7566 6669 7820 6973 2072  .    suffix is r
-0002edc0: 656d 6f76 6564 2066 726f 6d20 7468 6520  emoved from the 
-0002edd0: 4669 6c65 206f 626a 6563 7427 7320 666e  File object's fn
-0002ede0: 616d 6520 6669 656c 6420 616e 6420 6164  ame field and ad
-0002edf0: 6465 6420 746f 2074 6865 2073 7566 6669  ded to the suffi
-0002ee00: 7820 6669 656c 642e 2222 220a 2020 2020  x field.""".    
-0002ee10: 636f 6d6d 6974 5f73 6861 3a20 7374 7220  commit_sha: str 
-0002ee20: 3d20 2727 0a20 2020 2022 2222 5468 6520  = ''.    """The 
-0002ee30: 7468 6520 6669 6c65 2068 6173 2062 6565  the file has bee
-0002ee40: 6e20 7265 7472 6965 7665 6420 6672 6f6d  n retrieved from
-0002ee50: 2061 2070 6172 7469 6375 6c61 7220 6769   a particular gi
-0002ee60: 7420 7265 7669 7369 6f6e 2c20 7468 6973  t revision, this
-0002ee70: 2069 7320 7365 7420 746f 2074 6865 2072   is set to the r
-0002ee80: 6576 6973 696f 6e27 7320 6861 7368 2e22  evision's hash."
-0002ee90: 2222 0a0a 2020 2020 6465 6620 5f5f 7265  ""..    def __re
-0002eea0: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-0002eeb0: 2020 2020 7375 6666 6978 203d 2027 2720      suffix = '' 
-0002eec0: 6966 2073 656c 662e 7375 6666 6978 203d  if self.suffix =
-0002eed0: 3d20 2727 2065 6c73 6520 6622 2c20 7375  = '' else f", su
-0002eee0: 6666 6978 3a20 7b73 656c 662e 7375 6666  ffix: {self.suff
-0002eef0: 6978 7d2e 220a 2020 2020 2020 2020 636f  ix}.".        co
-0002ef00: 6d6d 6974 203d 2027 2720 6966 2073 656c  mmit = '' if sel
-0002ef10: 662e 636f 6d6d 6974 5f73 6861 203d 3d20  f.commit_sha == 
-0002ef20: 2727 2065 6c73 6520 6622 407b 7365 6c66  '' else f"@{self
-0002ef30: 2e63 6f6d 6d69 745f 7368 615b 3a37 5d7d  .commit_sha[:7]}
-0002ef40: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0002ef50: 2066 227b 7365 6c66 2e69 787d 3a20 277b   f"{self.ix}: '{
-0002ef60: 7365 6c66 2e72 656c 5f70 6174 687d 277b  self.rel_path}'{
-0002ef70: 636f 6d6d 6974 7d7b 7375 6666 6978 7d22  commit}{suffix}"
-0002ef80: 0a0a 2020 2020 6465 6620 7265 706c 6163  ..    def replac
-0002ef90: 655f 6578 7465 6e73 696f 6e28 7365 6c66  e_extension(self
-0002efa0: 2c20 6e65 775f 6578 7465 6e73 696f 6e3a  , new_extension:
-0002efb0: 2073 7472 2c20 2a2a 6b77 6172 6773 2920   str, **kwargs) 
-0002efc0: 2d3e 2053 656c 663a 0a20 2020 2020 2020  -> Self:.       
-0002efd0: 2069 6620 6e65 775f 6578 7465 6e73 696f   if new_extensio
-0002efe0: 6e5b 305d 2021 3d20 272e 273a 0a20 2020  n[0] != '.':.   
-0002eff0: 2020 2020 2020 2020 206e 6577 5f65 7874           new_ext
-0002f000: 656e 7369 6f6e 203d 2027 2e27 202b 206e  ension = '.' + n
-0002f010: 6577 5f65 7874 656e 7369 6f6e 0a20 2020  ew_extension.   
-0002f020: 2020 2020 206f 6c64 5f65 7874 5f6c 656e       old_ext_len
-0002f030: 203d 206c 656e 2873 656c 662e 6665 7874   = len(self.fext
-0002f040: 290a 2020 2020 2020 2020 6e65 775f 7661  ).        new_va
-0002f050: 6c73 203d 207b 7d0a 2020 2020 2020 2020  ls = {}.        
-0002f060: 666f 7220 6669 656c 6420 696e 2028 2266  for field in ("f
-0002f070: 696c 6522 2c20 2266 6578 7422 2c20 2272  ile", "fext", "r
-0002f080: 656c 5f70 6174 6822 2c20 2266 756c 6c5f  el_path", "full_
-0002f090: 7061 7468 2229 3a0a 2020 2020 2020 2020  path"):.        
-0002f0a0: 2020 2020 6f6c 645f 7661 6c20 3d20 6765      old_val = ge
-0002f0b0: 7461 7474 7228 7365 6c66 2c20 6669 656c  tattr(self, fiel
-0002f0c0: 6429 0a20 2020 2020 2020 2020 2020 206e  d).            n
-0002f0d0: 6577 5f76 616c 735b 6669 656c 645d 203d  ew_vals[field] =
-0002f0e0: 206f 6c64 5f76 616c 5b3a 2d6f 6c64 5f65   old_val[:-old_e
-0002f0f0: 7874 5f6c 656e 5d20 2b20 6e65 775f 6578  xt_len] + new_ex
-0002f100: 7465 6e73 696f 6e0a 2020 2020 2020 2020  tension.        
-0002f110: 7265 7475 726e 2072 6570 6c61 6365 2873  return replace(s
-0002f120: 656c 662c 202a 2a6e 6577 5f76 616c 732c  elf, **new_vals,
-0002f130: 202a 2a6b 7761 7267 7329 0a0a 0a20 2020   **kwargs)...   
-0002f140: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-0002f150: 2020 6465 6620 6672 6f6d 5f63 6f72 7075    def from_corpu
-0002f160: 735f 7061 7468 2863 6c73 2c0a 2020 2020  s_path(cls,.    
-0002f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f180: 2020 2020 2063 6f72 7075 735f 7061 7468       corpus_path
-0002f190: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
-0002f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f1b0: 6669 6c65 6e61 6d65 3a20 7374 722c 0a20  filename: str,. 
-0002f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f1d0: 2020 2020 2020 2020 6674 7970 653a 204f          ftype: O
-0002f1e0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0002f1f0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0002f200: 2020 2020 2020 2020 2020 2020 2020 7375                su
-0002f210: 6264 6972 3d27 2e27 2c0a 2020 2020 2020  bdir='.',.      
-0002f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f230: 2020 2069 783a 2069 6e74 203d 202d 3129     ix: int = -1)
-0002f240: 3a0a 2020 2020 2020 2020 2222 2220 4372  :.        """ Cr
-0002f250: 6561 7465 7320 4669 6c65 206f 626a 6563  eates File objec
-0002f260: 7420 6672 6f6d 2069 6e64 6976 6964 7561  t from individua
-0002f270: 6c20 636f 6d70 6f6e 656e 7473 0a0a 2020  l components..  
-0002f280: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0002f290: 2020 2020 2020 2020 636f 7270 7573 5f70          corpus_p
-0002f2a0: 6174 683a 2052 6f6f 7420 6469 7265 6374  ath: Root direct
-0002f2b0: 6f72 7920 6f66 2074 6865 2066 696c 6527  ory of the file'
-0002f2c0: 7320 636f 7270 7573 2e0a 2020 2020 2020  s corpus..      
-0002f2d0: 2020 2020 2020 6669 6c65 6e61 6d65 3a20        filename: 
-0002f2e0: 4675 6c6c 2066 696c 6520 6e61 6d65 2069  Full file name i
-0002f2f0: 6e63 6c75 6469 6e67 2073 7566 6669 7865  ncluding suffixe
-0002f300: 7320 616e 6420 6578 7465 6e73 696f 6e73  s and extensions
-0002f310: 2e0a 2020 2020 2020 2020 2020 2020 6674  ..            ft
-0002f320: 7970 653a 2046 696c 6520 7479 7065 2028  ype: File type (
-0002f330: 7573 6564 2061 7320 6465 6661 756c 7420  used as default 
-0002f340: 666f 6c64 6572 206e 616d 6520 666f 7220  folder name for 
-0002f350: 6372 6561 7469 6e67 2066 696c 655f 7061  creating file_pa
-0002f360: 7468 7329 2e0a 2020 2020 2020 2020 2020  ths)..          
-0002f370: 2020 7375 6264 6972 3a20 7265 6c61 7469    subdir: relati
-0002f380: 7665 2064 6972 6563 746f 7279 2061 7070  ve directory app
-0002f390: 656e 6465 6420 746f 2063 6f72 7075 735f  ended to corpus_
-0002f3a0: 7061 7468 2c20 6465 6661 756c 7473 2074  path, defaults t
-0002f3b0: 6f20 272e 272c 2069 2e65 2e20 6e6f 2073  o '.', i.e. no s
-0002f3c0: 7562 666f 6c64 6572 2e0a 2020 2020 2020  ubfolder..      
-0002f3d0: 2020 2020 2020 6978 3a20 4172 6269 7472        ix: Arbitr
-0002f3e0: 6172 7920 696e 6465 7820 6e75 6d62 6572  ary index number
-0002f3f0: 2c20 6465 6661 756c 7473 2074 6f20 2d31  , defaults to -1
-0002f400: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0002f410: 2020 2020 2020 6675 6c6c 5f70 6174 6820        full_path 
-0002f420: 3d20 6f73 2e70 6174 682e 7265 616c 7061  = os.path.realpa
-0002f430: 7468 286f 732e 7061 7468 2e6a 6f69 6e28  th(os.path.join(
-0002f440: 636f 7270 7573 5f70 6174 682c 2073 7562  corpus_path, sub
-0002f450: 6469 722c 2066 696c 656e 616d 6529 290a  dir, filename)).
-0002f460: 2020 2020 2020 2020 6669 6c65 5f6e 616d          file_nam
-0002f470: 652c 2066 696c 655f 6578 7420 3d20 6f73  e, file_ext = os
-0002f480: 2e70 6174 682e 7370 6c69 7465 7874 2866  .path.splitext(f
-0002f490: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
-0002f4a0: 2072 656c 5f70 6174 6820 3d20 6f73 2e70   rel_path = os.p
-0002f4b0: 6174 682e 6a6f 696e 2873 7562 6469 722c  ath.join(subdir,
-0002f4c0: 2066 696c 656e 616d 6529 0a20 2020 2020   filename).     
-0002f4d0: 2020 2069 6620 6674 7970 6520 6973 204e     if ftype is N
-0002f4e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002f4f0: 2066 696c 655f 7479 7065 203d 2070 6174   file_type = pat
-0002f500: 6832 7479 7065 2866 756c 6c5f 7061 7468  h2type(full_path
-0002f510: 2c20 6c6f 6767 6572 3d73 656c 662e 6c6f  , logger=self.lo
-0002f520: 6767 6572 290a 2020 2020 2020 2020 656c  gger).        el
-0002f530: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0002f540: 6669 6c65 5f74 7970 6520 3d20 6674 7970  file_type = ftyp
-0002f550: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0002f560: 2063 6c73 280a 2020 2020 2020 2020 2020   cls(.          
-0002f570: 2020 6978 3d69 782c 0a20 2020 2020 2020    ix=ix,.       
-0002f580: 2020 2020 2074 7970 653d 6669 6c65 5f74       type=file_t
-0002f590: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
-0002f5a0: 2066 696c 653d 6669 6c65 6e61 6d65 2c0a   file=filename,.
-0002f5b0: 2020 2020 2020 2020 2020 2020 666e 616d              fnam
-0002f5c0: 653d 6669 6c65 5f6e 616d 652c 0a20 2020  e=file_name,.   
-0002f5d0: 2020 2020 2020 2020 2066 6578 743d 6669           fext=fi
-0002f5e0: 6c65 5f65 7874 2c0a 2020 2020 2020 2020  le_ext,.        
-0002f5f0: 2020 2020 7375 6264 6972 3d73 7562 6469      subdir=subdi
-0002f600: 722c 0a20 2020 2020 2020 2020 2020 2063  r,.            c
-0002f610: 6f72 7075 735f 7061 7468 3d63 6f72 7075  orpus_path=corpu
-0002f620: 735f 7061 7468 2c0a 2020 2020 2020 2020  s_path,.        
-0002f630: 2020 2020 7265 6c5f 7061 7468 3d72 656c      rel_path=rel
-0002f640: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-0002f650: 2020 2066 756c 6c5f 7061 7468 3d66 756c     full_path=ful
-0002f660: 6c5f 7061 7468 2c0a 2020 2020 2020 2020  l_path,.        
-0002f670: 2020 2020 6469 7265 6374 6f72 793d 6f73      directory=os
-0002f680: 2e70 6174 682e 6469 726e 616d 6528 6675  .path.dirname(fu
-0002f690: 6c6c 5f70 6174 6829 2c0a 2020 2020 2020  ll_path),.      
-0002f6a0: 2020 2020 2020 7375 6666 6978 3d27 272c        suffix='',
-0002f6b0: 0a20 2020 2020 2020 2029 0a0a 4066 756e  .        )..@fun
-0002f6c0: 6374 696f 6e5f 6c6f 6767 6572 0a64 6566  ction_logger.def
-0002f6d0: 2061 7574 6f6d 6174 6963 616c 6c79 5f63   automatically_c
-0002f6e0: 686f 6f73 655f 6672 6f6d 5f64 6973 616d  hoose_from_disam
-0002f6f0: 6269 6775 6174 6564 5f66 696c 6573 2864  biguated_files(d
-0002f700: 6973 616d 6269 6775 6174 6564 5f63 686f  isambiguated_cho
-0002f710: 6963 6573 3a20 4469 6374 5b73 7472 2c20  ices: Dict[str, 
-0002f720: 4669 6c65 5d2c 0a20 2020 2020 2020 2020  File],.         
-0002f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f750: 2020 2020 2020 2020 2066 6e61 6d65 3a20           fname: 
-0002f760: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0002d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d7d0: 2020 696e 7465 7276 616c 733a 204c 6973    intervals: Lis
+0002d7e0: 745b 7064 2e49 6e74 6572 7661 6c5d 2c0a  t[pd.Interval],.
+0002d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d810: 2020 2074 7275 6e63 6174 653a 2062 6f6f     truncate: boo
+0002d820: 6c20 3d20 5472 7565 2920 2d3e 2044 6963  l = True) -> Dic
+0002d830: 745b 7064 2e49 6e74 6572 7661 6c2c 2070  t[pd.Interval, p
+0002d840: 642e 4461 7461 4672 616d 655d 3a0a 2020  d.DataFrame]:.  
+0002d850: 2020 2222 2220 466f 7220 6561 6368 2069    """ For each i
+0002d860: 6e74 6572 7661 6c2c 2063 7265 6174 6520  nterval, create 
+0002d870: 6120 6368 756e 6b20 6f66 2074 6865 2067  a chunk of the g
+0002d880: 6976 656e 2044 6174 6146 7261 6d65 2062  iven DataFrame b
+0002d890: 6173 6564 206f 6e20 6974 7320 496e 7465  ased on its Inte
+0002d8a0: 7276 616c 496e 6465 782e 0a20 2020 2054  rvalIndex..    T
+0002d8b0: 6869 7320 6973 2061 6e20 6f70 7469 6d69  his is an optimi
+0002d8c0: 7a65 6420 616c 676f 7269 7468 6d20 636f  zed algorithm co
+0002d8d0: 6d70 6172 6564 2074 6f20 6361 6c6c 696e  mpared to callin
+0002d8e0: 6720 496e 7465 7276 616c 496e 6465 782e  g IntervalIndex.
+0002d8f0: 6f76 6572 6c61 7073 2869 6e74 6572 7661  overlaps(interva
+0002d900: 6c29 2066 6f72 2065 6163 680a 2020 2020  l) for each.    
+0002d910: 6769 7665 6e20 696e 7465 7276 616c 2c20  given interval, 
+0002d920: 7769 7468 2074 6865 2061 6464 6974 696f  with the additio
+0002d930: 6e61 6c20 6164 7661 6e74 6167 6520 7468  nal advantage th
+0002d940: 6174 2069 7420 7769 6c6c 206e 6f74 2064  at it will not d
+0002d950: 6973 6361 7264 2072 6f77 7320 7768 6572  iscard rows wher
+0002d960: 6520 7468 650a 2020 2020 696e 7465 7276  e the.    interv
+0002d970: 616c 2069 7320 7a65 726f 2c20 7375 6368  al is zero, such
+0002d980: 2061 7320 5b32 352e 302c 2032 352e 3029   as [25.0, 25.0)
+0002d990: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+0002d9a0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0002d9b0: 0a20 2020 2064 6620 3a20 3a6f 626a 3a60  .    df : :obj:`
+0002d9c0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+0002d9d0: 600a 2020 2020 2020 2020 5468 6520 4461  `.        The Da
+0002d9e0: 7461 4672 616d 6520 6973 2065 7870 6563  taFrame is expec
+0002d9f0: 7465 6420 746f 2063 6f6d 6520 7769 7468  ted to come with
+0002da00: 2061 6e20 496e 7465 7276 616c 496e 6465   an IntervalInde
+0002da10: 7820 616e 6420 636f 6e74 6169 6e20 7468  x and contain th
+0002da20: 6520 636f 6c75 6d6e 7320 2771 7561 7274  e columns 'quart
+0002da30: 6572 6265 6174 7327 2061 6e64 2027 6475  erbeats' and 'du
+0002da40: 7261 7469 6f6e 5f71 6227 2e0a 2020 2020  ration_qb'..    
+0002da50: 2020 2020 5468 6f73 6520 6361 6e20 6265      Those can be
+0002da60: 206f 6274 6169 6e65 6420 7468 726f 7567   obtained throug
+0002da70: 6820 6060 5061 7273 652e 6765 745f 6c69  h ``Parse.get_li
+0002da80: 7374 7328 696e 7465 7276 616c 5f69 6e64  sts(interval_ind
+0002da90: 6578 3d54 7275 6529 6060 206f 720a 2020  ex=True)`` or.  
+0002daa0: 2020 2020 2020 6060 5061 7273 652e 6974        ``Parse.it
+0002dab0: 6572 5f74 7261 6e73 666f 726d 6564 2869  er_transformed(i
+0002dac0: 6e74 6572 7661 6c5f 696e 6465 783d 5472  nterval_index=Tr
+0002dad0: 7565 2960 602e 0a20 2020 2069 6e74 6572  ue)``..    inter
+0002dae0: 7661 6c73 203a 203a 6f62 6a3a 606c 6973  vals : :obj:`lis
+0002daf0: 7460 206f 6620 3a6f 626a 3a60 7064 2e49  t` of :obj:`pd.I
+0002db00: 6e74 6572 7661 6c60 0a20 2020 2020 2020  nterval`.       
+0002db10: 2054 6865 2069 6e74 6572 7661 6c73 2064   The intervals d
+0002db20: 6566 696e 696e 6720 7468 6520 6368 756e  efining the chun
+0002db30: 6b73 2720 6469 6d65 6e73 696f 6e73 2e20  ks' dimensions. 
+0002db40: 4578 7065 6374 6564 2074 6f20 6265 206e  Expected to be n
+0002db50: 6f6e 2d6f 7665 726c 6170 7069 6e67 2061  on-overlapping a
+0002db60: 6e64 206d 6f6e 6f74 6f6e 6963 616c 6c79  nd monotonically
+0002db70: 2069 6e63 7265 6173 696e 672e 0a20 2020   increasing..   
+0002db80: 2074 7275 6e63 6174 6520 3a20 3a6f 626a   truncate : :obj
+0002db90: 3a60 626f 6f6c 602c 206f 7074 696f 6e61  :`bool`, optiona
+0002dba0: 6c0a 2020 2020 2020 2020 4465 6661 756c  l.        Defaul
+0002dbb0: 7473 2074 6f20 5472 7565 2c20 6d65 616e  ts to True, mean
+0002dbc0: 696e 6720 7468 6174 2074 6865 2069 6e74  ing that the int
+0002dbd0: 6572 7661 6c20 696e 6465 7820 616e 6420  erval index and 
+0002dbe0: 7468 6520 2764 7572 6174 696f 6e5f 7162  the 'duration_qb
+0002dbf0: 2720 7769 6c6c 2062 6520 6164 6170 7465  ' will be adapte
+0002dc00: 6420 666f 7220 6f76 6572 6c61 7070 696e  d for overlappin
+0002dc10: 6720 696e 7465 7276 616c 732e 0a20 2020  g intervals..   
+0002dc20: 2020 2020 2050 6173 7320 4661 6c73 6520       Pass False 
+0002dc30: 746f 2067 6574 2063 6875 6e6b 7320 7769  to get chunks wi
+0002dc40: 7468 2061 6c6c 206f 7665 726c 6170 7069  th all overlappi
+0002dc50: 6e67 2069 6e74 6572 7661 6c73 2061 7320  ng intervals as 
+0002dc60: 7468 6579 2061 7265 2e0a 0a20 2020 2052  they are...    R
+0002dc70: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0002dc80: 2d2d 0a20 2020 203a 6f62 6a3a 6064 6963  --.    :obj:`dic
+0002dc90: 7460 0a20 2020 2020 2020 207b 696e 7465  t`.        {inte
+0002dca0: 7276 616c 202d 3e20 6368 756e 6b7d 0a20  rval -> chunk}. 
+0002dcb0: 2020 2022 2222 0a20 2020 206c 6566 7473     """.    lefts
+0002dcc0: 203d 2064 662e 696e 6465 782e 6c65 6674   = df.index.left
+0002dcd0: 2e76 616c 7565 7320 2020 2023 206c 6566  .values    # lef
+0002dce0: 7473 2061 6e64 2072 6967 6874 7320 7769  ts and rights wi
+0002dcf0: 6c6c 2067 6574 2073 686f 7274 6572 2028  ll get shorter (
+0002dd00: 706f 7465 6e74 6961 6c6c 7929 2077 6974  potentially) wit
+0002dd10: 6820 6576 6572 790a 2020 2020 7269 6768  h every.    righ
+0002dd20: 7473 203d 2064 662e 696e 6465 782e 7269  ts = df.index.ri
+0002dd30: 6768 742e 7661 6c75 6573 2020 2320 696e  ght.values  # in
+0002dd40: 7465 7276 616c 2c20 696e 206f 7264 6572  terval, in order
+0002dd50: 2074 6f20 7265 6475 6365 2074 6865 2074   to reduce the t
+0002dd60: 696d 6520 666f 7220 636f 6d70 6172 696e  ime for comparin
+0002dd70: 6720 7661 6c75 6573 0a20 2020 2063 6875  g values.    chu
+0002dd80: 6e6b 7320 3d20 7b7d 0a20 2020 2063 7572  nks = {}.    cur
+0002dd90: 7265 6e74 5f73 7461 7274 5f6d 6173 6b20  rent_start_mask 
+0002dda0: 3d20 6e70 2e6f 6e65 7328 6c65 6e28 6466  = np.ones(len(df
+0002ddb0: 2e69 6e64 6578 292c 2064 7479 7065 203d  .index), dtype =
+0002ddc0: 2062 6f6f 6c29 2023 206c 656e 6774 6820   bool) # length 
+0002ddd0: 7265 6d61 696e 7320 7468 6520 7361 6d65  remains the same
+0002dde0: 0a20 2020 2066 6f72 2069 7620 696e 2069  .    for iv in i
+0002ddf0: 6e74 6572 7661 6c73 3a0a 2020 2020 2020  ntervals:.      
+0002de00: 2020 2320 6173 7375 6d65 7320 696e 7465    # assumes inte
+0002de10: 7276 616c 7320 6172 6520 6e6f 6e2d 6f76  rvals are non-ov
+0002de20: 6572 6c61 7070 696e 6720 616e 6420 6d6f  erlapping and mo
+0002de30: 6e6f 746f 6e69 6361 6c6c 7920 696e 6372  notonically incr
+0002de40: 6561 7369 6e67 0a20 2020 2020 2020 206c  easing.        l
+0002de50: 2c20 7220 3d20 6976 2e6c 6566 742c 2069  , r = iv.left, i
+0002de60: 762e 7269 6768 740a 2020 2020 2020 2020  v.right.        
+0002de70: 2320 6e65 7665 7220 6167 6169 6e20 6368  # never again ch
+0002de80: 6563 6b20 6576 656e 7473 2065 6e64 696e  eck events endin
+0002de90: 6720 6265 666f 7265 2074 6865 2063 7572  g before the cur
+0002dea0: 7265 6e74 2069 6e74 6572 7661 6c27 7320  rent interval's 
+0002deb0: 7374 6172 740a 2020 2020 2020 2020 6e6f  start.        no
+0002dec0: 745f 656e 6469 6e67 5f62 6566 6f72 655f  t_ending_before_
+0002ded0: 6c20 3d20 2872 6967 6874 7320 3e3d 206c  l = (rights >= l
+0002dee0: 290a 2020 2020 2020 2020 6c65 6674 7320  ).        lefts 
+0002def0: 3d20 6c65 6674 735b 6e6f 745f 656e 6469  = lefts[not_endi
+0002df00: 6e67 5f62 6566 6f72 655f 6c5d 0a20 2020  ng_before_l].   
+0002df10: 2020 2020 2072 6967 6874 7320 3d20 7269       rights = ri
+0002df20: 6768 7473 5b6e 6f74 5f65 6e64 696e 675f  ghts[not_ending_
+0002df30: 6265 666f 7265 5f6c 5d0a 2020 2020 2020  before_l].      
+0002df40: 2020 6375 7272 656e 745f 7374 6172 745f    current_start_
+0002df50: 6d61 736b 5b63 7572 7265 6e74 5f73 7461  mask[current_sta
+0002df60: 7274 5f6d 6173 6b5d 203d 206e 6f74 5f65  rt_mask] = not_e
+0002df70: 6e64 696e 675f 6265 666f 7265 5f6c 0a20  nding_before_l. 
+0002df80: 2020 2020 2020 2073 7461 7274 696e 675f         starting_
+0002df90: 6265 666f 7265 5f72 203d 2028 7220 3e20  before_r = (r > 
+0002dfa0: 6c65 6674 7329 0a20 2020 2020 2020 206e  lefts).        n
+0002dfb0: 6f74 5f65 6e64 696e 675f 6f6e 5f6c 5f65  ot_ending_on_l_e
+0002dfc0: 7863 6570 745f 656d 7074 7920 3d20 2872  xcept_empty = (r
+0002dfd0: 6967 6874 7320 213d 206c 2920 7c20 286c  ights != l) | (l
+0002dfe0: 6566 7473 203d 3d20 6c29 0a20 2020 2020  efts == l).     
+0002dff0: 2020 206f 7665 726c 6170 7069 6e67 203d     overlapping =
+0002e000: 2028 7374 6172 7469 6e67 5f62 6566 6f72   (starting_befor
+0002e010: 655f 7220 2620 6e6f 745f 656e 6469 6e67  e_r & not_ending
+0002e020: 5f6f 6e5f 6c5f 6578 6365 7074 5f65 6d70  _on_l_except_emp
+0002e030: 7479 290a 2020 2020 2020 2020 626f 6f6c  ty).        bool
+0002e040: 5f6d 6173 6b20 3d20 6375 7272 656e 745f  _mask = current_
+0002e050: 7374 6172 745f 6d61 736b 2e63 6f70 7928  start_mask.copy(
+0002e060: 290a 2020 2020 2020 2020 626f 6f6c 5f6d  ).        bool_m
+0002e070: 6173 6b5b 6375 7272 656e 745f 7374 6172  ask[current_star
+0002e080: 745f 6d61 736b 5d20 3d20 6f76 6572 6c61  t_mask] = overla
+0002e090: 7070 696e 670a 2020 2020 2020 2020 6368  pping.        ch
+0002e0a0: 756e 6b20 3d20 6466 5b62 6f6f 6c5f 6d61  unk = df[bool_ma
+0002e0b0: 736b 5d2e 636f 7079 2829 0a20 2020 2020  sk].copy().     
+0002e0c0: 2020 2069 6620 7472 756e 6361 7465 3a0a     if truncate:.
+0002e0d0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0002e0e0: 6c65 6674 732c 206e 6577 5f72 6967 6874  lefts, new_right
+0002e0f0: 7320 3d20 6c65 6674 735b 6f76 6572 6c61  s = lefts[overla
+0002e100: 7070 696e 675d 2c20 7269 6768 7473 5b6f  pping], rights[o
+0002e110: 7665 726c 6170 7069 6e67 5d0a 2020 2020  verlapping].    
+0002e120: 2020 2020 2020 2020 7374 6172 7469 6e67          starting
+0002e130: 5f62 6566 6f72 655f 6c2c 2065 6e64 696e  _before_l, endin
+0002e140: 675f 6166 7465 725f 7220 3d20 286e 6577  g_after_r = (new
+0002e150: 5f6c 6566 7473 203c 206c 292c 2028 6e65  _lefts < l), (ne
+0002e160: 775f 7269 6768 7473 203e 2072 290a 2020  w_rights > r).  
+0002e170: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
+0002e180: 7274 696e 675f 6265 666f 7265 5f6c 2e73  rting_before_l.s
+0002e190: 756d 2829 203e 2030 206f 7220 656e 6469  um() > 0 or endi
+0002e1a0: 6e67 5f61 6674 6572 5f72 2e73 756d 2829  ng_after_r.sum()
+0002e1b0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+0002e1c0: 2020 2020 2020 6e65 775f 6c65 6674 735b        new_lefts[
+0002e1d0: 7374 6172 7469 6e67 5f62 6566 6f72 655f  starting_before_
+0002e1e0: 6c5d 203d 206c 0a20 2020 2020 2020 2020  l] = l.         
+0002e1f0: 2020 2020 2020 206e 6577 5f72 6967 6874         new_right
+0002e200: 735b 656e 6469 6e67 5f61 6674 6572 5f72  s[ending_after_r
+0002e210: 5d20 3d20 720a 2020 2020 2020 2020 2020  ] = r.          
+0002e220: 2020 2020 2020 6368 756e 6b2e 696e 6465        chunk.inde
+0002e230: 7820 3d20 7064 2e49 6e74 6572 7661 6c49  x = pd.IntervalI
+0002e240: 6e64 6578 2e66 726f 6d5f 6172 7261 7973  ndex.from_arrays
+0002e250: 286e 6577 5f6c 6566 7473 2c20 6e65 775f  (new_lefts, new_
+0002e260: 7269 6768 7473 2c20 636c 6f73 6564 3d27  rights, closed='
+0002e270: 6c65 6674 2729 0a20 2020 2020 2020 2020  left').         
+0002e280: 2020 2020 2020 2063 6875 6e6b 2e64 7572         chunk.dur
+0002e290: 6174 696f 6e5f 7162 203d 2028 6e65 775f  ation_qb = (new_
+0002e2a0: 7269 6768 7473 202d 206e 6577 5f6c 6566  rights - new_lef
+0002e2b0: 7473 290a 2020 2020 2020 2020 2020 2020  ts).            
+0002e2c0: 2020 2020 6368 756e 6b2e 7175 6172 7465      chunk.quarte
+0002e2d0: 7262 6561 7473 203d 206e 6577 5f6c 6566  rbeats = new_lef
+0002e2e0: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+0002e2f0: 2020 2063 6875 6e6b 2e73 6f72 745f 7661     chunk.sort_va
+0002e300: 6c75 6573 285b 2771 7561 7274 6572 6265  lues(['quarterbe
+0002e310: 6174 7327 2c20 2764 7572 6174 696f 6e5f  ats', 'duration_
+0002e320: 7162 275d 2c20 696e 706c 6163 653d 5472  qb'], inplace=Tr
+0002e330: 7565 290a 2020 2020 2020 2020 6368 756e  ue).        chun
+0002e340: 6b73 5b69 765d 203d 2063 6875 6e6b 0a20  ks[iv] = chunk. 
+0002e350: 2020 2072 6574 7572 6e20 6368 756e 6b73     return chunks
+0002e360: 0a0a 0a64 6566 2069 6e66 6572 5f74 7376  ...def infer_tsv
+0002e370: 5f74 7970 6528 6466 3a20 7064 2e44 6174  _type(df: pd.Dat
+0002e380: 6146 7261 6d65 2920 2d3e 204f 7074 696f  aFrame) -> Optio
+0002e390: 6e61 6c5b 7374 725d 3a0a 2020 2020 2222  nal[str]:.    ""
+0002e3a0: 2249 6e66 6572 7320 7468 6520 636f 6e74  "Infers the cont
+0002e3b0: 656e 7473 206f 6620 6120 4461 7461 4672  ents of a DataFr
+0002e3c0: 616d 6520 6672 6f6d 2074 6865 2070 7265  ame from the pre
+0002e3d0: 7365 6e63 6520 6f66 2070 6172 7469 6375  sence of particu
+0002e3e0: 6c61 7220 636f 6c75 6d6e 732e 2222 220a  lar columns.""".
+0002e3f0: 2020 2020 7479 7065 3263 6f6c 7320 3d20      type2cols = 
+0002e400: 7b0a 2020 2020 2020 2020 276e 6f74 6573  {.        'notes
+0002e410: 273a 205b 2774 7063 272c 2027 6d69 6469  ': ['tpc', 'midi
+0002e420: 275d 2c0a 2020 2020 2020 2020 2765 7665  '],.        'eve
+0002e430: 6e74 7327 3a20 5b27 4368 6f72 642f 6475  nts': ['Chord/du
+0002e440: 7261 7469 6f6e 5479 7065 272c 2027 5265  rationType', 'Re
+0002e450: 7374 2f64 7572 6174 696f 6e54 7970 6527  st/durationType'
+0002e460: 5d2c 0a20 2020 2020 2020 2027 6368 6f72  ],.        'chor
+0002e470: 6473 273a 205b 2763 686f 7264 5f69 6427  ds': ['chord_id'
+0002e480: 5d2c 0a20 2020 2020 2020 2027 7265 7374  ],.        'rest
+0002e490: 7327 3a20 5b27 6e6f 6d69 6e61 6c5f 6475  s': ['nominal_du
+0002e4a0: 7261 7469 6f6e 275d 2c0a 2020 2020 2020  ration'],.      
+0002e4b0: 2020 2765 7870 616e 6465 6427 3a20 5b27    'expanded': ['
+0002e4c0: 6e75 6d65 7261 6c27 5d2c 0a20 2020 2020  numeral'],.     
+0002e4d0: 2020 2027 6c61 6265 6c73 273a 205b 2768     'labels': ['h
+0002e4e0: 6172 6d6f 6e79 5f6c 6179 6572 272c 2027  armony_layer', '
+0002e4f0: 6c61 6265 6c27 2c20 276c 6162 656c 5f74  label', 'label_t
+0002e500: 7970 6527 5d2c 0a20 2020 2020 2020 2027  ype'],.        '
+0002e510: 6d65 6173 7572 6573 273a 205b 2761 6374  measures': ['act
+0002e520: 5f64 7572 275d 2c0a 2020 2020 2020 2020  _dur'],.        
+0002e530: 2763 6164 656e 6365 7327 3a20 5b27 6361  'cadences': ['ca
+0002e540: 6465 6e63 6527 5d2c 0a20 2020 2020 2020  dence'],.       
+0002e550: 2027 6d65 7461 6461 7461 273a 205b 2766   'metadata': ['f
+0002e560: 6e61 6d65 275d 2c0a 2020 2020 2020 2020  name'],.        
+0002e570: 2766 6f72 6d5f 6c61 6265 6c73 273a 205b  'form_labels': [
+0002e580: 2766 6f72 6d5f 6c61 6265 6c27 2c20 2761  'form_label', 'a
+0002e590: 275d 2c0a 2020 2020 7d0a 2020 2020 666f  '],.    }.    fo
+0002e5a0: 7220 742c 2063 6f6c 756d 6e73 2069 6e20  r t, columns in 
+0002e5b0: 7479 7065 3263 6f6c 732e 6974 656d 7328  type2cols.items(
+0002e5c0: 293a 0a20 2020 2020 2020 2069 6620 616e  ):.        if an
+0002e5d0: 7928 6320 696e 2064 662e 636f 6c75 6d6e  y(c in df.column
+0002e5e0: 7320 666f 7220 6320 696e 2063 6f6c 756d  s for c in colum
+0002e5f0: 6e73 293a 0a20 2020 2020 2020 2020 2020  ns):.           
+0002e600: 2072 6574 7572 6e20 740a 2020 2020 6966   return t.    if
+0002e610: 2061 6e79 2863 2069 6e20 6466 2e63 6f6c   any(c in df.col
+0002e620: 756d 6e73 2066 6f72 2063 2069 6e20 5b27  umns for c in ['
+0002e630: 6d63 272c 2027 6d6e 275d 293a 0a20 2020  mc', 'mn']):.   
+0002e640: 2020 2020 2072 6574 7572 6e20 276c 6162       return 'lab
+0002e650: 656c 7327 0a20 2020 2072 6574 7572 6e20  els'.    return 
+0002e660: 2775 6e6b 6e6f 776e 270a 0a0a 6465 6620  'unknown'...def 
+0002e670: 7265 6475 6365 5f64 6174 6166 7261 6d65  reduce_dataframe
+0002e680: 5f64 7572 6174 696f 6e5f 746f 5f66 6972  _duration_to_fir
+0002e690: 7374 5f72 6f77 2864 663a 2070 642e 4461  st_row(df: pd.Da
+0002e6a0: 7461 4672 616d 6529 202d 3e20 7064 2e44  taFrame) -> pd.D
+0002e6b0: 6174 6146 7261 6d65 3a0a 2020 2020 2222  ataFrame:.    ""
+0002e6c0: 2220 5265 6475 6365 7320 6120 4461 7461  " Reduces a Data
+0002e6d0: 4672 616d 6520 746f 2069 7473 2072 6f77  Frame to its row
+0002e6e0: 2061 6e64 2075 7064 6174 6573 2074 6865   and updates the
+0002e6f0: 2064 7572 6174 696f 6e5f 7162 2063 6f6c   duration_qb col
+0002e700: 756d 6e20 746f 2072 6566 6c65 6374 2074  umn to reflect t
+0002e710: 6865 2072 6564 7563 6564 2064 7572 6174  he reduced durat
+0002e720: 696f 6e2e 0a0a 2020 2020 4172 6773 3a0a  ion...    Args:.
+0002e730: 2020 2020 2020 6466 3a20 4461 7461 6672        df: Datafr
+0002e740: 616d 6520 6f66 2077 6869 6368 2074 6f20  ame of which to 
+0002e750: 6b65 6570 206f 6e6c 7920 7468 6520 6669  keep only the fi
+0002e760: 7273 7420 726f 772e 2049 6620 6974 2068  rst row. If it h
+0002e770: 6173 2061 6e20 496e 7465 7276 616c 496e  as an IntervalIn
+0002e780: 6465 782c 2074 6865 2069 6e74 6572 7661  dex, the interva
+0002e790: 6c20 6973 2075 7064 6174 6564 2074 6f0a  l is updated to.
+0002e7a0: 2020 2020 2020 2020 2020 7265 666c 6563            reflec
+0002e7b0: 7420 7468 6520 7768 6f6c 6520 6475 7261  t the whole dura
+0002e7c0: 7469 6f6e 2e0a 0a20 2020 2052 6574 7572  tion...    Retur
+0002e7d0: 6e73 3a0a 2020 2020 2020 4461 7461 4672  ns:.      DataFr
+0002e7e0: 616d 6520 7769 7468 206f 6e65 2072 6f77  ame with one row
+0002e7f0: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
+0002e800: 206c 656e 2864 6629 203d 3d20 313a 0a20   len(df) == 1:. 
+0002e810: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+0002e820: 0a20 2020 2069 6478 203d 2064 662e 696e  .    idx = df.in
+0002e830: 6465 780a 2020 2020 6669 7273 745f 6c6f  dex.    first_lo
+0002e840: 6320 3d20 6964 785b 305d 0a20 2020 2072  c = idx[0].    r
+0002e850: 6f77 203d 2064 662e 696c 6f63 5b5b 305d  ow = df.iloc[[0]
+0002e860: 5d0a 2020 2020 2320 6966 2069 7369 6e73  ].    # if isins
+0002e870: 7461 6e63 6528 6978 2c20 7064 2e49 6e74  tance(ix, pd.Int
+0002e880: 6572 7661 6c29 206f 7220 2869 7369 6e73  erval) or (isins
+0002e890: 7461 6e63 6528 6978 2c20 7475 706c 6529  tance(ix, tuple)
+0002e8a0: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
+0002e8b0: 6978 5b2d 315d 2c20 7064 2e49 6e74 6572  ix[-1], pd.Inter
+0002e8c0: 7661 6c29 293a 0a20 2020 2069 6620 6973  val)):.    if is
+0002e8d0: 696e 7374 616e 6365 2869 6478 2c20 7064  instance(idx, pd
+0002e8e0: 2e49 6e74 6572 7661 6c49 6e64 6578 293a  .IntervalIndex):
+0002e8f0: 0a20 2020 2020 2020 2073 7461 7274 203d  .        start =
+0002e900: 206d 696e 2869 6478 2e6c 6566 7429 0a20   min(idx.left). 
+0002e910: 2020 2020 2020 2065 6e64 203d 206d 6178         end = max
+0002e920: 2869 6478 2e72 6967 6874 290a 2020 2020  (idx.right).    
+0002e930: 2020 2020 6976 203d 2070 642e 496e 7465      iv = pd.Inte
+0002e940: 7276 616c 2873 7461 7274 2c20 656e 642c  rval(start, end,
+0002e950: 2063 6c6f 7365 643d 6964 782e 636c 6f73   closed=idx.clos
+0002e960: 6564 290a 2020 2020 2020 2020 726f 772e  ed).        row.
+0002e970: 696e 6465 7820 3d20 7064 2e49 6e74 6572  index = pd.Inter
+0002e980: 7661 6c49 6e64 6578 285b 6976 5d29 0a20  valIndex([iv]). 
+0002e990: 2020 2020 2020 2072 6f77 2e6c 6f63 5b69         row.loc[i
+0002e9a0: 762c 2027 6475 7261 7469 6f6e 5f71 6227  v, 'duration_qb'
+0002e9b0: 5d20 3d20 6976 2e6c 656e 6774 680a 2020  ] = iv.length.  
+0002e9c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002e9d0: 6e65 775f 6475 7261 7469 6f6e 203d 2064  new_duration = d
+0002e9e0: 662e 6475 7261 7469 6f6e 5f71 622e 7375  f.duration_qb.su
+0002e9f0: 6d28 290a 2020 2020 2020 2020 726f 772e  m().        row.
+0002ea00: 6c6f 635b 6669 7273 745f 6c6f 632c 2027  loc[first_loc, '
+0002ea10: 6475 7261 7469 6f6e 5f71 6227 5d20 3d20  duration_qb'] = 
+0002ea20: 6e65 775f 6475 7261 7469 6f6e 0a20 2020  new_duration.   
+0002ea30: 2072 6574 7572 6e20 726f 770a 0a0a 4064   return row...@d
+0002ea40: 6174 6163 6c61 7373 0a63 6c61 7373 2046  ataclass.class F
+0002ea50: 696c 653a 0a20 2020 2022 2222 5374 6f72  ile:.    """Stor
+0002ea60: 696e 6720 7061 7468 2061 6e64 2066 696c  ing path and fil
+0002ea70: 6520 6e61 6d65 2069 6e66 6f72 6d61 7469  e name informati
+0002ea80: 6f6e 2066 6f72 206f 6e65 2066 696c 652e  on for one file.
+0002ea90: 2222 220a 2020 2020 6978 3a20 696e 740a  """.    ix: int.
+0002eaa0: 2020 2020 2222 2249 6e64 6578 2069 6e74      """Index int
+0002eab0: 6567 6572 2028 4944 2922 2222 0a20 2020  eger (ID)""".   
+0002eac0: 2074 7970 653a 2073 7472 0a20 2020 2022   type: str.    "
+0002ead0: 2222 5265 636f 676e 697a 6564 2074 7970  ""Recognized typ
+0002eae0: 6520 e288 8820 3a61 7474 723a 606d 7333  e ... :attr:`ms3
+0002eaf0: 2e5f 7479 7069 6e67 2e46 6163 6574 6022  ._typing.Facet`"
+0002eb00: 2222 0a20 2020 2066 696c 653a 2073 7472  "".    file: str
+0002eb10: 0a20 2020 2022 2222 4669 6c65 206e 616d  .    """File nam
+0002eb20: 6520 696e 636c 7564 696e 6720 6578 7465  e including exte
+0002eb30: 6e73 696f 6e2e 2222 220a 2020 2020 666e  nsion.""".    fn
+0002eb40: 616d 653a 2073 7472 0a20 2020 2022 2222  ame: str.    """
+0002eb50: 666e 616d 6520 6578 636c 7564 696e 6720  fname excluding 
+0002eb60: 7468 6520 7375 6666 6978 2028 6166 7465  the suffix (afte
+0002eb70: 7220 7265 6769 7374 6572 696e 6720 7468  r registering th
+0002eb80: 6520 6669 6c65 2077 6974 6820 6120 3a6f  e file with a :o
+0002eb90: 626a 3a60 5069 6563 6560 292e 2222 220a  bj:`Piece`).""".
+0002eba0: 2020 2020 6665 7874 3a20 7374 720a 2020      fext: str.  
+0002ebb0: 2020 2222 2246 696c 6520 6578 7465 6e73    """File extens
+0002ebc0: 696f 6e73 2e22 2222 0a20 2020 2073 7562  ions.""".    sub
+0002ebd0: 6469 723a 2073 7472 0a20 2020 2022 2222  dir: str.    """
+0002ebe0: 4469 7265 6374 6f72 7920 7265 6c61 7469  Directory relati
+0002ebf0: 7665 2074 6f20 7468 6520 636f 7270 7573  ve to the corpus
+0002ec00: 2070 6174 6820 2865 2e67 2e20 272e 2f4d   path (e.g. './M
+0002ec10: 5333 2729 2e22 2222 0a20 2020 2063 6f72  S3').""".    cor
+0002ec20: 7075 735f 7061 7468 3a20 7374 720a 2020  pus_path: str.  
+0002ec30: 2020 2222 2241 6273 6f6c 7574 6520 7061    """Absolute pa
+0002ec40: 7468 206f 6620 7468 6520 6669 6c65 2773  th of the file's
+0002ec50: 2070 6172 656e 7420 6469 7265 6374 6f72   parent director
+0002ec60: 7920 7468 6174 2069 7320 636f 6e73 6964  y that is consid
+0002ec70: 6572 6564 2061 7320 636f 7270 7573 2064  ered as corpus d
+0002ec80: 6972 6563 746f 7279 2e22 2222 0a20 2020  irectory.""".   
+0002ec90: 2072 656c 5f70 6174 683a 2073 7472 0a20   rel_path: str. 
+0002eca0: 2020 2022 2222 4669 6c65 2070 6174 6820     """File path 
+0002ecb0: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
+0002ecc0: 636f 7270 7573 2070 6174 682e 2045 7175  corpus path. Equ
+0002ecd0: 6976 616c 656e 7420 746f 203c 7375 6264  ivalent to <subd
+0002ece0: 6972 3e2f 3c66 696c 653e 2e22 2222 0a20  ir>/<file>.""". 
+0002ecf0: 2020 2066 756c 6c5f 7061 7468 3a20 7374     full_path: st
+0002ed00: 720a 2020 2020 2222 2241 6273 6f6c 7574  r.    """Absolut
+0002ed10: 6520 6669 6c65 2070 6174 682e 2222 220a  e file path.""".
+0002ed20: 2020 2020 6469 7265 6374 6f72 793a 2073      directory: s
+0002ed30: 7472 0a20 2020 2022 2222 4162 736f 6c75  tr.    """Absolu
+0002ed40: 7465 2066 6f6c 6465 7220 7061 7468 2077  te folder path w
+0002ed50: 6865 7265 2074 6865 2066 696c 6520 6973  here the file is
+0002ed60: 206c 6f63 6174 6564 2e22 2222 0a20 2020   located.""".   
+0002ed70: 2073 7566 6669 783a 2073 7472 203d 2027   suffix: str = '
+0002ed80: 270a 2020 2020 2222 2255 706f 6e20 7265  '.    """Upon re
+0002ed90: 6769 7374 6572 696e 6720 7468 6520 4669  gistering the Fi
+0002eda0: 6c65 2077 6974 6820 6120 3a6f 626a 3a60  le with a :obj:`
+0002edb0: 5069 6563 6560 2c20 6966 2074 6865 2063  Piece`, if the c
+0002edc0: 7572 7265 6e74 2066 6e61 6d65 2068 6173  urrent fname has
+0002edd0: 2061 2073 7566 6669 7820 636f 6d70 6172   a suffix compar
+0002ede0: 6564 2074 6f20 7468 6520 5069 6563 6527  ed to the Piece'
+0002edf0: 7320 666e 616d 652c 200a 2020 2020 7375  s fname, .    su
+0002ee00: 6666 6978 2069 7320 7265 6d6f 7665 6420  ffix is removed 
+0002ee10: 6672 6f6d 2074 6865 2046 696c 6520 6f62  from the File ob
+0002ee20: 6a65 6374 2773 2066 6e61 6d65 2066 6965  ject's fname fie
+0002ee30: 6c64 2061 6e64 2061 6464 6564 2074 6f20  ld and added to 
+0002ee40: 7468 6520 7375 6666 6978 2066 6965 6c64  the suffix field
+0002ee50: 2e22 2222 0a20 2020 2063 6f6d 6d69 745f  .""".    commit_
+0002ee60: 7368 613a 2073 7472 203d 2027 270a 2020  sha: str = ''.  
+0002ee70: 2020 2222 2254 6865 2074 6865 2066 696c    """The the fil
+0002ee80: 6520 6861 7320 6265 656e 2072 6574 7269  e has been retri
+0002ee90: 6576 6564 2066 726f 6d20 6120 7061 7274  eved from a part
+0002eea0: 6963 756c 6172 2067 6974 2072 6576 6973  icular git revis
+0002eeb0: 696f 6e2c 2074 6869 7320 6973 2073 6574  ion, this is set
+0002eec0: 2074 6f20 7468 6520 7265 7669 7369 6f6e   to the revision
+0002eed0: 2773 2068 6173 682e 2222 220a 0a20 2020  's hash."""..   
+0002eee0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+0002eef0: 6c66 293a 0a20 2020 2020 2020 2073 7566  lf):.        suf
+0002ef00: 6669 7820 3d20 2727 2069 6620 7365 6c66  fix = '' if self
+0002ef10: 2e73 7566 6669 7820 3d3d 2027 2720 656c  .suffix == '' el
+0002ef20: 7365 2066 222c 2073 7566 6669 783a 207b  se f", suffix: {
+0002ef30: 7365 6c66 2e73 7566 6669 787d 2e22 0a20  self.suffix}.". 
+0002ef40: 2020 2020 2020 2063 6f6d 6d69 7420 3d20         commit = 
+0002ef50: 2727 2069 6620 7365 6c66 2e63 6f6d 6d69  '' if self.commi
+0002ef60: 745f 7368 6120 3d3d 2027 2720 656c 7365  t_sha == '' else
+0002ef70: 2066 2240 7b73 656c 662e 636f 6d6d 6974   f"@{self.commit
+0002ef80: 5f73 6861 5b3a 375d 7d22 0a20 2020 2020  _sha[:7]}".     
+0002ef90: 2020 2072 6574 7572 6e20 6622 7b73 656c     return f"{sel
+0002efa0: 662e 6978 7d3a 2027 7b73 656c 662e 7265  f.ix}: '{self.re
+0002efb0: 6c5f 7061 7468 7d27 7b63 6f6d 6d69 747d  l_path}'{commit}
+0002efc0: 7b73 7566 6669 787d 220a 0a20 2020 2064  {suffix}"..    d
+0002efd0: 6566 2072 6570 6c61 6365 5f65 7874 656e  ef replace_exten
+0002efe0: 7369 6f6e 2873 656c 662c 206e 6577 5f65  sion(self, new_e
+0002eff0: 7874 656e 7369 6f6e 3a20 7374 722c 202a  xtension: str, *
+0002f000: 2a6b 7761 7267 7329 202d 3e20 5365 6c66  *kwargs) -> Self
+0002f010: 3a0a 2020 2020 2020 2020 6966 206e 6577  :.        if new
+0002f020: 5f65 7874 656e 7369 6f6e 5b30 5d20 213d  _extension[0] !=
+0002f030: 2027 2e27 3a0a 2020 2020 2020 2020 2020   '.':.          
+0002f040: 2020 6e65 775f 6578 7465 6e73 696f 6e20    new_extension 
+0002f050: 3d20 272e 2720 2b20 6e65 775f 6578 7465  = '.' + new_exte
+0002f060: 6e73 696f 6e0a 2020 2020 2020 2020 6f6c  nsion.        ol
+0002f070: 645f 6578 745f 6c65 6e20 3d20 6c65 6e28  d_ext_len = len(
+0002f080: 7365 6c66 2e66 6578 7429 0a20 2020 2020  self.fext).     
+0002f090: 2020 206e 6577 5f76 616c 7320 3d20 7b7d     new_vals = {}
+0002f0a0: 0a20 2020 2020 2020 2066 6f72 2066 6965  .        for fie
+0002f0b0: 6c64 2069 6e20 2822 6669 6c65 222c 2022  ld in ("file", "
+0002f0c0: 6665 7874 222c 2022 7265 6c5f 7061 7468  fext", "rel_path
+0002f0d0: 222c 2022 6675 6c6c 5f70 6174 6822 293a  ", "full_path"):
+0002f0e0: 0a20 2020 2020 2020 2020 2020 206f 6c64  .            old
+0002f0f0: 5f76 616c 203d 2067 6574 6174 7472 2873  _val = getattr(s
+0002f100: 656c 662c 2066 6965 6c64 290a 2020 2020  elf, field).    
+0002f110: 2020 2020 2020 2020 6e65 775f 7661 6c73          new_vals
+0002f120: 5b66 6965 6c64 5d20 3d20 6f6c 645f 7661  [field] = old_va
+0002f130: 6c5b 3a2d 6f6c 645f 6578 745f 6c65 6e5d  l[:-old_ext_len]
+0002f140: 202b 206e 6577 5f65 7874 656e 7369 6f6e   + new_extension
+0002f150: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002f160: 7265 706c 6163 6528 7365 6c66 2c20 2a2a  replace(self, **
+0002f170: 6e65 775f 7661 6c73 2c20 2a2a 6b77 6172  new_vals, **kwar
+0002f180: 6773 290a 0a0a 2020 2020 4063 6c61 7373  gs)...    @class
+0002f190: 6d65 7468 6f64 0a20 2020 2064 6566 2066  method.    def f
+0002f1a0: 726f 6d5f 636f 7270 7573 5f70 6174 6828  rom_corpus_path(
+0002f1b0: 636c 732c 0a20 2020 2020 2020 2020 2020  cls,.           
+0002f1c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0002f1d0: 7270 7573 5f70 6174 683a 2073 7472 2c0a  rpus_path: str,.
+0002f1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f1f0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+0002f200: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+0002f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f220: 2066 7479 7065 3a20 4f70 7469 6f6e 616c   ftype: Optional
+0002f230: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0002f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f250: 2020 2020 2020 2073 7562 6469 723d 272e         subdir='.
+0002f260: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0002f270: 2020 2020 2020 2020 2020 2020 6978 3a20              ix: 
+0002f280: 696e 7420 3d20 2d31 293a 0a20 2020 2020  int = -1):.     
+0002f290: 2020 2022 2222 2043 7265 6174 6573 2046     """ Creates F
+0002f2a0: 696c 6520 6f62 6a65 6374 2066 726f 6d20  ile object from 
+0002f2b0: 696e 6469 7669 6475 616c 2063 6f6d 706f  individual compo
+0002f2c0: 6e65 6e74 730a 0a20 2020 2020 2020 2041  nents..        A
+0002f2d0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0002f2e0: 2063 6f72 7075 735f 7061 7468 3a20 526f   corpus_path: Ro
+0002f2f0: 6f74 2064 6972 6563 746f 7279 206f 6620  ot directory of 
+0002f300: 7468 6520 6669 6c65 2773 2063 6f72 7075  the file's corpu
+0002f310: 732e 0a20 2020 2020 2020 2020 2020 2066  s..            f
+0002f320: 696c 656e 616d 653a 2046 756c 6c20 6669  ilename: Full fi
+0002f330: 6c65 206e 616d 6520 696e 636c 7564 696e  le name includin
+0002f340: 6720 7375 6666 6978 6573 2061 6e64 2065  g suffixes and e
+0002f350: 7874 656e 7369 6f6e 732e 0a20 2020 2020  xtensions..     
+0002f360: 2020 2020 2020 2066 7479 7065 3a20 4669         ftype: Fi
+0002f370: 6c65 2074 7970 6520 2875 7365 6420 6173  le type (used as
+0002f380: 2064 6566 6175 6c74 2066 6f6c 6465 7220   default folder 
+0002f390: 6e61 6d65 2066 6f72 2063 7265 6174 696e  name for creatin
+0002f3a0: 6720 6669 6c65 5f70 6174 6873 292e 0a20  g file_paths).. 
+0002f3b0: 2020 2020 2020 2020 2020 2073 7562 6469             subdi
+0002f3c0: 723a 2072 656c 6174 6976 6520 6469 7265  r: relative dire
+0002f3d0: 6374 6f72 7920 6170 7065 6e64 6564 2074  ctory appended t
+0002f3e0: 6f20 636f 7270 7573 5f70 6174 682c 2064  o corpus_path, d
+0002f3f0: 6566 6175 6c74 7320 746f 2027 2e27 2c20  efaults to '.', 
+0002f400: 692e 652e 206e 6f20 7375 6266 6f6c 6465  i.e. no subfolde
+0002f410: 722e 0a20 2020 2020 2020 2020 2020 2069  r..            i
+0002f420: 783a 2041 7262 6974 7261 7279 2069 6e64  x: Arbitrary ind
+0002f430: 6578 206e 756d 6265 722c 2064 6566 6175  ex number, defau
+0002f440: 6c74 7320 746f 202d 312e 0a20 2020 2020  lts to -1..     
+0002f450: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+0002f460: 756c 6c5f 7061 7468 203d 206f 732e 7061  ull_path = os.pa
+0002f470: 7468 2e72 6561 6c70 6174 6828 6f73 2e70  th.realpath(os.p
+0002f480: 6174 682e 6a6f 696e 2863 6f72 7075 735f  ath.join(corpus_
+0002f490: 7061 7468 2c20 7375 6264 6972 2c20 6669  path, subdir, fi
+0002f4a0: 6c65 6e61 6d65 2929 0a20 2020 2020 2020  lename)).       
+0002f4b0: 2066 696c 655f 6e61 6d65 2c20 6669 6c65   file_name, file
+0002f4c0: 5f65 7874 203d 206f 732e 7061 7468 2e73  _ext = os.path.s
+0002f4d0: 706c 6974 6578 7428 6669 6c65 6e61 6d65  plitext(filename
+0002f4e0: 290a 2020 2020 2020 2020 7265 6c5f 7061  ).        rel_pa
+0002f4f0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+0002f500: 6e28 7375 6264 6972 2c20 6669 6c65 6e61  n(subdir, filena
+0002f510: 6d65 290a 2020 2020 2020 2020 6966 2066  me).        if f
+0002f520: 7479 7065 2069 7320 4e6f 6e65 3a0a 2020  type is None:.  
+0002f530: 2020 2020 2020 2020 2020 6669 6c65 5f74            file_t
+0002f540: 7970 6520 3d20 7061 7468 3274 7970 6528  ype = path2type(
+0002f550: 6675 6c6c 5f70 6174 682c 206c 6f67 6765  full_path, logge
+0002f560: 723d 7365 6c66 2e6c 6f67 6765 7229 0a20  r=self.logger). 
+0002f570: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0002f580: 2020 2020 2020 2020 2066 696c 655f 7479           file_ty
+0002f590: 7065 203d 2066 7479 7065 0a20 2020 2020  pe = ftype.     
+0002f5a0: 2020 2072 6574 7572 6e20 636c 7328 0a20     return cls(. 
+0002f5b0: 2020 2020 2020 2020 2020 2069 783d 6978             ix=ix
+0002f5c0: 2c0a 2020 2020 2020 2020 2020 2020 7479  ,.            ty
+0002f5d0: 7065 3d66 696c 655f 7479 7065 2c0a 2020  pe=file_type,.  
+0002f5e0: 2020 2020 2020 2020 2020 6669 6c65 3d66            file=f
+0002f5f0: 696c 656e 616d 652c 0a20 2020 2020 2020  ilename,.       
+0002f600: 2020 2020 2066 6e61 6d65 3d66 696c 655f       fname=file_
+0002f610: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+0002f620: 2020 6665 7874 3d66 696c 655f 6578 742c    fext=file_ext,
+0002f630: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
+0002f640: 6469 723d 7375 6264 6972 2c0a 2020 2020  dir=subdir,.    
+0002f650: 2020 2020 2020 2020 636f 7270 7573 5f70          corpus_p
+0002f660: 6174 683d 636f 7270 7573 5f70 6174 682c  ath=corpus_path,
+0002f670: 0a20 2020 2020 2020 2020 2020 2072 656c  .            rel
+0002f680: 5f70 6174 683d 7265 6c5f 7061 7468 2c0a  _path=rel_path,.
+0002f690: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
+0002f6a0: 5f70 6174 683d 6675 6c6c 5f70 6174 682c  _path=full_path,
+0002f6b0: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
+0002f6c0: 6563 746f 7279 3d6f 732e 7061 7468 2e64  ectory=os.path.d
+0002f6d0: 6972 6e61 6d65 2866 756c 6c5f 7061 7468  irname(full_path
+0002f6e0: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
+0002f6f0: 7566 6669 783d 2727 2c0a 2020 2020 2020  uffix='',.      
+0002f700: 2020 290a 0a40 6675 6e63 7469 6f6e 5f6c    )..@function_l
+0002f710: 6f67 6765 720a 6465 6620 6175 746f 6d61  ogger.def automa
+0002f720: 7469 6361 6c6c 795f 6368 6f6f 7365 5f66  tically_choose_f
+0002f730: 726f 6d5f 6469 7361 6d62 6967 7561 7465  rom_disambiguate
+0002f740: 645f 6669 6c65 7328 6469 7361 6d62 6967  d_files(disambig
+0002f750: 7561 7465 645f 6368 6f69 6365 733a 2044  uated_choices: D
+0002f760: 6963 745b 7374 722c 2046 696c 655d 2c0a  ict[str, File],.
 0002f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f790: 2020 2020 2020 2066 696c 655f 7479 7065         file_type
-0002f7a0: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
+0002f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f7a0: 2020 666e 616d 653a 2073 7472 2c0a 2020    fname: str,.  
 0002f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0002f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f7d0: 2020 2020 2020 2020 2029 202d 3e20 4669           ) -> Fi
-0002f7e0: 6c65 3a0a 2020 2020 6966 206c 656e 2864  le:.    if len(d
-0002f7f0: 6973 616d 6269 6775 6174 6564 5f63 686f  isambiguated_cho
-0002f800: 6963 6573 2920 3d3d 2031 3a0a 2020 2020  ices) == 1:.    
-0002f810: 2020 2020 7265 7475 726e 206c 6973 7428      return list(
-0002f820: 6469 7361 6d62 6967 7561 7465 645f 6368  disambiguated_ch
-0002f830: 6f69 6365 732e 6b65 7973 2829 295b 305d  oices.keys())[0]
-0002f840: 0a20 2020 2064 6973 616d 625f 7365 7269  .    disamb_seri
-0002f850: 6573 203d 2070 642e 5365 7269 6573 2864  es = pd.Series(d
-0002f860: 6973 616d 6269 6775 6174 6564 5f63 686f  isambiguated_cho
-0002f870: 6963 6573 290a 2020 2020 6669 6c65 7320  ices).    files 
-0002f880: 3d20 6c69 7374 2864 6973 616d 6269 6775  = list(disambigu
-0002f890: 6174 6564 5f63 686f 6963 6573 2e76 616c  ated_choices.val
-0002f8a0: 7565 7328 2929 0a20 2020 2066 696c 6573  ues()).    files
-0002f8b0: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
-0002f8c0: 6d65 2866 696c 6573 2c20 696e 6465 783d  me(files, index=
-0002f8d0: 6469 7361 6d62 5f73 6572 6965 732e 696e  disamb_series.in
-0002f8e0: 6465 7829 0a20 2020 2063 686f 6963 655f  dex).    choice_
-0002f8f0: 6265 7477 6565 6e5f 6e20 3d20 6c65 6e28  between_n = len(
-0002f900: 6669 6c65 7329 0a20 2020 2069 6620 6669  files).    if fi
-0002f910: 6c65 5f74 7970 6520 3d3d 2027 7363 6f72  le_type == 'scor
-0002f920: 6573 273a 0a20 2020 2020 2020 2023 2069  es':.        # i
-0002f930: 6620 6120 7363 6f72 6520 6973 2072 6571  f a score is req
-0002f940: 7565 7374 6564 2c20 6368 6563 6b20 6966  uested, check if
-0002f950: 2074 6865 7265 2069 7320 6f6e 6c79 2061   there is only a
-0002f960: 2073 696e 676c 6520 4d53 4358 206f 7220   single MSCX or 
-0002f970: 6f74 6865 7277 6973 6520 4d53 435a 2066  otherwise MSCZ f
-0002f980: 696c 6520 616e 6420 7069 636b 2074 6861  ile and pick tha
-0002f990: 740a 2020 2020 2020 2020 6665 7874 7320  t.        fexts 
-0002f9a0: 3d20 6669 6c65 735f 6466 2e66 6578 742e  = files_df.fext.
-0002f9b0: 7374 722e 6c6f 7765 7228 290a 2020 2020  str.lower().    
-0002f9c0: 2020 2020 6665 7874 5f63 6f75 6e74 7320      fext_counts 
-0002f9d0: 3d20 6665 7874 732e 7661 6c75 655f 636f  = fexts.value_co
-0002f9e0: 756e 7473 2829 0a20 2020 2020 2020 2069  unts().        i
-0002f9f0: 6620 272e 6d73 6378 2720 696e 2066 6578  f '.mscx' in fex
-0002fa00: 745f 636f 756e 7473 3a0a 2020 2020 2020  t_counts:.      
-0002fa10: 2020 2020 2020 6966 2066 6578 745f 636f        if fext_co
-0002fa20: 756e 7473 5b27 2e6d 7363 7827 5d20 3d3d  unts['.mscx'] ==
-0002fa30: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0002fa40: 2020 2020 7365 6c65 6374 6564 5f66 696c      selected_fil
-0002fa50: 6520 3d20 6469 7361 6d62 5f73 6572 6965  e = disamb_serie
-0002fa60: 735b 6665 7874 7320 3d3d 2027 2e6d 7363  s[fexts == '.msc
-0002fa70: 7827 5d2e 696c 6f63 5b30 5d0a 2020 2020  x'].iloc[0].    
-0002fa80: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0002fa90: 6572 2e64 6562 7567 2866 2249 6e20 6f72  er.debug(f"In or
-0002faa0: 6465 7220 746f 2070 6963 6b20 6f6e 6520  der to pick one 
-0002fab0: 6672 6f6d 2074 6865 207b 6368 6f69 6365  from the {choice
-0002fac0: 5f62 6574 7765 656e 5f6e 7d20 7363 6f72  _between_n} scor
-0002fad0: 6573 2077 6974 6820 666e 616d 6520 277b  es with fname '{
-0002fae0: 666e 616d 657d 272c 2027 7b73 656c 6563  fname}', '{selec
-0002faf0: 7465 645f 6669 6c65 2e72 656c 5f70 6174  ted_file.rel_pat
-0002fb00: 687d 2720 7761 7320 7365 6c65 6374 6564  h}' was selected
-0002fb10: 2062 6563 6175 7365 2069 7420 6973 2074   because it is t
-0002fb20: 6865 206f 6e6c 7920 220a 2020 2020 2020  he only ".      
-0002fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fb40: 2020 2020 2020 2020 2020 2066 226f 6e65             f"one
-0002fb50: 2069 6e20 4d53 4358 2066 6f72 6d61 742e   in MSCX format.
-0002fb60: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0002fb70: 2020 2072 6574 7572 6e20 7365 6c65 6374     return select
-0002fb80: 6564 5f66 696c 650a 2020 2020 2020 2020  ed_file.        
-0002fb90: 656c 6966 2027 2e6d 7363 7a27 2069 6e20  elif '.mscz' in 
-0002fba0: 6665 7874 5f63 6f75 6e74 7320 616e 6420  fext_counts and 
-0002fbb0: 6665 7874 5f63 6f75 6e74 735b 272e 6d73  fext_counts['.ms
-0002fbc0: 637a 275d 203d 3d20 313a 0a20 2020 2020  cz'] == 1:.     
-0002fbd0: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-0002fbe0: 6669 6c65 203d 2064 6973 616d 625f 7365  file = disamb_se
-0002fbf0: 7269 6573 5b66 6578 7473 203d 3d20 272e  ries[fexts == '.
-0002fc00: 6d73 637a 275d 2e69 6c6f 635b 305d 0a20  mscz'].iloc[0]. 
-0002fc10: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0002fc20: 722e 6465 6275 6728 6622 496e 206f 7264  r.debug(f"In ord
-0002fc30: 6572 2074 6f20 7069 636b 206f 6e65 2066  er to pick one f
-0002fc40: 726f 6d20 7468 6520 7b63 686f 6963 655f  rom the {choice_
-0002fc50: 6265 7477 6565 6e5f 6e7d 2073 636f 7265  between_n} score
-0002fc60: 7320 7769 7468 2066 6e61 6d65 2027 7b66  s with fname '{f
-0002fc70: 6e61 6d65 7d27 2c20 277b 7365 6c65 6374  name}', '{select
-0002fc80: 6564 5f66 696c 652e 7265 6c5f 7061 7468  ed_file.rel_path
-0002fc90: 7d27 2077 6173 2073 656c 6563 7465 6420  }' was selected 
-0002fca0: 6265 6361 7573 6520 6974 2069 7320 7468  because it is th
-0002fcb0: 6520 6f6e 6c79 2022 0a20 2020 2020 2020  e only ".       
-0002fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fcd0: 2020 2020 2020 6622 6f6e 6520 696e 204d        f"one in M
-0002fce0: 5343 5a20 666f 726d 6174 2e22 290a 2020  SCZ format.").  
-0002fcf0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002fd00: 2073 656c 6563 7465 645f 6669 6c65 0a20   selected_file. 
-0002fd10: 2020 2023 2061 7320 6669 7273 7420 6469     # as first di
-0002fd20: 7361 6d62 6967 7561 7469 6f6e 2063 7269  sambiguation cri
-0002fd30: 7465 7269 6f6e 2c20 6368 6563 6b20 6966  terion, check if
-0002fd40: 2074 6865 2073 686f 7274 6573 7420 6469   the shortest di
-0002fd50: 7361 6d62 6967 7561 7469 6f6e 2073 7472  sambiguation str
-0002fd60: 696e 6720 7065 7274 6169 6e73 2074 6f20  ing pertains to 
-0002fd70: 3120 6669 6c65 206f 6e6c 7920 616e 6420  1 file only and 
-0002fd80: 7069 636b 2074 6861 740a 2020 2020 6469  pick that.    di
-0002fd90: 7361 6d62 5f73 7472 5f6c 656e 6774 6873  samb_str_lengths
-0002fda0: 203d 2070 642e 5365 7269 6573 2864 6973   = pd.Series(dis
-0002fdb0: 616d 625f 7365 7269 6573 2e69 6e64 6578  amb_series.index
-0002fdc0: 2e6d 6170 286c 656e 292c 2069 6e64 6578  .map(len), index
-0002fdd0: 3d64 6973 616d 625f 7365 7269 6573 2e69  =disamb_series.i
-0002fde0: 6e64 6578 290a 2020 2020 7368 6f72 7465  ndex).    shorte
-0002fdf0: 7374 5f6c 656e 6774 685f 7365 6c65 6374  st_length_select
-0002fe00: 6f72 203d 2028 6469 7361 6d62 5f73 7472  or = (disamb_str
-0002fe10: 5f6c 656e 6774 6873 203d 3d20 6469 7361  _lengths == disa
-0002fe20: 6d62 5f73 7472 5f6c 656e 6774 6873 2e6d  mb_str_lengths.m
-0002fe30: 696e 2829 290a 2020 2020 6e5f 6861 7665  in()).    n_have
-0002fe40: 5f73 686f 7274 6573 745f 6c65 6e67 7468  _shortest_length
-0002fe50: 203d 2073 686f 7274 6573 745f 6c65 6e67   = shortest_leng
-0002fe60: 7468 5f73 656c 6563 746f 722e 7375 6d28  th_selector.sum(
-0002fe70: 290a 2020 2020 6966 206e 5f68 6176 655f  ).    if n_have_
-0002fe80: 7368 6f72 7465 7374 5f6c 656e 6774 6820  shortest_length 
-0002fe90: 3d3d 2031 3a0a 2020 2020 2020 2020 6978  == 1:.        ix
-0002fea0: 203d 2064 6973 616d 625f 7374 725f 6c65   = disamb_str_le
-0002feb0: 6e67 7468 732e 6964 786d 696e 2829 0a20  ngths.idxmin(). 
-0002fec0: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-0002fed0: 6669 6c65 203d 2064 6973 616d 625f 7365  file = disamb_se
-0002fee0: 7269 6573 2e6c 6f63 5b69 785d 0a20 2020  ries.loc[ix].   
-0002fef0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0002ff00: 6728 6622 496e 206f 7264 6572 2074 6f20  g(f"In order to 
-0002ff10: 7069 636b 206f 6e65 2066 726f 6d20 7468  pick one from th
-0002ff20: 6520 7b63 686f 6963 655f 6265 7477 6565  e {choice_betwee
-0002ff30: 6e5f 6e7d 2027 7b66 696c 655f 7479 7065  n_n} '{file_type
-0002ff40: 7d27 2077 6974 6820 666e 616d 6520 277b  }' with fname '{
-0002ff50: 666e 616d 657d 272c 2074 6865 206f 6e65  fname}', the one
-0002ff60: 2077 6974 6820 7468 6520 7368 6f72 7465   with the shorte
-0002ff70: 7374 2064 6973 616d 6269 6775 6174 696e  st disambiguatin
-0002ff80: 6720 7374 7269 6e67 2027 7b69 787d 2720  g string '{ix}' 
-0002ff90: 7761 7320 7365 6c65 6374 6564 2e22 290a  was selected.").
-0002ffa0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002ffb0: 656c 6563 7465 645f 6669 6c65 0a20 2020  elected_file.   
-0002ffc0: 2069 6620 6669 6c65 5f74 7970 6520 213d   if file_type !=
-0002ffd0: 2027 756e 6b6e 6f77 6e27 3a0a 2020 2020   'unknown':.    
-0002ffe0: 2020 2020 2320 6f74 6865 7277 6973 652c      # otherwise,
-0002fff0: 2063 6865 636b 2069 6620 6f6e 6c79 206f   check if only o
-00030000: 6e65 2066 696c 6520 6973 206c 7969 6e67  ne file is lying
-00030010: 2069 6e20 6120 6469 7265 6374 6f72 7920   in a directory 
-00030020: 7769 7468 2064 6566 6175 6c74 206e 616d  with default nam
-00030030: 650a 2020 2020 2020 2020 7375 6264 6972  e.        subdir
-00030040: 7320 3d20 6669 6c65 735f 6466 2e73 7562  s = files_df.sub
-00030050: 6469 720a 2020 2020 2020 2020 6465 6661  dir.        defa
-00030060: 756c 745f 636f 6d70 6f6e 656e 7473 203d  ult_components =
-00030070: 2066 696c 655f 7479 7065 3270 6174 685f   file_type2path_
-00030080: 636f 6d70 6f6e 656e 745f 6d61 7028 295b  component_map()[
-00030090: 6669 6c65 5f74 7970 655d 0a20 2020 2020  file_type].     
-000300a0: 2020 2064 6566 6175 6c74 5f63 6f6d 706f     default_compo
-000300b0: 6e65 6e74 735f 7265 6765 7820 3d20 277c  nents_regex = '|
-000300c0: 272e 6a6f 696e 2863 6f6d 702e 7265 706c  '.join(comp.repl
-000300d0: 6163 6528 272e 272c 2072 275c 2e27 2920  ace('.', r'\.') 
-000300e0: 666f 7220 636f 6d70 2069 6e20 6465 6661  for comp in defa
-000300f0: 756c 745f 636f 6d70 6f6e 656e 7473 290a  ult_components).
-00030100: 2020 2020 2020 2020 6465 6661 756c 745f          default_
-00030110: 7365 6c65 6374 6f72 203d 2073 7562 6469  selector = subdi
-00030120: 7273 2e73 7472 2e63 6f6e 7461 696e 7328  rs.str.contains(
-00030130: 6465 6661 756c 745f 636f 6d70 6f6e 656e  default_componen
-00030140: 7473 5f72 6567 6578 2c20 7265 6765 783d  ts_regex, regex=
-00030150: 5472 7565 290a 2020 2020 2020 2020 6966  True).        if
-00030160: 2064 6566 6175 6c74 5f73 656c 6563 746f   default_selecto
-00030170: 722e 7375 6d28 2920 3d3d 2031 3a0a 2020  r.sum() == 1:.  
-00030180: 2020 2020 2020 2020 2020 7375 6264 6972            subdir
-00030190: 203d 2073 7562 6469 7273 5b64 6566 6175   = subdirs[defau
-000301a0: 6c74 5f73 656c 6563 746f 725d 2e69 6c6f  lt_selector].ilo
-000301b0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-000301c0: 2073 656c 6563 7465 645f 6669 6c65 203d   selected_file =
-000301d0: 2064 6973 616d 625f 7365 7269 6573 5b64   disamb_series[d
-000301e0: 6566 6175 6c74 5f73 656c 6563 746f 725d  efault_selector]
-000301f0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-00030200: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00030210: 6728 6622 496e 206f 7264 6572 2074 6f20  g(f"In order to 
-00030220: 7069 636b 206f 6e65 2066 726f 6d20 7468  pick one from th
-00030230: 6520 7b63 686f 6963 655f 6265 7477 6565  e {choice_betwee
-00030240: 6e5f 6e7d 2027 7b66 696c 655f 7479 7065  n_n} '{file_type
-00030250: 7d27 2077 6974 6820 666e 616d 6520 277b  }' with fname '{
-00030260: 666e 616d 657d 272c 2074 6865 206f 6e65  fname}', the one
-00030270: 2069 6e20 7468 6520 6465 6661 756c 7420   in the default 
-00030280: 7375 6264 6972 2027 7b73 7562 6469 727d  subdir '{subdir}
-00030290: 2720 7761 7320 7365 6c65 6374 6564 2e22  ' was selected."
-000302a0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000302b0: 7475 726e 2073 656c 6563 7465 645f 6669  turn selected_fi
-000302c0: 6c65 0a20 2020 2020 2020 2023 206f 7220  le.        # or 
-000302d0: 6966 206f 6e6c 7920 6f6e 6520 6669 6c65  if only one file
-000302e0: 2063 6f6e 7461 696e 7320 6120 6465 6661   contains a defa
-000302f0: 756c 7420 6e61 6d65 2069 6e20 6974 7320  ult name in its 
-00030300: 7375 6666 6978 0a20 2020 2020 2020 2073  suffix.        s
-00030310: 7566 6669 7865 7320 3d20 6669 6c65 735f  uffixes = files_
-00030320: 6466 2e73 7566 6669 780a 2020 2020 2020  df.suffix.      
-00030330: 2020 6465 6661 756c 745f 7365 6c65 6374    default_select
-00030340: 6f72 203d 2073 7566 6669 7865 732e 7374  or = suffixes.st
-00030350: 722e 636f 6e74 6169 6e73 2864 6566 6175  r.contains(defau
-00030360: 6c74 5f63 6f6d 706f 6e65 6e74 735f 7265  lt_components_re
-00030370: 6765 782c 2072 6567 6578 3d54 7275 6529  gex, regex=True)
-00030380: 0a20 2020 2020 2020 2069 6620 6465 6661  .        if defa
-00030390: 756c 745f 7365 6c65 6374 6f72 2e73 756d  ult_selector.sum
-000303a0: 2829 203d 3d20 313a 0a20 2020 2020 2020  () == 1:.       
-000303b0: 2020 2020 2073 7566 6669 7820 3d20 7375       suffix = su
-000303c0: 6666 6978 6573 5b64 6566 6175 6c74 5f73  ffixes[default_s
-000303d0: 656c 6563 746f 725d 2e69 6c6f 635b 305d  elector].iloc[0]
-000303e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000303f0: 6563 7465 645f 6669 6c65 203d 2064 6973  ected_file = dis
-00030400: 616d 625f 7365 7269 6573 5b64 6566 6175  amb_series[defau
-00030410: 6c74 5f73 656c 6563 746f 725d 2e69 6c6f  lt_selector].ilo
-00030420: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-00030430: 206c 6f67 6765 722e 6465 6275 6728 6622   logger.debug(f"
-00030440: 496e 206f 7264 6572 2074 6f20 7069 636b  In order to pick
-00030450: 206f 6e65 2066 726f 6d20 7468 6520 7b63   one from the {c
-00030460: 686f 6963 655f 6265 7477 6565 6e5f 6e7d  hoice_between_n}
-00030470: 2027 7b66 696c 655f 7479 7065 7d27 2077   '{file_type}' w
-00030480: 6974 6820 666e 616d 6520 277b 666e 616d  ith fname '{fnam
-00030490: 657d 272c 2074 6865 206f 6e65 2069 6e20  e}', the one in 
-000304a0: 7468 6520 6465 6661 756c 7420 7375 6666  the default suff
-000304b0: 6978 2027 7b73 7566 6669 787d 2720 7761  ix '{suffix}' wa
-000304c0: 7320 7365 6c65 6374 6564 2e22 290a 2020  s selected.").  
-000304d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000304e0: 2073 656c 6563 7465 645f 6669 6c65 0a20   selected_file. 
-000304f0: 2020 2023 2069 6620 6e6f 2066 696c 6520     # if no file 
-00030500: 7761 7320 7365 6c65 6374 6564 2c20 7472  was selected, tr
-00030510: 7920 6167 6169 6e20 7769 7468 206f 6e6c  y again with onl
-00030520: 7920 7468 6f73 6520 6861 7669 6e67 2074  y those having t
-00030530: 6865 2073 686f 7274 6573 7420 6469 7361  he shortest disa
-00030540: 6d62 6967 7561 7469 6f6e 2073 7472 696e  mbiguation strin
-00030550: 6773 0a20 2020 2069 6620 7368 6f72 7465  gs.    if shorte
-00030560: 7374 5f6c 656e 6774 685f 7365 6c65 6374  st_length_select
-00030570: 6f72 2e61 6c6c 2829 3a0a 2020 2020 2020  or.all():.      
-00030580: 2020 2320 6966 2061 6c6c 2064 6973 616d    # if all disam
-00030590: 6269 6775 6174 696f 6e20 7374 7269 6e67  biguation string
-000305a0: 7320 616c 7265 6164 7920 6861 7665 2074  s already have t
-000305b0: 6865 2073 686f 7274 6573 7420 6c65 6e67  he shortest leng
-000305c0: 7468 2c20 6173 2061 206c 6173 7420 7265  th, as a last re
-000305d0: 736f 7274 0a20 2020 2020 2020 2023 2066  sort.        # f
-000305e0: 616c 6c20 6261 636b 2074 6f20 7468 6520  all back to the 
-000305f0: 6c65 7869 676f 6772 6170 6869 6361 6c6c  lexigographicall
-00030600: 7920 6669 7273 740a 2020 2020 2020 2020  y first.        
-00030610: 736f 7274 6564 5f64 6973 616d 625f 7365  sorted_disamb_se
-00030620: 7269 6573 203d 2064 6973 616d 625f 7365  ries = disamb_se
-00030630: 7269 6573 2e73 6f72 745f 696e 6465 7828  ries.sort_index(
-00030640: 290a 2020 2020 2020 2020 6469 7361 6d62  ).        disamb
-00030650: 203d 2073 6f72 7465 645f 6469 7361 6d62   = sorted_disamb
-00030660: 5f73 6572 6965 732e 696e 6465 785b 305d  _series.index[0]
-00030670: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
-00030680: 645f 6669 6c65 203d 2073 6f72 7465 645f  d_file = sorted_
-00030690: 6469 7361 6d62 5f73 6572 6965 732e 696c  disamb_series.il
-000306a0: 6f63 5b30 5d0a 2020 2020 2020 2020 6c6f  oc[0].        lo
-000306b0: 6767 6572 2e77 6172 6e69 6e67 2866 2255  gger.warning(f"U
-000306c0: 6e61 626c 6520 746f 2061 7574 6f6d 6174  nable to automat
-000306d0: 6963 616c 6c79 2063 686f 6f73 6520 6672  ically choose fr
-000306e0: 6f6d 2074 6865 207b 6368 6f69 6365 5f62  om the {choice_b
-000306f0: 6574 7765 656e 5f6e 7d20 277b 6669 6c65  etween_n} '{file
-00030700: 5f74 7970 657d 2720 7769 7468 2066 6e61  _type}' with fna
-00030710: 6d65 2027 7b66 6e61 6d65 7d27 2e20 4927  me '{fname}'. I'
-00030720: 6d20 7069 636b 696e 6720 277b 7365 6c65  m picking '{sele
-00030730: 6374 6564 5f66 696c 652e 7265 6c5f 7061  cted_file.rel_pa
-00030740: 7468 7d27 2022 0a20 2020 2020 2020 2020  th}' ".         
-00030750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030760: 2020 2066 2262 6563 6175 7365 2069 7473     f"because its
-00030770: 2064 6973 616d 6269 6775 6174 696f 6e20   disambiguation 
-00030780: 7374 7269 6e67 2027 7b64 6973 616d 627d  string '{disamb}
-00030790: 2720 6973 2074 6865 206c 6578 6963 6f67  ' is the lexicog
-000307a0: 7261 7068 6963 616c 6c79 2066 6972 7374  raphically first
-000307b0: 2061 6d6f 6e67 207b 736f 7274 6564 5f64   among {sorted_d
-000307c0: 6973 616d 625f 7365 7269 6573 2e69 6e64  isamb_series.ind
-000307d0: 6578 2e74 6f5f 6c69 7374 2829 7d22 290a  ex.to_list()}").
-000307e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000307f0: 656c 6563 7465 645f 6669 6c65 0a20 2020  elected_file.   
-00030800: 206f 6e6c 795f 7368 6f72 7465 7374 5f64   only_shortest_d
-00030810: 6973 616d 625f 7374 7220 3d20 6469 7361  isamb_str = disa
-00030820: 6d62 5f73 6572 6965 735b 7368 6f72 7465  mb_series[shorte
-00030830: 7374 5f6c 656e 6774 685f 7365 6c65 6374  st_length_select
-00030840: 6f72 5d2e 746f 5f64 6963 7428 290a 2020  or].to_dict().  
-00030850: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
-00030860: 4166 7465 7220 7468 6520 6669 7273 7420  After the first 
-00030870: 756e 7375 6363 6573 7366 756c 2061 7474  unsuccessful att
-00030880: 656d 7074 2074 6f20 6368 6f6f 7365 2066  empt to choose f
-00030890: 726f 6d20 7b63 686f 6963 655f 6265 7477  rom {choice_betw
-000308a0: 6565 6e5f 6e7d 2027 7b66 696c 655f 7479  een_n} '{file_ty
-000308b0: 7065 7d27 2077 6974 6820 666e 616d 6520  pe}' with fname 
-000308c0: 277b 666e 616d 657d 272c 2074 7279 696e  '{fname}', tryin
-000308d0: 6720 6167 6169 6e20 220a 2020 2020 2020  g again ".      
-000308e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000308f0: 2020 6622 6166 7465 7220 7265 6475 6369    f"after reduci
-00030900: 6e67 2074 6865 2063 686f 6963 6573 2074  ng the choices t
-00030910: 6f20 7468 6520 7b73 686f 7274 6573 745f  o the {shortest_
-00030920: 6c65 6e67 7468 5f73 656c 6563 746f 722e  length_selector.
-00030930: 7375 6d28 297d 2077 6974 6820 7468 6520  sum()} with the 
-00030940: 7368 6f72 7465 7374 2064 6973 616d 6269  shortest disambi
-00030950: 6775 6174 696f 6e20 7374 7269 6e67 732e  guation strings.
-00030960: 2229 0a20 2020 2072 6574 7572 6e20 6175  ").    return au
-00030970: 746f 6d61 7469 6361 6c6c 795f 6368 6f6f  tomatically_choo
-00030980: 7365 5f66 726f 6d5f 6469 7361 6d62 6967  se_from_disambig
-00030990: 7561 7465 645f 6669 6c65 7328 6f6e 6c79  uated_files(only
-000309a0: 5f73 686f 7274 6573 745f 6469 7361 6d62  _shortest_disamb
-000309b0: 5f73 7472 2c20 666e 616d 652c 2066 696c  _str, fname, fil
-000309c0: 655f 7479 7065 290a 0a64 6566 2061 736b  e_type)..def ask
-000309d0: 5f75 7365 725f 746f 5f63 686f 6f73 6528  _user_to_choose(
-000309e0: 7175 6572 793a 2073 7472 2c20 6368 6f69  query: str, choi
-000309f0: 6365 733a 2043 6f6c 6c65 6374 696f 6e5b  ces: Collection[
-00030a00: 416e 795d 2920 2d3e 204f 7074 696f 6e61  Any]) -> Optiona
-00030a10: 6c5b 416e 795d 3a0a 2020 2020 2222 2241  l[Any]:.    """A
-00030a20: 736b 2075 7365 7220 746f 2069 6e70 7574  sk user to input
-00030a30: 2061 6e20 696e 7465 6765 7220 616e 6420   an integer and 
-00030a40: 7265 7475 726e 2074 6865 206e 7468 2063  return the nth c
-00030a50: 686f 6963 6520 7365 6c65 6374 6564 2062  hoice selected b
-00030a60: 7920 7468 6520 7573 6572 2e22 2222 0a20  y the user.""". 
-00030a70: 2020 206e 5f63 686f 6963 6573 203d 206c     n_choices = l
-00030a80: 656e 2863 686f 6963 6573 290a 2020 2020  en(choices).    
-00030a90: 7261 6e67 655f 7374 7220 3d20 6622 312d  range_str = f"1-
-00030aa0: 7b6e 5f63 686f 6963 6573 7d22 0a20 2020  {n_choices}".   
-00030ab0: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
-00030ac0: 2020 2020 2073 203d 2069 6e70 7574 2871       s = input(q
-00030ad0: 7565 7279 290a 2020 2020 2020 2020 7472  uery).        tr
-00030ae0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-00030af0: 6e74 5f69 203d 2069 6e74 2873 290a 2020  nt_i = int(s).  
-00030b00: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00030b10: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
-00030b20: 2020 2020 7072 696e 7428 6622 5661 6c75      print(f"Valu
-00030b30: 6520 277b 737d 2720 636f 756c 6420 6e6f  e '{s}' could no
-00030b40: 7420 6265 2063 6f6e 7665 7274 6564 2074  t be converted t
-00030b50: 6f20 616e 2069 6e74 6567 6572 2e22 290a  o an integer.").
-00030b60: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00030b70: 696e 7565 0a20 2020 2020 2020 2069 6620  inue.        if 
-00030b80: 6e6f 7420 2830 203c 3d20 696e 745f 6920  not (0 <= int_i 
-00030b90: 3c3d 206e 5f63 686f 6963 6573 293a 0a20  <= n_choices):. 
-00030ba0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00030bb0: 2866 2256 616c 7565 2027 7b73 7d27 2069  (f"Value '{s}' i
-00030bc0: 7320 6e6f 7420 7769 7468 696e 207b 7261  s not within {ra
-00030bd0: 6e67 655f 7374 727d 2e22 290a 2020 2020  nge_str}.").    
-00030be0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00030bf0: 0a20 2020 2020 2020 2069 6620 696e 745f  .        if int_
-00030c00: 6920 3d3d 2030 3a0a 2020 2020 2020 2020  i == 0:.        
-00030c10: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00030c20: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00030c30: 686f 6963 6573 5b69 6e74 5f69 202d 2031  hoices[int_i - 1
-00030c40: 5d0a 0a0a 6465 6620 6173 6b5f 7573 6572  ]...def ask_user
-00030c50: 5f74 6f5f 6368 6f6f 7365 5f66 726f 6d5f  _to_choose_from_
-00030c60: 6469 7361 6d62 6967 7561 7465 645f 6669  disambiguated_fi
-00030c70: 6c65 7328 6469 7361 6d62 6967 7561 7465  les(disambiguate
-00030c80: 645f 6368 6f69 6365 733a 2044 6963 745b  d_choices: Dict[
-00030c90: 7374 722c 2046 696c 655d 2c0a 2020 2020  str, File],.    
-00030ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030cc0: 2020 2020 2020 2020 2020 2020 666e 616d              fnam
-00030cd0: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
-00030ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f7e0: 6669 6c65 5f74 7970 653a 2073 7472 2c0a  file_type: str,.
+0002f7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f820: 2020 2920 2d3e 2046 696c 653a 0a20 2020    ) -> File:.   
+0002f830: 2069 6620 6c65 6e28 6469 7361 6d62 6967   if len(disambig
+0002f840: 7561 7465 645f 6368 6f69 6365 7329 203d  uated_choices) =
+0002f850: 3d20 313a 0a20 2020 2020 2020 2072 6574  = 1:.        ret
+0002f860: 7572 6e20 6c69 7374 2864 6973 616d 6269  urn list(disambi
+0002f870: 6775 6174 6564 5f63 686f 6963 6573 2e6b  guated_choices.k
+0002f880: 6579 7328 2929 5b30 5d0a 2020 2020 6469  eys())[0].    di
+0002f890: 7361 6d62 5f73 6572 6965 7320 3d20 7064  samb_series = pd
+0002f8a0: 2e53 6572 6965 7328 6469 7361 6d62 6967  .Series(disambig
+0002f8b0: 7561 7465 645f 6368 6f69 6365 7329 0a20  uated_choices). 
+0002f8c0: 2020 2066 696c 6573 203d 206c 6973 7428     files = list(
+0002f8d0: 6469 7361 6d62 6967 7561 7465 645f 6368  disambiguated_ch
+0002f8e0: 6f69 6365 732e 7661 6c75 6573 2829 290a  oices.values()).
+0002f8f0: 2020 2020 6669 6c65 735f 6466 203d 2070      files_df = p
+0002f900: 642e 4461 7461 4672 616d 6528 6669 6c65  d.DataFrame(file
+0002f910: 732c 2069 6e64 6578 3d64 6973 616d 625f  s, index=disamb_
+0002f920: 7365 7269 6573 2e69 6e64 6578 290a 2020  series.index).  
+0002f930: 2020 6368 6f69 6365 5f62 6574 7765 656e    choice_between
+0002f940: 5f6e 203d 206c 656e 2866 696c 6573 290a  _n = len(files).
+0002f950: 2020 2020 6966 2066 696c 655f 7479 7065      if file_type
+0002f960: 203d 3d20 2773 636f 7265 7327 3a0a 2020   == 'scores':.  
+0002f970: 2020 2020 2020 2320 6966 2061 2073 636f        # if a sco
+0002f980: 7265 2069 7320 7265 7175 6573 7465 642c  re is requested,
+0002f990: 2063 6865 636b 2069 6620 7468 6572 6520   check if there 
+0002f9a0: 6973 206f 6e6c 7920 6120 7369 6e67 6c65  is only a single
+0002f9b0: 204d 5343 5820 6f72 206f 7468 6572 7769   MSCX or otherwi
+0002f9c0: 7365 204d 5343 5a20 6669 6c65 2061 6e64  se MSCZ file and
+0002f9d0: 2070 6963 6b20 7468 6174 0a20 2020 2020   pick that.     
+0002f9e0: 2020 2066 6578 7473 203d 2066 696c 6573     fexts = files
+0002f9f0: 5f64 662e 6665 7874 2e73 7472 2e6c 6f77  _df.fext.str.low
+0002fa00: 6572 2829 0a20 2020 2020 2020 2066 6578  er().        fex
+0002fa10: 745f 636f 756e 7473 203d 2066 6578 7473  t_counts = fexts
+0002fa20: 2e76 616c 7565 5f63 6f75 6e74 7328 290a  .value_counts().
+0002fa30: 2020 2020 2020 2020 6966 2027 2e6d 7363          if '.msc
+0002fa40: 7827 2069 6e20 6665 7874 5f63 6f75 6e74  x' in fext_count
+0002fa50: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+0002fa60: 6620 6665 7874 5f63 6f75 6e74 735b 272e  f fext_counts['.
+0002fa70: 6d73 6378 275d 203d 3d20 313a 0a20 2020  mscx'] == 1:.   
+0002fa80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0002fa90: 6563 7465 645f 6669 6c65 203d 2064 6973  ected_file = dis
+0002faa0: 616d 625f 7365 7269 6573 5b66 6578 7473  amb_series[fexts
+0002fab0: 203d 3d20 272e 6d73 6378 275d 2e69 6c6f   == '.mscx'].ilo
+0002fac0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+0002fad0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0002fae0: 6728 6622 496e 206f 7264 6572 2074 6f20  g(f"In order to 
+0002faf0: 7069 636b 206f 6e65 2066 726f 6d20 7468  pick one from th
+0002fb00: 6520 7b63 686f 6963 655f 6265 7477 6565  e {choice_betwee
+0002fb10: 6e5f 6e7d 2073 636f 7265 7320 7769 7468  n_n} scores with
+0002fb20: 2066 6e61 6d65 2027 7b66 6e61 6d65 7d27   fname '{fname}'
+0002fb30: 2c20 277b 7365 6c65 6374 6564 5f66 696c  , '{selected_fil
+0002fb40: 652e 7265 6c5f 7061 7468 7d27 2077 6173  e.rel_path}' was
+0002fb50: 2073 656c 6563 7465 6420 6265 6361 7573   selected becaus
+0002fb60: 6520 6974 2069 7320 7468 6520 6f6e 6c79  e it is the only
+0002fb70: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0002fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fb90: 2020 2020 6622 6f6e 6520 696e 204d 5343      f"one in MSC
+0002fba0: 5820 666f 726d 6174 2e22 290a 2020 2020  X format.").    
+0002fbb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0002fbc0: 726e 2073 656c 6563 7465 645f 6669 6c65  rn selected_file
+0002fbd0: 0a20 2020 2020 2020 2065 6c69 6620 272e  .        elif '.
+0002fbe0: 6d73 637a 2720 696e 2066 6578 745f 636f  mscz' in fext_co
+0002fbf0: 756e 7473 2061 6e64 2066 6578 745f 636f  unts and fext_co
+0002fc00: 756e 7473 5b27 2e6d 7363 7a27 5d20 3d3d  unts['.mscz'] ==
+0002fc10: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0002fc20: 7365 6c65 6374 6564 5f66 696c 6520 3d20  selected_file = 
+0002fc30: 6469 7361 6d62 5f73 6572 6965 735b 6665  disamb_series[fe
+0002fc40: 7874 7320 3d3d 2027 2e6d 7363 7a27 5d2e  xts == '.mscz'].
+0002fc50: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
+0002fc60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0002fc70: 2866 2249 6e20 6f72 6465 7220 746f 2070  (f"In order to p
+0002fc80: 6963 6b20 6f6e 6520 6672 6f6d 2074 6865  ick one from the
+0002fc90: 207b 6368 6f69 6365 5f62 6574 7765 656e   {choice_between
+0002fca0: 5f6e 7d20 7363 6f72 6573 2077 6974 6820  _n} scores with 
+0002fcb0: 666e 616d 6520 277b 666e 616d 657d 272c  fname '{fname}',
+0002fcc0: 2027 7b73 656c 6563 7465 645f 6669 6c65   '{selected_file
+0002fcd0: 2e72 656c 5f70 6174 687d 2720 7761 7320  .rel_path}' was 
+0002fce0: 7365 6c65 6374 6564 2062 6563 6175 7365  selected because
+0002fcf0: 2069 7420 6973 2074 6865 206f 6e6c 7920   it is the only 
+0002fd00: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0002fd10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002fd20: 226f 6e65 2069 6e20 4d53 435a 2066 6f72  "one in MSCZ for
+0002fd30: 6d61 742e 2229 0a20 2020 2020 2020 2020  mat.").         
+0002fd40: 2020 2072 6574 7572 6e20 7365 6c65 6374     return select
+0002fd50: 6564 5f66 696c 650a 2020 2020 2320 6173  ed_file.    # as
+0002fd60: 2066 6972 7374 2064 6973 616d 6269 6775   first disambigu
+0002fd70: 6174 696f 6e20 6372 6974 6572 696f 6e2c  ation criterion,
+0002fd80: 2063 6865 636b 2069 6620 7468 6520 7368   check if the sh
+0002fd90: 6f72 7465 7374 2064 6973 616d 6269 6775  ortest disambigu
+0002fda0: 6174 696f 6e20 7374 7269 6e67 2070 6572  ation string per
+0002fdb0: 7461 696e 7320 746f 2031 2066 696c 6520  tains to 1 file 
+0002fdc0: 6f6e 6c79 2061 6e64 2070 6963 6b20 7468  only and pick th
+0002fdd0: 6174 0a20 2020 2064 6973 616d 625f 7374  at.    disamb_st
+0002fde0: 725f 6c65 6e67 7468 7320 3d20 7064 2e53  r_lengths = pd.S
+0002fdf0: 6572 6965 7328 6469 7361 6d62 5f73 6572  eries(disamb_ser
+0002fe00: 6965 732e 696e 6465 782e 6d61 7028 6c65  ies.index.map(le
+0002fe10: 6e29 2c20 696e 6465 783d 6469 7361 6d62  n), index=disamb
+0002fe20: 5f73 6572 6965 732e 696e 6465 7829 0a20  _series.index). 
+0002fe30: 2020 2073 686f 7274 6573 745f 6c65 6e67     shortest_leng
+0002fe40: 7468 5f73 656c 6563 746f 7220 3d20 2864  th_selector = (d
+0002fe50: 6973 616d 625f 7374 725f 6c65 6e67 7468  isamb_str_length
+0002fe60: 7320 3d3d 2064 6973 616d 625f 7374 725f  s == disamb_str_
+0002fe70: 6c65 6e67 7468 732e 6d69 6e28 2929 0a20  lengths.min()). 
+0002fe80: 2020 206e 5f68 6176 655f 7368 6f72 7465     n_have_shorte
+0002fe90: 7374 5f6c 656e 6774 6820 3d20 7368 6f72  st_length = shor
+0002fea0: 7465 7374 5f6c 656e 6774 685f 7365 6c65  test_length_sele
+0002feb0: 6374 6f72 2e73 756d 2829 0a20 2020 2069  ctor.sum().    i
+0002fec0: 6620 6e5f 6861 7665 5f73 686f 7274 6573  f n_have_shortes
+0002fed0: 745f 6c65 6e67 7468 203d 3d20 313a 0a20  t_length == 1:. 
+0002fee0: 2020 2020 2020 2069 7820 3d20 6469 7361         ix = disa
+0002fef0: 6d62 5f73 7472 5f6c 656e 6774 6873 2e69  mb_str_lengths.i
+0002ff00: 6478 6d69 6e28 290a 2020 2020 2020 2020  dxmin().        
+0002ff10: 7365 6c65 6374 6564 5f66 696c 6520 3d20  selected_file = 
+0002ff20: 6469 7361 6d62 5f73 6572 6965 732e 6c6f  disamb_series.lo
+0002ff30: 635b 6978 5d0a 2020 2020 2020 2020 6c6f  c[ix].        lo
+0002ff40: 6767 6572 2e64 6562 7567 2866 2249 6e20  gger.debug(f"In 
+0002ff50: 6f72 6465 7220 746f 2070 6963 6b20 6f6e  order to pick on
+0002ff60: 6520 6672 6f6d 2074 6865 207b 6368 6f69  e from the {choi
+0002ff70: 6365 5f62 6574 7765 656e 5f6e 7d20 277b  ce_between_n} '{
+0002ff80: 6669 6c65 5f74 7970 657d 2720 7769 7468  file_type}' with
+0002ff90: 2066 6e61 6d65 2027 7b66 6e61 6d65 7d27   fname '{fname}'
+0002ffa0: 2c20 7468 6520 6f6e 6520 7769 7468 2074  , the one with t
+0002ffb0: 6865 2073 686f 7274 6573 7420 6469 7361  he shortest disa
+0002ffc0: 6d62 6967 7561 7469 6e67 2073 7472 696e  mbiguating strin
+0002ffd0: 6720 277b 6978 7d27 2077 6173 2073 656c  g '{ix}' was sel
+0002ffe0: 6563 7465 642e 2229 0a20 2020 2020 2020  ected.").       
+0002fff0: 2072 6574 7572 6e20 7365 6c65 6374 6564   return selected
+00030000: 5f66 696c 650a 2020 2020 6966 2066 696c  _file.    if fil
+00030010: 655f 7479 7065 2021 3d20 2775 6e6b 6e6f  e_type != 'unkno
+00030020: 776e 273a 0a20 2020 2020 2020 2023 206f  wn':.        # o
+00030030: 7468 6572 7769 7365 2c20 6368 6563 6b20  therwise, check 
+00030040: 6966 206f 6e6c 7920 6f6e 6520 6669 6c65  if only one file
+00030050: 2069 7320 6c79 696e 6720 696e 2061 2064   is lying in a d
+00030060: 6972 6563 746f 7279 2077 6974 6820 6465  irectory with de
+00030070: 6661 756c 7420 6e61 6d65 0a20 2020 2020  fault name.     
+00030080: 2020 2073 7562 6469 7273 203d 2066 696c     subdirs = fil
+00030090: 6573 5f64 662e 7375 6264 6972 0a20 2020  es_df.subdir.   
+000300a0: 2020 2020 2064 6566 6175 6c74 5f63 6f6d       default_com
+000300b0: 706f 6e65 6e74 7320 3d20 6669 6c65 5f74  ponents = file_t
+000300c0: 7970 6532 7061 7468 5f63 6f6d 706f 6e65  ype2path_compone
+000300d0: 6e74 5f6d 6170 2829 5b66 696c 655f 7479  nt_map()[file_ty
+000300e0: 7065 5d0a 2020 2020 2020 2020 6465 6661  pe].        defa
+000300f0: 756c 745f 636f 6d70 6f6e 656e 7473 5f72  ult_components_r
+00030100: 6567 6578 203d 2027 7c27 2e6a 6f69 6e28  egex = '|'.join(
+00030110: 636f 6d70 2e72 6570 6c61 6365 2827 2e27  comp.replace('.'
+00030120: 2c20 7227 5c2e 2729 2066 6f72 2063 6f6d  , r'\.') for com
+00030130: 7020 696e 2064 6566 6175 6c74 5f63 6f6d  p in default_com
+00030140: 706f 6e65 6e74 7329 0a20 2020 2020 2020  ponents).       
+00030150: 2064 6566 6175 6c74 5f73 656c 6563 746f   default_selecto
+00030160: 7220 3d20 7375 6264 6972 732e 7374 722e  r = subdirs.str.
+00030170: 636f 6e74 6169 6e73 2864 6566 6175 6c74  contains(default
+00030180: 5f63 6f6d 706f 6e65 6e74 735f 7265 6765  _components_rege
+00030190: 782c 2072 6567 6578 3d54 7275 6529 0a20  x, regex=True). 
+000301a0: 2020 2020 2020 2069 6620 6465 6661 756c         if defaul
+000301b0: 745f 7365 6c65 6374 6f72 2e73 756d 2829  t_selector.sum()
+000301c0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+000301d0: 2020 2073 7562 6469 7220 3d20 7375 6264     subdir = subd
+000301e0: 6972 735b 6465 6661 756c 745f 7365 6c65  irs[default_sele
+000301f0: 6374 6f72 5d2e 696c 6f63 5b30 5d0a 2020  ctor].iloc[0].  
+00030200: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+00030210: 6564 5f66 696c 6520 3d20 6469 7361 6d62  ed_file = disamb
+00030220: 5f73 6572 6965 735b 6465 6661 756c 745f  _series[default_
+00030230: 7365 6c65 6374 6f72 5d2e 696c 6f63 5b30  selector].iloc[0
+00030240: 5d0a 2020 2020 2020 2020 2020 2020 6c6f  ].            lo
+00030250: 6767 6572 2e64 6562 7567 2866 2249 6e20  gger.debug(f"In 
+00030260: 6f72 6465 7220 746f 2070 6963 6b20 6f6e  order to pick on
+00030270: 6520 6672 6f6d 2074 6865 207b 6368 6f69  e from the {choi
+00030280: 6365 5f62 6574 7765 656e 5f6e 7d20 277b  ce_between_n} '{
+00030290: 6669 6c65 5f74 7970 657d 2720 7769 7468  file_type}' with
+000302a0: 2066 6e61 6d65 2027 7b66 6e61 6d65 7d27   fname '{fname}'
+000302b0: 2c20 7468 6520 6f6e 6520 696e 2074 6865  , the one in the
+000302c0: 2064 6566 6175 6c74 2073 7562 6469 7220   default subdir 
+000302d0: 277b 7375 6264 6972 7d27 2077 6173 2073  '{subdir}' was s
+000302e0: 656c 6563 7465 642e 2229 0a20 2020 2020  elected.").     
+000302f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00030300: 6c65 6374 6564 5f66 696c 650a 2020 2020  lected_file.    
+00030310: 2020 2020 2320 6f72 2069 6620 6f6e 6c79      # or if only
+00030320: 206f 6e65 2066 696c 6520 636f 6e74 6169   one file contai
+00030330: 6e73 2061 2064 6566 6175 6c74 206e 616d  ns a default nam
+00030340: 6520 696e 2069 7473 2073 7566 6669 780a  e in its suffix.
+00030350: 2020 2020 2020 2020 7375 6666 6978 6573          suffixes
+00030360: 203d 2066 696c 6573 5f64 662e 7375 6666   = files_df.suff
+00030370: 6978 0a20 2020 2020 2020 2064 6566 6175  ix.        defau
+00030380: 6c74 5f73 656c 6563 746f 7220 3d20 7375  lt_selector = su
+00030390: 6666 6978 6573 2e73 7472 2e63 6f6e 7461  ffixes.str.conta
+000303a0: 696e 7328 6465 6661 756c 745f 636f 6d70  ins(default_comp
+000303b0: 6f6e 656e 7473 5f72 6567 6578 2c20 7265  onents_regex, re
+000303c0: 6765 783d 5472 7565 290a 2020 2020 2020  gex=True).      
+000303d0: 2020 6966 2064 6566 6175 6c74 5f73 656c    if default_sel
+000303e0: 6563 746f 722e 7375 6d28 2920 3d3d 2031  ector.sum() == 1
+000303f0: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
+00030400: 6666 6978 203d 2073 7566 6669 7865 735b  ffix = suffixes[
+00030410: 6465 6661 756c 745f 7365 6c65 6374 6f72  default_selector
+00030420: 5d2e 696c 6f63 5b30 5d0a 2020 2020 2020  ].iloc[0].      
+00030430: 2020 2020 2020 7365 6c65 6374 6564 5f66        selected_f
+00030440: 696c 6520 3d20 6469 7361 6d62 5f73 6572  ile = disamb_ser
+00030450: 6965 735b 6465 6661 756c 745f 7365 6c65  ies[default_sele
+00030460: 6374 6f72 5d2e 696c 6f63 5b30 5d0a 2020  ctor].iloc[0].  
+00030470: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00030480: 2e64 6562 7567 2866 2249 6e20 6f72 6465  .debug(f"In orde
+00030490: 7220 746f 2070 6963 6b20 6f6e 6520 6672  r to pick one fr
+000304a0: 6f6d 2074 6865 207b 6368 6f69 6365 5f62  om the {choice_b
+000304b0: 6574 7765 656e 5f6e 7d20 277b 6669 6c65  etween_n} '{file
+000304c0: 5f74 7970 657d 2720 7769 7468 2066 6e61  _type}' with fna
+000304d0: 6d65 2027 7b66 6e61 6d65 7d27 2c20 7468  me '{fname}', th
+000304e0: 6520 6f6e 6520 696e 2074 6865 2064 6566  e one in the def
+000304f0: 6175 6c74 2073 7566 6669 7820 277b 7375  ault suffix '{su
+00030500: 6666 6978 7d27 2077 6173 2073 656c 6563  ffix}' was selec
+00030510: 7465 642e 2229 0a20 2020 2020 2020 2020  ted.").         
+00030520: 2020 2072 6574 7572 6e20 7365 6c65 6374     return select
+00030530: 6564 5f66 696c 650a 2020 2020 2320 6966  ed_file.    # if
+00030540: 206e 6f20 6669 6c65 2077 6173 2073 656c   no file was sel
+00030550: 6563 7465 642c 2074 7279 2061 6761 696e  ected, try again
+00030560: 2077 6974 6820 6f6e 6c79 2074 686f 7365   with only those
+00030570: 2068 6176 696e 6720 7468 6520 7368 6f72   having the shor
+00030580: 7465 7374 2064 6973 616d 6269 6775 6174  test disambiguat
+00030590: 696f 6e20 7374 7269 6e67 730a 2020 2020  ion strings.    
+000305a0: 6966 2073 686f 7274 6573 745f 6c65 6e67  if shortest_leng
+000305b0: 7468 5f73 656c 6563 746f 722e 616c 6c28  th_selector.all(
+000305c0: 293a 0a20 2020 2020 2020 2023 2069 6620  ):.        # if 
+000305d0: 616c 6c20 6469 7361 6d62 6967 7561 7469  all disambiguati
+000305e0: 6f6e 2073 7472 696e 6773 2061 6c72 6561  on strings alrea
+000305f0: 6479 2068 6176 6520 7468 6520 7368 6f72  dy have the shor
+00030600: 7465 7374 206c 656e 6774 682c 2061 7320  test length, as 
+00030610: 6120 6c61 7374 2072 6573 6f72 740a 2020  a last resort.  
+00030620: 2020 2020 2020 2320 6661 6c6c 2062 6163        # fall bac
+00030630: 6b20 746f 2074 6865 206c 6578 6967 6f67  k to the lexigog
+00030640: 7261 7068 6963 616c 6c79 2066 6972 7374  raphically first
+00030650: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
+00030660: 6469 7361 6d62 5f73 6572 6965 7320 3d20  disamb_series = 
+00030670: 6469 7361 6d62 5f73 6572 6965 732e 736f  disamb_series.so
+00030680: 7274 5f69 6e64 6578 2829 0a20 2020 2020  rt_index().     
+00030690: 2020 2064 6973 616d 6220 3d20 736f 7274     disamb = sort
+000306a0: 6564 5f64 6973 616d 625f 7365 7269 6573  ed_disamb_series
+000306b0: 2e69 6e64 6578 5b30 5d0a 2020 2020 2020  .index[0].      
+000306c0: 2020 7365 6c65 6374 6564 5f66 696c 6520    selected_file 
+000306d0: 3d20 736f 7274 6564 5f64 6973 616d 625f  = sorted_disamb_
+000306e0: 7365 7269 6573 2e69 6c6f 635b 305d 0a20  series.iloc[0]. 
+000306f0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+00030700: 726e 696e 6728 6622 556e 6162 6c65 2074  rning(f"Unable t
+00030710: 6f20 6175 746f 6d61 7469 6361 6c6c 7920  o automatically 
+00030720: 6368 6f6f 7365 2066 726f 6d20 7468 6520  choose from the 
+00030730: 7b63 686f 6963 655f 6265 7477 6565 6e5f  {choice_between_
+00030740: 6e7d 2027 7b66 696c 655f 7479 7065 7d27  n} '{file_type}'
+00030750: 2077 6974 6820 666e 616d 6520 277b 666e   with fname '{fn
+00030760: 616d 657d 272e 2049 276d 2070 6963 6b69  ame}'. I'm picki
+00030770: 6e67 2027 7b73 656c 6563 7465 645f 6669  ng '{selected_fi
+00030780: 6c65 2e72 656c 5f70 6174 687d 2720 220a  le.rel_path}' ".
+00030790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000307a0: 2020 2020 2020 2020 2020 2020 6622 6265              f"be
+000307b0: 6361 7573 6520 6974 7320 6469 7361 6d62  cause its disamb
+000307c0: 6967 7561 7469 6f6e 2073 7472 696e 6720  iguation string 
+000307d0: 277b 6469 7361 6d62 7d27 2069 7320 7468  '{disamb}' is th
+000307e0: 6520 6c65 7869 636f 6772 6170 6869 6361  e lexicographica
+000307f0: 6c6c 7920 6669 7273 7420 616d 6f6e 6720  lly first among 
+00030800: 7b73 6f72 7465 645f 6469 7361 6d62 5f73  {sorted_disamb_s
+00030810: 6572 6965 732e 696e 6465 782e 746f 5f6c  eries.index.to_l
+00030820: 6973 7428 297d 2229 0a20 2020 2020 2020  ist()}").       
+00030830: 2072 6574 7572 6e20 7365 6c65 6374 6564   return selected
+00030840: 5f66 696c 650a 2020 2020 6f6e 6c79 5f73  _file.    only_s
+00030850: 686f 7274 6573 745f 6469 7361 6d62 5f73  hortest_disamb_s
+00030860: 7472 203d 2064 6973 616d 625f 7365 7269  tr = disamb_seri
+00030870: 6573 5b73 686f 7274 6573 745f 6c65 6e67  es[shortest_leng
+00030880: 7468 5f73 656c 6563 746f 725d 2e74 6f5f  th_selector].to_
+00030890: 6469 6374 2829 0a20 2020 206c 6f67 6765  dict().    logge
+000308a0: 722e 696e 666f 2866 2241 6674 6572 2074  r.info(f"After t
+000308b0: 6865 2066 6972 7374 2075 6e73 7563 6365  he first unsucce
+000308c0: 7373 6675 6c20 6174 7465 6d70 7420 746f  ssful attempt to
+000308d0: 2063 686f 6f73 6520 6672 6f6d 207b 6368   choose from {ch
+000308e0: 6f69 6365 5f62 6574 7765 656e 5f6e 7d20  oice_between_n} 
+000308f0: 277b 6669 6c65 5f74 7970 657d 2720 7769  '{file_type}' wi
+00030900: 7468 2066 6e61 6d65 2027 7b66 6e61 6d65  th fname '{fname
+00030910: 7d27 2c20 7472 7969 6e67 2061 6761 696e  }', trying again
+00030920: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00030930: 2020 2020 2020 2020 2020 2066 2261 6674             f"aft
+00030940: 6572 2072 6564 7563 696e 6720 7468 6520  er reducing the 
+00030950: 6368 6f69 6365 7320 746f 2074 6865 207b  choices to the {
+00030960: 7368 6f72 7465 7374 5f6c 656e 6774 685f  shortest_length_
+00030970: 7365 6c65 6374 6f72 2e73 756d 2829 7d20  selector.sum()} 
+00030980: 7769 7468 2074 6865 2073 686f 7274 6573  with the shortes
+00030990: 7420 6469 7361 6d62 6967 7561 7469 6f6e  t disambiguation
+000309a0: 2073 7472 696e 6773 2e22 290a 2020 2020   strings.").    
+000309b0: 7265 7475 726e 2061 7574 6f6d 6174 6963  return automatic
+000309c0: 616c 6c79 5f63 686f 6f73 655f 6672 6f6d  ally_choose_from
+000309d0: 5f64 6973 616d 6269 6775 6174 6564 5f66  _disambiguated_f
+000309e0: 696c 6573 286f 6e6c 795f 7368 6f72 7465  iles(only_shorte
+000309f0: 7374 5f64 6973 616d 625f 7374 722c 2066  st_disamb_str, f
+00030a00: 6e61 6d65 2c20 6669 6c65 5f74 7970 6529  name, file_type)
+00030a10: 0a0a 6465 6620 6173 6b5f 7573 6572 5f74  ..def ask_user_t
+00030a20: 6f5f 6368 6f6f 7365 2871 7565 7279 3a20  o_choose(query: 
+00030a30: 7374 722c 2063 686f 6963 6573 3a20 436f  str, choices: Co
+00030a40: 6c6c 6563 7469 6f6e 5b41 6e79 5d29 202d  llection[Any]) -
+00030a50: 3e20 4f70 7469 6f6e 616c 5b41 6e79 5d3a  > Optional[Any]:
+00030a60: 0a20 2020 2022 2222 4173 6b20 7573 6572  .    """Ask user
+00030a70: 2074 6f20 696e 7075 7420 616e 2069 6e74   to input an int
+00030a80: 6567 6572 2061 6e64 2072 6574 7572 6e20  eger and return 
+00030a90: 7468 6520 6e74 6820 6368 6f69 6365 2073  the nth choice s
+00030aa0: 656c 6563 7465 6420 6279 2074 6865 2075  elected by the u
+00030ab0: 7365 722e 2222 220a 2020 2020 6e5f 6368  ser.""".    n_ch
+00030ac0: 6f69 6365 7320 3d20 6c65 6e28 6368 6f69  oices = len(choi
+00030ad0: 6365 7329 0a20 2020 2072 616e 6765 5f73  ces).    range_s
+00030ae0: 7472 203d 2066 2231 2d7b 6e5f 6368 6f69  tr = f"1-{n_choi
+00030af0: 6365 737d 220a 2020 2020 7768 696c 6520  ces}".    while 
+00030b00: 5472 7565 3a0a 2020 2020 2020 2020 7320  True:.        s 
+00030b10: 3d20 696e 7075 7428 7175 6572 7929 0a20  = input(query). 
+00030b20: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00030b30: 2020 2020 2020 2020 696e 745f 6920 3d20          int_i = 
+00030b40: 696e 7428 7329 0a20 2020 2020 2020 2065  int(s).        e
+00030b50: 7863 6570 7420 4578 6365 7074 696f 6e3a  xcept Exception:
+00030b60: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00030b70: 6e74 2866 2256 616c 7565 2027 7b73 7d27  nt(f"Value '{s}'
+00030b80: 2063 6f75 6c64 206e 6f74 2062 6520 636f   could not be co
+00030b90: 6e76 6572 7465 6420 746f 2061 6e20 696e  nverted to an in
+00030ba0: 7465 6765 722e 2229 0a20 2020 2020 2020  teger.").       
+00030bb0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00030bc0: 2020 2020 2020 6966 206e 6f74 2028 3020        if not (0 
+00030bd0: 3c3d 2069 6e74 5f69 203c 3d20 6e5f 6368  <= int_i <= n_ch
+00030be0: 6f69 6365 7329 3a0a 2020 2020 2020 2020  oices):.        
+00030bf0: 2020 2020 7072 696e 7428 6622 5661 6c75      print(f"Valu
+00030c00: 6520 277b 737d 2720 6973 206e 6f74 2077  e '{s}' is not w
+00030c10: 6974 6869 6e20 7b72 616e 6765 5f73 7472  ithin {range_str
+00030c20: 7d2e 2229 0a20 2020 2020 2020 2020 2020  }.").           
+00030c30: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00030c40: 2020 6966 2069 6e74 5f69 203d 3d20 303a    if int_i == 0:
+00030c50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00030c60: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+00030c70: 2072 6574 7572 6e20 6368 6f69 6365 735b   return choices[
+00030c80: 696e 745f 6920 2d20 315d 0a0a 0a64 6566  int_i - 1]...def
+00030c90: 2061 736b 5f75 7365 725f 746f 5f63 686f   ask_user_to_cho
+00030ca0: 6f73 655f 6672 6f6d 5f64 6973 616d 6269  ose_from_disambi
+00030cb0: 6775 6174 6564 5f66 696c 6573 2864 6973  guated_files(dis
+00030cc0: 616d 6269 6775 6174 6564 5f63 686f 6963  ambiguated_choic
+00030cd0: 6573 3a20 4469 6374 5b73 7472 2c20 4669  es: Dict[str, Fi
+00030ce0: 6c65 5d2c 0a20 2020 2020 2020 2020 2020  le],.           
 00030cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030d00: 2020 2020 2020 2020 6669 6c65 5f74 7970          file_typ
-00030d10: 653a 2073 7472 203d 2027 2729 202d 3e20  e: str = '') -> 
-00030d20: 4f70 7469 6f6e 616c 5b46 696c 655d 3a0a  Optional[File]:.
-00030d30: 2020 2020 736f 7274 6564 5f6b 6579 7320      sorted_keys 
-00030d40: 3d20 736f 7274 6564 2864 6973 616d 6269  = sorted(disambi
-00030d50: 6775 6174 6564 5f63 686f 6963 6573 2e6b  guated_choices.k
-00030d60: 6579 7328 292c 206b 6579 3d6c 616d 6264  eys(), key=lambd
-00030d70: 6120 733a 2028 6c65 6e28 7329 2c20 7329  a s: (len(s), s)
-00030d80: 290a 2020 2020 6469 7361 6d62 6967 7561  ).    disambigua
-00030d90: 7465 645f 6368 6f69 6365 7320 3d20 7b6b  ted_choices = {k
-00030da0: 3a20 6469 7361 6d62 6967 7561 7465 645f  : disambiguated_
-00030db0: 6368 6f69 6365 735b 6b5d 2066 6f72 206b  choices[k] for k
-00030dc0: 2069 6e20 736f 7274 6564 5f6b 6579 737d   in sorted_keys}
-00030dd0: 0a20 2020 2066 696c 655f 6c69 7374 203d  .    file_list =
-00030de0: 206c 6973 7428 6469 7361 6d62 6967 7561   list(disambigua
-00030df0: 7465 645f 6368 6f69 6365 732e 7661 6c75  ted_choices.valu
-00030e00: 6573 2829 290a 2020 2020 6469 7361 6d62  es()).    disamb
-00030e10: 5f73 7472 696e 6773 203d 2070 642e 5365  _strings = pd.Se
-00030e20: 7269 6573 2864 6973 616d 6269 6775 6174  ries(disambiguat
-00030e30: 6564 5f63 686f 6963 6573 2e6b 6579 7328  ed_choices.keys(
-00030e40: 292c 206e 616d 653d 2764 6973 616d 6269  ), name='disambi
-00030e50: 6775 6174 696f 6e5f 7374 7227 290a 2020  guation_str').  
-00030e60: 2020 6368 6f69 6365 735f 6466 203d 2070    choices_df = p
-00030e70: 642e 636f 6e63 6174 285b 6469 7361 6d62  d.concat([disamb
-00030e80: 5f73 7472 696e 6773 2c0a 2020 2020 2020  _strings,.      
-00030e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ea0: 2020 2020 2020 7064 2e44 6174 6146 7261        pd.DataFra
-00030eb0: 6d65 2866 696c 655f 6c69 7374 295b 5b27  me(file_list)[['
-00030ec0: 7265 6c5f 7061 7468 272c 2027 7479 7065  rel_path', 'type
-00030ed0: 272c 2027 6978 275d 5d5d 2c0a 2020 2020  ', 'ix']]],.    
-00030ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ef0: 2020 2020 2020 2061 7869 733d 3129 0a20         axis=1). 
-00030f00: 2020 2063 686f 6963 6573 5f64 662e 696e     choices_df.in
-00030f10: 6465 7820 3d20 7064 2e49 6e64 6578 2872  dex = pd.Index(r
-00030f20: 616e 6765 2831 2c20 6c65 6e28 6669 6c65  ange(1, len(file
-00030f30: 5f6c 6973 7429 202b 2031 292c 206e 616d  _list) + 1), nam
-00030f40: 653d 2773 656c 6563 743a 2729 0a20 2020  e='select:').   
-00030f50: 2072 616e 6765 5f73 7472 203d 2066 2231   range_str = f"1
-00030f60: 2d7b 6c65 6e28 6469 7361 6d62 6967 7561  -{len(disambigua
-00030f70: 7465 645f 6368 6f69 6365 7329 7d22 0a20  ted_choices)}". 
-00030f80: 2020 2071 7565 7279 203d 2066 2253 656c     query = f"Sel
-00030f90: 6563 7469 6f6e 205b 7b72 616e 6765 5f73  ection [{range_s
-00030fa0: 7472 7d5d 3a20 220a 2020 2020 7072 696e  tr}]: ".    prin
-00030fb0: 7428 6622 5365 7665 7261 6c20 277b 6669  t(f"Several '{fi
-00030fc0: 6c65 5f74 7970 657d 2720 6176 6169 6c61  le_type}' availa
-00030fd0: 626c 6520 666f 7220 277b 666e 616d 657d  ble for '{fname}
-00030fe0: 273a 5c6e 7b63 686f 6963 6573 5f64 662e  ':\n{choices_df.
-00030ff0: 746f 5f73 7472 696e 6728 297d 2229 0a20  to_string()}"). 
-00031000: 2020 2070 7269 6e74 2866 2250 6c65 6173     print(f"Pleas
-00031010: 6520 7365 6c65 6374 206f 6e65 206f 6620  e select one of 
-00031020: 7468 6520 6669 6c65 7320 6279 2070 6173  the files by pas
-00031030: 7369 6e67 2061 6e20 696e 7465 6765 7220  sing an integer 
-00031040: 6265 7477 6565 6e20 7b72 616e 6765 5f73  between {range_s
-00031050: 7472 7d20 286f 7220 3020 666f 7220 6e6f  tr} (or 0 for no
-00031060: 6e65 293a 2229 0a20 2020 2072 6574 7572  ne):").    retur
-00031070: 6e20 6173 6b5f 7573 6572 5f74 6f5f 6368  n ask_user_to_ch
-00031080: 6f6f 7365 2871 7565 7279 2c20 6669 6c65  oose(query, file
-00031090: 5f6c 6973 7429 0a0a 0a40 6675 6e63 7469  _list)...@functi
-000310a0: 6f6e 5f6c 6f67 6765 720a 6465 6620 6469  on_logger.def di
-000310b0: 7361 6d62 6967 7561 7465 5f66 696c 6573  sambiguate_files
-000310c0: 2866 696c 6573 3a20 436f 6c6c 6563 7469  (files: Collecti
-000310d0: 6f6e 5b46 696c 655d 2c20 666e 616d 653a  on[File], fname:
-000310e0: 2073 7472 2c20 6669 6c65 5f74 7970 653a   str, file_type:
-000310f0: 2073 7472 2c20 6368 6f6f 7365 3a20 4c69   str, choose: Li
-00031100: 7465 7261 6c5b 2761 7574 6f27 2c20 2761  teral['auto', 'a
-00031110: 736b 275d 203d 2027 6175 746f 2729 202d  sk'] = 'auto') -
-00031120: 3e20 4f70 7469 6f6e 616c 5b46 696c 655d  > Optional[File]
-00031130: 3a0a 2020 2020 2222 2252 6563 6569 7665  :.    """Receive
-00031140: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
-00031150: 6620 3a6f 626a 3a60 4669 6c65 6020 7769  f :obj:`File` wi
-00031160: 7468 2074 6865 2061 696d 2074 6f20 7069  th the aim to pi
-00031170: 636b 206f 6e65 206f 6620 7468 656d 2e0a  ck one of them..
-00031180: 2020 2020 4669 7273 742c 2061 2064 6963      First, a dic
-00031190: 7469 6f6e 6172 7920 6973 2063 7265 6174  tionary is creat
-000311a0: 6564 2077 6865 7265 2074 6865 206b 6579  ed where the key
-000311b0: 7320 6172 6520 6469 7361 6d62 6967 7561  s are disambigua
-000311c0: 7469 6f6e 2073 7472 696e 6773 2062 6173  tion strings bas
-000311d0: 6564 206f 6e20 7468 6520 6669 6c65 7327  ed on the files'
-000311e0: 2070 6174 6873 2061 6e64 0a20 2020 2073   paths and.    s
-000311f0: 7566 6669 7865 732e 0a0a 2020 2020 4172  uffixes...    Ar
-00031200: 6773 3a0a 2020 2020 2020 6669 6c65 733a  gs:.      files:
-00031210: 0a20 2020 2020 2063 686f 6f73 653a 2049  .      choose: I
-00031220: 6620 2761 7574 6f27 2028 6465 6661 756c  f 'auto' (defaul
-00031230: 7429 2c20 7468 6520 6669 6c65 2077 6974  t), the file wit
-00031240: 6820 7468 6520 7368 6f72 7465 7374 2064  h the shortest d
-00031250: 6973 616d 6269 6775 6174 696f 6e20 7374  isambiguation st
-00031260: 7269 6e67 2069 7320 6368 6f73 656e 2e20  ring is chosen. 
-00031270: 5365 7420 746f 2054 7275 650a 2020 2020  Set to True.    
-00031280: 2020 2020 2020 6966 2079 6f75 2077 616e        if you wan
-00031290: 7420 746f 2062 6520 6173 6b65 6420 746f  t to be asked to
-000312a0: 206d 616e 7561 6c6c 7920 6368 6f6f 7365   manually choose
-000312b0: 2061 2066 696c 652e 0a0a 2020 2020 5265   a file...    Re
-000312c0: 7475 726e 733a 0a20 2020 2020 2054 6865  turns:.      The
-000312d0: 2073 656c 6563 7465 6420 6669 6c65 2e0a   selected file..
-000312e0: 2020 2020 2222 220a 2020 2020 6e5f 6669      """.    n_fi
-000312f0: 6c65 7320 3d20 6c65 6e28 6669 6c65 7329  les = len(files)
-00031300: 0a20 2020 2069 6620 6e5f 6669 6c65 7320  .    if n_files 
-00031310: 3d3d 2030 3a0a 2020 2020 2020 2020 7265  == 0:.        re
-00031320: 7475 726e 0a20 2020 2066 696c 6573 203d  turn.    files =
-00031330: 2074 7570 6c65 2866 696c 6573 290a 2020   tuple(files).  
-00031340: 2020 6966 206e 5f66 696c 6573 203d 3d20    if n_files == 
-00031350: 313a 0a20 2020 2020 2020 2072 6574 7572  1:.        retur
-00031360: 6e20 6669 6c65 735b 305d 0a20 2020 2069  n files[0].    i
-00031370: 6620 6368 6f6f 7365 206e 6f74 2069 6e20  f choose not in 
-00031380: 2827 6175 746f 272c 2027 6173 6b27 293a  ('auto', 'ask'):
-00031390: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-000313a0: 696e 666f 2866 2254 6865 2076 616c 7565  info(f"The value
-000313b0: 2066 6f72 2063 686f 6f73 6520 6e65 6564   for choose need
-000313c0: 7320 746f 2062 6520 2761 7574 6f27 206f  s to be 'auto' o
-000313d0: 7220 2761 736b 272c 206e 6f74 207b 6368  r 'ask', not {ch
-000313e0: 6f6f 7365 7d2e 2053 6574 7469 6e67 2074  oose}. Setting t
-000313f0: 6f20 2761 7574 6f27 2e22 290a 2020 2020  o 'auto'.").    
-00031400: 2020 2020 6368 6f6f 7365 203d 2027 6175      choose = 'au
-00031410: 746f 270a 2020 2020 6469 7361 6d62 6967  to'.    disambig
-00031420: 7561 7469 6f6e 5f64 6963 7420 3d20 6669  uation_dict = fi
-00031430: 6c65 7332 6469 7361 6d62 6967 7561 7469  les2disambiguati
-00031440: 6f6e 5f64 6963 7428 6669 6c65 732c 206c  on_dict(files, l
-00031450: 6f67 6765 723d 6c6f 6767 6572 290a 2020  ogger=logger).  
-00031460: 2020 6966 2063 686f 6f73 6520 3d3d 2027    if choose == '
-00031470: 6173 6b27 3a0a 2020 2020 2020 2020 7265  ask':.        re
-00031480: 7475 726e 2061 736b 5f75 7365 725f 746f  turn ask_user_to
-00031490: 5f63 686f 6f73 655f 6672 6f6d 5f64 6973  _choose_from_dis
-000314a0: 616d 6269 6775 6174 6564 5f66 696c 6573  ambiguated_files
-000314b0: 2864 6973 616d 6269 6775 6174 696f 6e5f  (disambiguation_
-000314c0: 6469 6374 2c20 666e 616d 652c 2066 696c  dict, fname, fil
-000314d0: 655f 7479 7065 290a 2020 2020 7265 7475  e_type).    retu
-000314e0: 726e 2061 7574 6f6d 6174 6963 616c 6c79  rn automatically
-000314f0: 5f63 686f 6f73 655f 6672 6f6d 5f64 6973  _choose_from_dis
-00031500: 616d 6269 6775 6174 6564 5f66 696c 6573  ambiguated_files
-00031510: 2864 6973 616d 6269 6775 6174 696f 6e5f  (disambiguation_
-00031520: 6469 6374 2c20 666e 616d 652c 2066 696c  dict, fname, fil
-00031530: 655f 7479 7065 2c20 6c6f 6767 6572 3d6c  e_type, logger=l
-00031540: 6f67 6765 7229 0a0a 2320 4066 756e 6374  ogger)..# @funct
-00031550: 696f 6e5f 6c6f 6767 6572 0a23 2064 6566  ion_logger.# def
-00031560: 2064 6973 616d 6269 6775 6174 655f 7061   disambiguate_pa
-00031570: 7273 6564 5f66 696c 6573 2874 7570 6c65  rsed_files(tuple
-00031580: 735f 7769 7468 5f66 696c 655f 6173 5f66  s_with_file_as_f
-00031590: 6972 7374 5f65 6c65 6d65 6e74 3a20 436f  irst_element: Co
-000315a0: 6c6c 6563 7469 6f6e 5b54 7570 6c65 5d2c  llection[Tuple],
-000315b0: 2066 6e61 6d65 3a20 7374 722c 2066 696c   fname: str, fil
-000315c0: 655f 7479 7065 3a20 7374 722c 2063 686f  e_type: str, cho
-000315d0: 6f73 653a 204c 6974 6572 616c 5b27 6175  ose: Literal['au
-000315e0: 746f 272c 2027 6173 6b27 5d20 3d20 2761  to', 'ask'] = 'a
-000315f0: 7574 6f27 2920 2d3e 204f 7074 696f 6e61  uto') -> Optiona
-00031600: 6c5b 4669 6c65 5d3a 0a23 2020 2020 2066  l[File]:.#     f
-00031610: 696c 6573 203d 205b 7475 705b 305d 2066  iles = [tup[0] f
-00031620: 6f72 2074 7570 2069 6e20 7475 706c 6573  or tup in tuples
-00031630: 5f77 6974 685f 6669 6c65 5f61 735f 6669  _with_file_as_fi
-00031640: 7273 745f 656c 656d 656e 745d 0a23 2020  rst_element].#  
-00031650: 2020 2073 656c 6563 7465 6420 3d20 6469     selected = di
-00031660: 7361 6d62 6967 7561 7465 5f66 696c 6573  sambiguate_files
-00031670: 2866 696c 6573 2c20 666e 616d 653d 666e  (files, fname=fn
-00031680: 616d 652c 2066 696c 655f 7479 7065 3d66  ame, file_type=f
-00031690: 696c 655f 7479 7065 2c20 6368 6f6f 7365  ile_type, choose
-000316a0: 3d63 686f 6f73 652c 206c 6f67 6765 723d  =choose, logger=
-000316b0: 6c6f 6767 6572 290a 2320 2020 2020 6966  logger).#     if
-000316c0: 2073 656c 6563 7465 6420 6973 204e 6f6e   selected is Non
-000316d0: 653a 0a23 2020 2020 2020 2020 2072 6574  e:.#         ret
-000316e0: 7572 6e0a 2320 2020 2020 666f 7220 7475  urn.#     for tu
-000316f0: 7020 696e 2074 7570 6c65 735f 7769 7468  p in tuples_with
-00031700: 5f66 696c 655f 6173 5f66 6972 7374 5f65  _file_as_first_e
-00031710: 6c65 6d65 6e74 3a0a 2320 2020 2020 2020  lement:.#       
-00031720: 2020 6966 2074 7570 5b30 5d20 3d3d 2073    if tup[0] == s
-00031730: 656c 6563 7465 643a 0a23 2020 2020 2020  elected:.#      
-00031740: 2020 2020 2020 2072 6574 7572 6e20 7475         return tu
-00031750: 700a 0a0a 4066 756e 6374 696f 6e5f 6c6f  p...@function_lo
-00031760: 6767 6572 0a64 6566 2066 696c 6573 3264  gger.def files2d
-00031770: 6973 616d 6269 6775 6174 696f 6e5f 6469  isambiguation_di
-00031780: 6374 2866 696c 6573 3a20 436f 6c6c 6563  ct(files: Collec
-00031790: 7469 6f6e 5b46 696c 655d 2c20 696e 636c  tion[File], incl
-000317a0: 7564 655f 6469 7361 6d62 6967 7561 746f  ude_disambiguato
-000317b0: 723a 2062 6f6f 6c20 3d20 4661 6c73 6529  r: bool = False)
-000317c0: 202d 3e20 4669 6c65 4469 6374 3a0a 2020   -> FileDict:.  
-000317d0: 2020 2222 2254 616b 6573 2061 206c 6973    """Takes a lis
-000317e0: 7420 6f66 203a 636c 6173 733a 6046 696c  t of :class:`Fil
-000317f0: 6560 2072 6574 7572 6e73 2061 2064 6963  e` returns a dic
-00031800: 7469 6f6e 6172 7920 7769 7468 2064 6973  tionary with dis
-00031810: 616d 6269 6775 6174 696e 6720 7374 7269  ambiguating stri
-00031820: 6e67 7320 6261 7365 6420 6f6e 2070 6174  ngs based on pat
-00031830: 6820 636f 6d70 6f6e 656e 7473 2e0a 2020  h components..  
-00031840: 2020 6f66 2064 6973 7469 6e63 7420 7374    of distinct st
-00031850: 7269 6e67 7320 746f 2064 6973 7469 6e67  rings to disting
-00031860: 7569 7368 2066 696c 6573 2070 6572 7461  uish files perta
-00031870: 696e 696e 6720 746f 2074 6865 2073 616d  ining to the sam
-00031880: 6520 7479 7065 2e22 2222 0a20 2020 206e  e type.""".    n
-00031890: 5f66 696c 6573 203d 206c 656e 2866 696c  _files = len(fil
-000318a0: 6573 290a 2020 2020 6966 206e 5f66 696c  es).    if n_fil
-000318b0: 6573 203d 3d20 303a 0a20 2020 2020 2020  es == 0:.       
-000318c0: 2072 6574 7572 6e20 7b7d 0a20 2020 2066   return {}.    f
-000318d0: 696c 6573 203d 2074 7570 6c65 2866 696c  iles = tuple(fil
-000318e0: 6573 290a 2020 2020 6966 206e 5f66 696c  es).    if n_fil
-000318f0: 6573 3d3d 2031 3a0a 2020 2020 2020 2020  es== 1:.        
-00031900: 6620 3d20 6669 6c65 735b 305d 0a20 2020  f = files[0].   
-00031910: 2020 2020 2072 6574 7572 6e20 7b66 2e74       return {f.t
-00031920: 7970 653a 2066 7d0a 2020 2020 6469 7361  ype: f}.    disa
-00031930: 6d62 6967 7561 7469 6f6e 203d 205b 662e  mbiguation = [f.
-00031940: 7479 7065 2066 6f72 2066 2069 6e20 6669  type for f in fi
-00031950: 6c65 735d 0a20 2020 2069 6620 6c65 6e28  les].    if len(
-00031960: 7365 7428 6469 7361 6d62 6967 7561 7469  set(disambiguati
-00031970: 6f6e 2929 203d 3d20 6e5f 6669 6c65 733a  on)) == n_files:
-00031980: 0a20 2020 2020 2020 2023 2064 6f6e 6520  .        # done 
-00031990: 6469 7361 6d62 6967 7561 7469 6e67 0a20  disambiguating. 
-000319a0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-000319b0: 6374 287a 6970 2864 6973 616d 6269 6775  ct(zip(disambigu
-000319c0: 6174 696f 6e2c 2066 696c 6573 2929 0a20  ation, files)). 
-000319d0: 2020 2069 6620 696e 636c 7564 655f 6469     if include_di
-000319e0: 7361 6d62 6967 7561 746f 7220 616e 6420  sambiguator and 
-000319f0: 6c65 6e28 7365 7428 6469 7361 6d62 6967  len(set(disambig
-00031a00: 7561 7469 6f6e 2929 203e 2031 3a0a 2020  uation)) > 1:.  
-00031a10: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-00031a20: 6e69 6e67 2866 2249 6e63 6c75 6469 6e67  ning(f"Including
-00031a30: 2074 6865 2064 6973 616d 6269 6775 6174   the disambiguat
-00031a40: 6f72 2072 656d 6f76 6573 2074 6865 2066  or removes the f
-00031a50: 6163 6574 206e 616d 652c 2062 7574 2074  acet name, but t
-00031a60: 6865 2066 696c 6573 2070 6572 7461 696e  he files pertain
-00031a70: 2074 6f20 220a 2020 2020 2020 2020 2020   to ".          
-00031a80: 2020 2020 2020 2020 2020 2066 2273 6576             f"sev
-00031a90: 6572 616c 2066 6163 6574 733a 207b 7365  eral facets: {se
-00031aa0: 7428 6469 7361 6d62 6967 7561 7469 6f6e  t(disambiguation
-00031ab0: 297d 2229 0a20 2020 2023 2066 6972 7374  )}").    # first
-00031ac0: 2c20 7472 7920 746f 2064 6973 616d 6269  , try to disambi
-00031ad0: 6775 6174 6520 6261 7365 6420 6f6e 2074  guate based on t
-00031ae0: 6865 2066 696c 6573 2720 7375 622d 6469  he files' sub-di
-00031af0: 7265 6374 6f72 6965 730a 2020 2020 7375  rectories.    su
-00031b00: 6264 6972 7320 3d20 5b5d 0a20 2020 2066  bdirs = [].    f
-00031b10: 6f72 2066 2069 6e20 6669 6c65 733a 0a20  or f in files:. 
-00031b20: 2020 2020 2020 2066 696c 655f 7479 7065         file_type
-00031b30: 203d 2066 2e74 7970 650a 2020 2020 2020   = f.type.      
-00031b40: 2020 7375 6264 6972 203d 2066 2e73 7562    subdir = f.sub
-00031b50: 6469 722e 7374 7269 7028 7222 5c2f 2e22  dir.strip(r"\/."
-00031b60: 290a 2020 2020 2020 2020 6966 2073 7562  ).        if sub
-00031b70: 6469 722e 7374 6172 7473 7769 7468 2866  dir.startswith(f
-00031b80: 696c 655f 7479 7065 293a 0a20 2020 2020  ile_type):.     
-00031b90: 2020 2020 2020 2073 7562 6469 7220 3d20         subdir = 
-00031ba0: 7375 6264 6972 5b6c 656e 2866 696c 655f  subdir[len(file_
-00031bb0: 7479 7065 293a 5d0a 2020 2020 2020 2020  type):].        
-00031bc0: 6966 2073 7562 6469 722e 7374 7269 7028  if subdir.strip(
-00031bd0: 7222 5c2f 2229 203d 3d20 2727 3a0a 2020  r"\/") == '':.  
-00031be0: 2020 2020 2020 2020 2020 7375 6264 6972            subdir
-00031bf0: 203d 2027 270a 2020 2020 2020 2020 7375   = ''.        su
-00031c00: 6264 6972 732e 6170 7065 6e64 2873 7562  bdirs.append(sub
-00031c10: 6469 7229 0a20 2020 2069 6620 6c65 6e28  dir).    if len(
-00031c20: 7365 7428 7375 6264 6972 7329 2920 3e20  set(subdirs)) > 
-00031c30: 313a 0a20 2020 2020 2020 2023 2066 696c  1:.        # fil
-00031c40: 6573 2063 616e 2028 7061 7274 6961 6c6c  es can (partiall
-00031c50: 7929 2062 6520 6469 7361 6d62 6967 7561  y) be disambigua
-00031c60: 7465 6420 6265 6361 7573 6520 7468 6579  ted because they
-00031c70: 2061 7265 2069 6e20 6469 6666 6572 656e   are in differen
-00031c80: 7420 7375 622d 6469 7265 6374 6f72 6965  t sub-directorie
-00031c90: 730a 2020 2020 2020 2020 6966 2069 6e63  s.        if inc
-00031ca0: 6c75 6465 5f64 6973 616d 6269 6775 6174  lude_disambiguat
-00031cb0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00031cc0: 6469 7361 6d62 6967 7561 7469 6f6e 203d  disambiguation =
-00031cd0: 205b 6622 7375 6264 6972 3a20 7b27 2e27   [f"subdir: {'.'
-00031ce0: 2069 6620 7375 6264 6972 203d 3d20 2727   if subdir == ''
-00031cf0: 2065 6c73 6520 7375 6264 6972 7d22 2066   else subdir}" f
-00031d00: 6f72 2064 6973 616d 622c 2073 7562 6469  or disamb, subdi
-00031d10: 7220 696e 207a 6970 2864 6973 616d 6269  r in zip(disambi
-00031d20: 6775 6174 696f 6e2c 2073 7562 6469 7273  guation, subdirs
-00031d30: 295d 0a20 2020 2020 2020 2065 6c73 653a  )].        else:
-00031d40: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00031d50: 616d 6269 6775 6174 696f 6e20 3d20 5b6f  ambiguation = [o
-00031d60: 732e 7061 7468 2e6a 6f69 6e28 6469 7361  s.path.join(disa
-00031d70: 6d62 2c20 7375 6264 6972 2920 666f 7220  mb, subdir) for 
-00031d80: 6469 7361 6d62 2c20 7375 6264 6972 2069  disamb, subdir i
-00031d90: 6e20 7a69 7028 6469 7361 6d62 6967 7561  n zip(disambigua
-00031da0: 7469 6f6e 2c20 7375 6264 6972 7329 5d0a  tion, subdirs)].
-00031db0: 2020 2020 6966 206c 656e 2873 6574 2864      if len(set(d
-00031dc0: 6973 616d 6269 6775 6174 696f 6e29 2920  isambiguation)) 
-00031dd0: 3d3d 206e 5f66 696c 6573 3a0a 2020 2020  == n_files:.    
-00031de0: 2020 2020 2320 646f 6e65 2064 6973 616d      # done disam
-00031df0: 6269 6775 6174 696e 670a 2020 2020 2020  biguating.      
-00031e00: 2020 7265 7475 726e 2064 6963 7428 7a69    return dict(zi
-00031e10: 7028 6469 7361 6d62 6967 7561 7469 6f6e  p(disambiguation
-00031e20: 2c20 6669 6c65 7329 290a 2020 2020 2320  , files)).    # 
-00031e30: 6e65 7874 2c20 7472 7920 6164 6469 6e67  next, try adding
-00031e40: 2064 6574 6563 7465 6420 7375 6666 6978   detected suffix
-00031e50: 6573 0a20 2020 2066 6f72 2069 782c 2066  es.    for ix, f
-00031e60: 2069 6e20 656e 756d 6572 6174 6528 6669   in enumerate(fi
-00031e70: 6c65 7329 3a0a 2020 2020 2020 2020 6966  les):.        if
-00031e80: 2066 2e73 7566 6669 7820 213d 2027 273a   f.suffix != '':
-00031e90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00031ea0: 696e 636c 7564 655f 6469 7361 6d62 6967  include_disambig
-00031eb0: 7561 746f 723a 0a20 2020 2020 2020 2020  uator:.         
-00031ec0: 2020 2020 2020 2064 6973 616d 6269 6775         disambigu
-00031ed0: 6174 696f 6e5b 6978 5d20 2b3d 2066 222c  ation[ix] += f",
-00031ee0: 2073 7566 6669 783a 207b 662e 7375 6666   suffix: {f.suff
-00031ef0: 6978 7d22 0a20 2020 2020 2020 2020 2020  ix}".           
-00031f00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00031f10: 2020 2020 2020 2064 6973 616d 6269 6775         disambigu
-00031f20: 6174 696f 6e5b 6978 5d20 2b3d 2066 225b  ation[ix] += f"[
-00031f30: 7b66 2e73 7566 6669 787d 5d22 0a20 2020  {f.suffix}]".   
-00031f40: 2069 6620 6c65 6e28 7365 7428 6469 7361   if len(set(disa
-00031f50: 6d62 6967 7561 7469 6f6e 2929 203d 3d20  mbiguation)) == 
-00031f60: 6e5f 6669 6c65 733a 0a20 2020 2020 2020  n_files:.       
-00031f70: 2023 2064 6f6e 6520 6469 7361 6d62 6967   # done disambig
-00031f80: 7561 7469 6e67 0a20 2020 2020 2020 2072  uating.        r
-00031f90: 6574 7572 6e20 6469 6374 287a 6970 2864  eturn dict(zip(d
-00031fa0: 6973 616d 6269 6775 6174 696f 6e2c 2066  isambiguation, f
-00031fb0: 696c 6573 2929 0a20 2020 2023 206e 6f77  iles)).    # now
-00031fc0: 2c20 6164 6420 6669 6c65 2065 7874 656e  , add file exten
-00031fd0: 7369 6f6e 7320 746f 2064 6973 616d 6269  sions to disambi
-00031fe0: 6775 6174 6520 6675 7274 6865 720a 2020  guate further.  
-00031ff0: 2020 6966 206c 656e 2873 6574 2866 2e66    if len(set(f.f
-00032000: 6578 7420 666f 7220 6620 696e 2066 696c  ext for f in fil
-00032010: 6573 2929 203e 2031 3a0a 2020 2020 2020  es)) > 1:.      
-00032020: 2020 666f 7220 6978 2c20 6620 696e 2065    for ix, f in e
-00032030: 6e75 6d65 7261 7465 2866 696c 6573 293a  numerate(files):
-00032040: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00032050: 696e 636c 7564 655f 6469 7361 6d62 6967  include_disambig
-00032060: 7561 746f 723a 0a20 2020 2020 2020 2020  uator:.         
-00032070: 2020 2020 2020 2064 6973 616d 6269 6775         disambigu
-00032080: 6174 696f 6e5b 6978 5d20 2b3d 2066 222c  ation[ix] += f",
-00032090: 2066 6578 743a 207b 662e 6665 7874 7d22   fext: {f.fext}"
-000320a0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000320b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000320c0: 2020 2064 6973 616d 6269 6775 6174 696f     disambiguatio
-000320d0: 6e5b 6978 5d20 2b3d 2066 2e66 6578 740a  n[ix] += f.fext.
-000320e0: 2020 2020 6966 206c 656e 2873 6574 2864      if len(set(d
-000320f0: 6973 616d 6269 6775 6174 696f 6e29 2920  isambiguation)) 
-00032100: 3d3d 206e 5f66 696c 6573 3a0a 2020 2020  == n_files:.    
-00032110: 2020 2020 2320 646f 6e65 2064 6973 616d      # done disam
-00032120: 6269 6775 6174 696e 670a 2020 2020 2020  biguating.      
-00032130: 2020 7265 7475 726e 2064 6963 7428 7a69    return dict(zi
-00032140: 7028 6469 7361 6d62 6967 7561 7469 6f6e  p(disambiguation
-00032150: 2c20 6669 6c65 7329 290a 2020 2020 7374  , files)).    st
-00032160: 725f 636f 756e 7473 203d 2043 6f75 6e74  r_counts = Count
-00032170: 6572 2864 6973 616d 6269 6775 6174 696f  er(disambiguatio
-00032180: 6e29 0a20 2020 2064 7570 6c69 6361 7465  n).    duplicate
-00032190: 5f64 6973 616d 6269 6775 6174 696f 6e5f  _disambiguation_
-000321a0: 7374 7269 6e67 7320 3d20 5b73 2066 6f72  strings = [s for
-000321b0: 2073 2c20 636e 7420 696e 2073 7472 5f63   s, cnt in str_c
-000321c0: 6f75 6e74 732e 6974 656d 7328 2920 6966  ounts.items() if
-000321d0: 2063 6e74 203e 2031 5d0a 2020 2020 616d   cnt > 1].    am
-000321e0: 6269 6775 6174 655f 6669 6c65 7320 3d20  biguate_files = 
-000321f0: 7b73 3a20 5b66 2066 6f72 2064 6973 616d  {s: [f for disam
-00032200: 622c 2066 2069 6e20 7a69 7028 6469 7361  b, f in zip(disa
-00032210: 6d62 6967 7561 7469 6f6e 2c20 6669 6c65  mbiguation, file
-00032220: 7329 2069 6620 6469 7361 6d62 203d 3d20  s) if disamb == 
-00032230: 735d 2066 6f72 2073 2069 6e20 6475 706c  s] for s in dupl
-00032240: 6963 6174 655f 6469 7361 6d62 6967 7561  icate_disambigua
-00032250: 7469 6f6e 5f73 7472 696e 6773 7d0a 2020  tion_strings}.  
-00032260: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00032270: 7a69 7028 6469 7361 6d62 6967 7561 7469  zip(disambiguati
-00032280: 6f6e 2c20 6669 6c65 7329 290a 2020 2020  on, files)).    
-00032290: 7265 6d61 696e 696e 675f 6f6e 6573 203d  remaining_ones =
-000322a0: 207b 733a 2072 6573 756c 745b 735d 2066   {s: result[s] f
-000322b0: 6f72 2073 2069 6e20 6475 706c 6963 6174  or s in duplicat
-000322c0: 655f 6469 7361 6d62 6967 7561 7469 6f6e  e_disambiguation
-000322d0: 5f73 7472 696e 6773 7d0a 2020 2020 6c6f  _strings}.    lo
-000322e0: 6767 6572 2e77 6172 6e69 6e67 2866 2254  gger.warning(f"T
-000322f0: 6865 2066 6f6c 6c6f 7769 6e67 2066 696c  he following fil
-00032300: 6573 2063 6f75 6c64 206e 6f74 2062 6520  es could not be 
-00032310: 616d 6269 6775 6174 6564 3a20 7b61 6d62  ambiguated: {amb
-00032320: 6967 7561 7465 5f66 696c 6573 7d2e 5c6e  iguate_files}.\n
-00032330: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00032340: 2020 2020 2066 2249 6e20 7468 6520 7265       f"In the re
-00032350: 7375 6c74 2c20 6f6e 6c79 2074 6865 7365  sult, only these
-00032360: 2072 656d 6169 6e3a 207b 7265 6d61 696e   remain: {remain
-00032370: 696e 675f 6f6e 6573 7d2e 2229 0a20 2020  ing_ones}.").   
-00032380: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00032390: 0a64 6566 206c 6974 6572 616c 5f74 7970  .def literal_typ
-000323a0: 6532 7475 706c 6528 7479 703a 2054 7970  e2tuple(typ: Typ
-000323b0: 6556 6172 2920 2d3e 2054 7570 6c65 5b73  eVar) -> Tuple[s
-000323c0: 7472 5d3a 0a20 2020 2022 2222 5475 726e  tr]:.    """Turn
-000323d0: 7320 7468 6520 6669 7273 7420 4c69 7465  s the first Lite
-000323e0: 7261 6c20 696e 636c 7564 6564 2069 6e20  ral included in 
-000323f0: 7468 6520 5479 7065 5661 7220 696e 746f  the TypeVar into
-00032400: 2061 206c 6973 7420 6f66 2076 616c 7565   a list of value
-00032410: 732e 2054 6865 2066 6972 7374 206c 6974  s. The first lit
-00032420: 6572 616c 2076 616c 7565 0a20 2020 206e  eral value.    n
-00032430: 6565 6473 2074 6f20 6265 2061 2073 7472  eeds to be a str
-00032440: 696e 672c 206f 7468 6572 7769 7365 2074  ing, otherwise t
-00032450: 6865 2066 756e 6374 696f 6e20 6d61 7920  he function may 
-00032460: 6c65 6164 2074 6f20 756e 6578 7065 6374  lead to unexpect
-00032470: 6564 2062 6568 6176 696f 7572 2e0a 2020  ed behaviour..  
-00032480: 2020 2222 220a 2020 2020 6966 2069 7369    """.    if isi
-00032490: 6e73 7461 6e63 6528 7479 702e 5f5f 6172  nstance(typ.__ar
-000324a0: 6773 5f5f 5b30 5d2c 2073 7472 293a 0a20  gs__[0], str):. 
-000324b0: 2020 2020 2020 2072 6574 7572 6e20 7479         return ty
-000324c0: 702e 5f5f 6172 6773 5f5f 0a20 2020 2072  p.__args__.    r
-000324d0: 6574 7572 6e20 6c69 7465 7261 6c5f 7479  eturn literal_ty
-000324e0: 7065 3274 7570 6c65 2874 7970 2e5f 5f61  pe2tuple(typ.__a
-000324f0: 7267 735f 5f5b 305d 290a 0a0a 406c 7275  rgs__[0])...@lru
-00032500: 5f63 6163 6865 0a40 6675 6e63 7469 6f6e  _cache.@function
-00032510: 5f6c 6f67 6765 720a 6465 6620 6172 6775  _logger.def argu
-00032520: 6d65 6e74 5f61 6e64 5f6c 6974 6572 616c  ment_and_literal
-00032530: 5f74 7970 6532 6c69 7374 2861 7267 756d  _type2list(argum
-00032540: 656e 743a 2055 6e69 6f6e 5b73 7472 2c20  ent: Union[str, 
-00032550: 5475 706c 655b 7374 725d 2c20 4c69 7465  Tuple[str], Lite
-00032560: 7261 6c5b 4e6f 6e65 5d5d 2c0a 2020 2020  ral[None]],.    
-00032570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032580: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00032590: 7970 3a20 4f70 7469 6f6e 616c 5b55 6e69  yp: Optional[Uni
-000325a0: 6f6e 5b54 7970 6556 6172 2c20 5475 706c  on[TypeVar, Tupl
-000325b0: 655b 7374 725d 5d5d 203d 204e 6f6e 652c  e[str]]] = None,
-000325c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000325d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000325e0: 2020 2020 6e6f 6e65 5f6d 6561 6e73 5f61      none_means_a
-000325f0: 6c6c 3a20 626f 6f6c 203d 2054 7275 652c  ll: bool = True,
-00032600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030d10: 2020 2020 2066 6e61 6d65 3a20 7374 722c       fname: str,
+00030d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030d50: 2066 696c 655f 7479 7065 3a20 7374 7220   file_type: str 
+00030d60: 3d20 2727 2920 2d3e 204f 7074 696f 6e61  = '') -> Optiona
+00030d70: 6c5b 4669 6c65 5d3a 0a20 2020 2073 6f72  l[File]:.    sor
+00030d80: 7465 645f 6b65 7973 203d 2073 6f72 7465  ted_keys = sorte
+00030d90: 6428 6469 7361 6d62 6967 7561 7465 645f  d(disambiguated_
+00030da0: 6368 6f69 6365 732e 6b65 7973 2829 2c20  choices.keys(), 
+00030db0: 6b65 793d 6c61 6d62 6461 2073 3a20 286c  key=lambda s: (l
+00030dc0: 656e 2873 292c 2073 2929 0a20 2020 2064  en(s), s)).    d
+00030dd0: 6973 616d 6269 6775 6174 6564 5f63 686f  isambiguated_cho
+00030de0: 6963 6573 203d 207b 6b3a 2064 6973 616d  ices = {k: disam
+00030df0: 6269 6775 6174 6564 5f63 686f 6963 6573  biguated_choices
+00030e00: 5b6b 5d20 666f 7220 6b20 696e 2073 6f72  [k] for k in sor
+00030e10: 7465 645f 6b65 7973 7d0a 2020 2020 6669  ted_keys}.    fi
+00030e20: 6c65 5f6c 6973 7420 3d20 6c69 7374 2864  le_list = list(d
+00030e30: 6973 616d 6269 6775 6174 6564 5f63 686f  isambiguated_cho
+00030e40: 6963 6573 2e76 616c 7565 7328 2929 0a20  ices.values()). 
+00030e50: 2020 2064 6973 616d 625f 7374 7269 6e67     disamb_string
+00030e60: 7320 3d20 7064 2e53 6572 6965 7328 6469  s = pd.Series(di
+00030e70: 7361 6d62 6967 7561 7465 645f 6368 6f69  sambiguated_choi
+00030e80: 6365 732e 6b65 7973 2829 2c20 6e61 6d65  ces.keys(), name
+00030e90: 3d27 6469 7361 6d62 6967 7561 7469 6f6e  ='disambiguation
+00030ea0: 5f73 7472 2729 0a20 2020 2063 686f 6963  _str').    choic
+00030eb0: 6573 5f64 6620 3d20 7064 2e63 6f6e 6361  es_df = pd.conca
+00030ec0: 7428 5b64 6973 616d 625f 7374 7269 6e67  t([disamb_string
+00030ed0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00030ee0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00030ef0: 642e 4461 7461 4672 616d 6528 6669 6c65  d.DataFrame(file
+00030f00: 5f6c 6973 7429 5b5b 2772 656c 5f70 6174  _list)[['rel_pat
+00030f10: 6827 2c20 2774 7970 6527 2c20 2769 7827  h', 'type', 'ix'
+00030f20: 5d5d 5d2c 0a20 2020 2020 2020 2020 2020  ]]],.           
+00030f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030f40: 6178 6973 3d31 290a 2020 2020 6368 6f69  axis=1).    choi
+00030f50: 6365 735f 6466 2e69 6e64 6578 203d 2070  ces_df.index = p
+00030f60: 642e 496e 6465 7828 7261 6e67 6528 312c  d.Index(range(1,
+00030f70: 206c 656e 2866 696c 655f 6c69 7374 2920   len(file_list) 
+00030f80: 2b20 3129 2c20 6e61 6d65 3d27 7365 6c65  + 1), name='sele
+00030f90: 6374 3a27 290a 2020 2020 7261 6e67 655f  ct:').    range_
+00030fa0: 7374 7220 3d20 6622 312d 7b6c 656e 2864  str = f"1-{len(d
+00030fb0: 6973 616d 6269 6775 6174 6564 5f63 686f  isambiguated_cho
+00030fc0: 6963 6573 297d 220a 2020 2020 7175 6572  ices)}".    quer
+00030fd0: 7920 3d20 6622 5365 6c65 6374 696f 6e20  y = f"Selection 
+00030fe0: 5b7b 7261 6e67 655f 7374 727d 5d3a 2022  [{range_str}]: "
+00030ff0: 0a20 2020 2070 7269 6e74 2866 2253 6576  .    print(f"Sev
+00031000: 6572 616c 2027 7b66 696c 655f 7479 7065  eral '{file_type
+00031010: 7d27 2061 7661 696c 6162 6c65 2066 6f72  }' available for
+00031020: 2027 7b66 6e61 6d65 7d27 3a5c 6e7b 6368   '{fname}':\n{ch
+00031030: 6f69 6365 735f 6466 2e74 6f5f 7374 7269  oices_df.to_stri
+00031040: 6e67 2829 7d22 290a 2020 2020 7072 696e  ng()}").    prin
+00031050: 7428 6622 506c 6561 7365 2073 656c 6563  t(f"Please selec
+00031060: 7420 6f6e 6520 6f66 2074 6865 2066 696c  t one of the fil
+00031070: 6573 2062 7920 7061 7373 696e 6720 616e  es by passing an
+00031080: 2069 6e74 6567 6572 2062 6574 7765 656e   integer between
+00031090: 207b 7261 6e67 655f 7374 727d 2028 6f72   {range_str} (or
+000310a0: 2030 2066 6f72 206e 6f6e 6529 3a22 290a   0 for none):").
+000310b0: 2020 2020 7265 7475 726e 2061 736b 5f75      return ask_u
+000310c0: 7365 725f 746f 5f63 686f 6f73 6528 7175  ser_to_choose(qu
+000310d0: 6572 792c 2066 696c 655f 6c69 7374 290a  ery, file_list).
+000310e0: 0a0a 4066 756e 6374 696f 6e5f 6c6f 6767  ..@function_logg
+000310f0: 6572 0a64 6566 2064 6973 616d 6269 6775  er.def disambigu
+00031100: 6174 655f 6669 6c65 7328 6669 6c65 733a  ate_files(files:
+00031110: 2043 6f6c 6c65 6374 696f 6e5b 4669 6c65   Collection[File
+00031120: 5d2c 2066 6e61 6d65 3a20 7374 722c 2066  ], fname: str, f
+00031130: 696c 655f 7479 7065 3a20 7374 722c 2063  ile_type: str, c
+00031140: 686f 6f73 653a 204c 6974 6572 616c 5b27  hoose: Literal['
+00031150: 6175 746f 272c 2027 6173 6b27 5d20 3d20  auto', 'ask'] = 
+00031160: 2761 7574 6f27 2920 2d3e 204f 7074 696f  'auto') -> Optio
+00031170: 6e61 6c5b 4669 6c65 5d3a 0a20 2020 2022  nal[File]:.    "
+00031180: 2222 5265 6365 6976 6573 2061 2063 6f6c  ""Receives a col
+00031190: 6c65 6374 696f 6e20 6f66 203a 6f62 6a3a  lection of :obj:
+000311a0: 6046 696c 6560 2077 6974 6820 7468 6520  `File` with the 
+000311b0: 6169 6d20 746f 2070 6963 6b20 6f6e 6520  aim to pick one 
+000311c0: 6f66 2074 6865 6d2e 0a20 2020 2046 6972  of them..    Fir
+000311d0: 7374 2c20 6120 6469 6374 696f 6e61 7279  st, a dictionary
+000311e0: 2069 7320 6372 6561 7465 6420 7768 6572   is created wher
+000311f0: 6520 7468 6520 6b65 7973 2061 7265 2064  e the keys are d
+00031200: 6973 616d 6269 6775 6174 696f 6e20 7374  isambiguation st
+00031210: 7269 6e67 7320 6261 7365 6420 6f6e 2074  rings based on t
+00031220: 6865 2066 696c 6573 2720 7061 7468 7320  he files' paths 
+00031230: 616e 640a 2020 2020 7375 6666 6978 6573  and.    suffixes
+00031240: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00031250: 2020 2066 696c 6573 3a0a 2020 2020 2020     files:.      
+00031260: 6368 6f6f 7365 3a20 4966 2027 6175 746f  choose: If 'auto
+00031270: 2720 2864 6566 6175 6c74 292c 2074 6865  ' (default), the
+00031280: 2066 696c 6520 7769 7468 2074 6865 2073   file with the s
+00031290: 686f 7274 6573 7420 6469 7361 6d62 6967  hortest disambig
+000312a0: 7561 7469 6f6e 2073 7472 696e 6720 6973  uation string is
+000312b0: 2063 686f 7365 6e2e 2053 6574 2074 6f20   chosen. Set to 
+000312c0: 5472 7565 0a20 2020 2020 2020 2020 2069  True.          i
+000312d0: 6620 796f 7520 7761 6e74 2074 6f20 6265  f you want to be
+000312e0: 2061 736b 6564 2074 6f20 6d61 6e75 616c   asked to manual
+000312f0: 6c79 2063 686f 6f73 6520 6120 6669 6c65  ly choose a file
+00031300: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
+00031310: 2020 2020 2020 5468 6520 7365 6c65 6374        The select
+00031320: 6564 2066 696c 652e 0a20 2020 2022 2222  ed file..    """
+00031330: 0a20 2020 206e 5f66 696c 6573 203d 206c  .    n_files = l
+00031340: 656e 2866 696c 6573 290a 2020 2020 6966  en(files).    if
+00031350: 206e 5f66 696c 6573 203d 3d20 303a 0a20   n_files == 0:. 
+00031360: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00031370: 2020 6669 6c65 7320 3d20 7475 706c 6528    files = tuple(
+00031380: 6669 6c65 7329 0a20 2020 2069 6620 6e5f  files).    if n_
+00031390: 6669 6c65 7320 3d3d 2031 3a0a 2020 2020  files == 1:.    
+000313a0: 2020 2020 7265 7475 726e 2066 696c 6573      return files
+000313b0: 5b30 5d0a 2020 2020 6966 2063 686f 6f73  [0].    if choos
+000313c0: 6520 6e6f 7420 696e 2028 2761 7574 6f27  e not in ('auto'
+000313d0: 2c20 2761 736b 2729 3a0a 2020 2020 2020  , 'ask'):.      
+000313e0: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
+000313f0: 5468 6520 7661 6c75 6520 666f 7220 6368  The value for ch
+00031400: 6f6f 7365 206e 6565 6473 2074 6f20 6265  oose needs to be
+00031410: 2027 6175 746f 2720 6f72 2027 6173 6b27   'auto' or 'ask'
+00031420: 2c20 6e6f 7420 7b63 686f 6f73 657d 2e20  , not {choose}. 
+00031430: 5365 7474 696e 6720 746f 2027 6175 746f  Setting to 'auto
+00031440: 272e 2229 0a20 2020 2020 2020 2063 686f  '.").        cho
+00031450: 6f73 6520 3d20 2761 7574 6f27 0a20 2020  ose = 'auto'.   
+00031460: 2064 6973 616d 6269 6775 6174 696f 6e5f   disambiguation_
+00031470: 6469 6374 203d 2066 696c 6573 3264 6973  dict = files2dis
+00031480: 616d 6269 6775 6174 696f 6e5f 6469 6374  ambiguation_dict
+00031490: 2866 696c 6573 2c20 6c6f 6767 6572 3d6c  (files, logger=l
+000314a0: 6f67 6765 7229 0a20 2020 2069 6620 6368  ogger).    if ch
+000314b0: 6f6f 7365 203d 3d20 2761 736b 273a 0a20  oose == 'ask':. 
+000314c0: 2020 2020 2020 2072 6574 7572 6e20 6173         return as
+000314d0: 6b5f 7573 6572 5f74 6f5f 6368 6f6f 7365  k_user_to_choose
+000314e0: 5f66 726f 6d5f 6469 7361 6d62 6967 7561  _from_disambigua
+000314f0: 7465 645f 6669 6c65 7328 6469 7361 6d62  ted_files(disamb
+00031500: 6967 7561 7469 6f6e 5f64 6963 742c 2066  iguation_dict, f
+00031510: 6e61 6d65 2c20 6669 6c65 5f74 7970 6529  name, file_type)
+00031520: 0a20 2020 2072 6574 7572 6e20 6175 746f  .    return auto
+00031530: 6d61 7469 6361 6c6c 795f 6368 6f6f 7365  matically_choose
+00031540: 5f66 726f 6d5f 6469 7361 6d62 6967 7561  _from_disambigua
+00031550: 7465 645f 6669 6c65 7328 6469 7361 6d62  ted_files(disamb
+00031560: 6967 7561 7469 6f6e 5f64 6963 742c 2066  iguation_dict, f
+00031570: 6e61 6d65 2c20 6669 6c65 5f74 7970 652c  name, file_type,
+00031580: 206c 6f67 6765 723d 6c6f 6767 6572 290a   logger=logger).
+00031590: 0a23 2040 6675 6e63 7469 6f6e 5f6c 6f67  .# @function_log
+000315a0: 6765 720a 2320 6465 6620 6469 7361 6d62  ger.# def disamb
+000315b0: 6967 7561 7465 5f70 6172 7365 645f 6669  iguate_parsed_fi
+000315c0: 6c65 7328 7475 706c 6573 5f77 6974 685f  les(tuples_with_
+000315d0: 6669 6c65 5f61 735f 6669 7273 745f 656c  file_as_first_el
+000315e0: 656d 656e 743a 2043 6f6c 6c65 6374 696f  ement: Collectio
+000315f0: 6e5b 5475 706c 655d 2c20 666e 616d 653a  n[Tuple], fname:
+00031600: 2073 7472 2c20 6669 6c65 5f74 7970 653a   str, file_type:
+00031610: 2073 7472 2c20 6368 6f6f 7365 3a20 4c69   str, choose: Li
+00031620: 7465 7261 6c5b 2761 7574 6f27 2c20 2761  teral['auto', 'a
+00031630: 736b 275d 203d 2027 6175 746f 2729 202d  sk'] = 'auto') -
+00031640: 3e20 4f70 7469 6f6e 616c 5b46 696c 655d  > Optional[File]
+00031650: 3a0a 2320 2020 2020 6669 6c65 7320 3d20  :.#     files = 
+00031660: 5b74 7570 5b30 5d20 666f 7220 7475 7020  [tup[0] for tup 
+00031670: 696e 2074 7570 6c65 735f 7769 7468 5f66  in tuples_with_f
+00031680: 696c 655f 6173 5f66 6972 7374 5f65 6c65  ile_as_first_ele
+00031690: 6d65 6e74 5d0a 2320 2020 2020 7365 6c65  ment].#     sele
+000316a0: 6374 6564 203d 2064 6973 616d 6269 6775  cted = disambigu
+000316b0: 6174 655f 6669 6c65 7328 6669 6c65 732c  ate_files(files,
+000316c0: 2066 6e61 6d65 3d66 6e61 6d65 2c20 6669   fname=fname, fi
+000316d0: 6c65 5f74 7970 653d 6669 6c65 5f74 7970  le_type=file_typ
+000316e0: 652c 2063 686f 6f73 653d 6368 6f6f 7365  e, choose=choose
+000316f0: 2c20 6c6f 6767 6572 3d6c 6f67 6765 7229  , logger=logger)
+00031700: 0a23 2020 2020 2069 6620 7365 6c65 6374  .#     if select
+00031710: 6564 2069 7320 4e6f 6e65 3a0a 2320 2020  ed is None:.#   
+00031720: 2020 2020 2020 7265 7475 726e 0a23 2020        return.#  
+00031730: 2020 2066 6f72 2074 7570 2069 6e20 7475     for tup in tu
+00031740: 706c 6573 5f77 6974 685f 6669 6c65 5f61  ples_with_file_a
+00031750: 735f 6669 7273 745f 656c 656d 656e 743a  s_first_element:
+00031760: 0a23 2020 2020 2020 2020 2069 6620 7475  .#         if tu
+00031770: 705b 305d 203d 3d20 7365 6c65 6374 6564  p[0] == selected
+00031780: 3a0a 2320 2020 2020 2020 2020 2020 2020  :.#             
+00031790: 7265 7475 726e 2074 7570 0a0a 0a40 6675  return tup...@fu
+000317a0: 6e63 7469 6f6e 5f6c 6f67 6765 720a 6465  nction_logger.de
+000317b0: 6620 6669 6c65 7332 6469 7361 6d62 6967  f files2disambig
+000317c0: 7561 7469 6f6e 5f64 6963 7428 6669 6c65  uation_dict(file
+000317d0: 733a 2043 6f6c 6c65 6374 696f 6e5b 4669  s: Collection[Fi
+000317e0: 6c65 5d2c 2069 6e63 6c75 6465 5f64 6973  le], include_dis
+000317f0: 616d 6269 6775 6174 6f72 3a20 626f 6f6c  ambiguator: bool
+00031800: 203d 2046 616c 7365 2920 2d3e 2046 696c   = False) -> Fil
+00031810: 6544 6963 743a 0a20 2020 2022 2222 5461  eDict:.    """Ta
+00031820: 6b65 7320 6120 6c69 7374 206f 6620 3a63  kes a list of :c
+00031830: 6c61 7373 3a60 4669 6c65 6020 7265 7475  lass:`File` retu
+00031840: 726e 7320 6120 6469 6374 696f 6e61 7279  rns a dictionary
+00031850: 2077 6974 6820 6469 7361 6d62 6967 7561   with disambigua
+00031860: 7469 6e67 2073 7472 696e 6773 2062 6173  ting strings bas
+00031870: 6564 206f 6e20 7061 7468 2063 6f6d 706f  ed on path compo
+00031880: 6e65 6e74 732e 0a20 2020 206f 6620 6469  nents..    of di
+00031890: 7374 696e 6374 2073 7472 696e 6773 2074  stinct strings t
+000318a0: 6f20 6469 7374 696e 6775 6973 6820 6669  o distinguish fi
+000318b0: 6c65 7320 7065 7274 6169 6e69 6e67 2074  les pertaining t
+000318c0: 6f20 7468 6520 7361 6d65 2074 7970 652e  o the same type.
+000318d0: 2222 220a 2020 2020 6e5f 6669 6c65 7320  """.    n_files 
+000318e0: 3d20 6c65 6e28 6669 6c65 7329 0a20 2020  = len(files).   
+000318f0: 2069 6620 6e5f 6669 6c65 7320 3d3d 2030   if n_files == 0
+00031900: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00031910: 207b 7d0a 2020 2020 6669 6c65 7320 3d20   {}.    files = 
+00031920: 7475 706c 6528 6669 6c65 7329 0a20 2020  tuple(files).   
+00031930: 2069 6620 6e5f 6669 6c65 733d 3d20 313a   if n_files== 1:
+00031940: 0a20 2020 2020 2020 2066 203d 2066 696c  .        f = fil
+00031950: 6573 5b30 5d0a 2020 2020 2020 2020 7265  es[0].        re
+00031960: 7475 726e 207b 662e 7479 7065 3a20 667d  turn {f.type: f}
+00031970: 0a20 2020 2064 6973 616d 6269 6775 6174  .    disambiguat
+00031980: 696f 6e20 3d20 5b66 2e74 7970 6520 666f  ion = [f.type fo
+00031990: 7220 6620 696e 2066 696c 6573 5d0a 2020  r f in files].  
+000319a0: 2020 6966 206c 656e 2873 6574 2864 6973    if len(set(dis
+000319b0: 616d 6269 6775 6174 696f 6e29 2920 3d3d  ambiguation)) ==
+000319c0: 206e 5f66 696c 6573 3a0a 2020 2020 2020   n_files:.      
+000319d0: 2020 2320 646f 6e65 2064 6973 616d 6269    # done disambi
+000319e0: 6775 6174 696e 670a 2020 2020 2020 2020  guating.        
+000319f0: 7265 7475 726e 2064 6963 7428 7a69 7028  return dict(zip(
+00031a00: 6469 7361 6d62 6967 7561 7469 6f6e 2c20  disambiguation, 
+00031a10: 6669 6c65 7329 290a 2020 2020 6966 2069  files)).    if i
+00031a20: 6e63 6c75 6465 5f64 6973 616d 6269 6775  nclude_disambigu
+00031a30: 6174 6f72 2061 6e64 206c 656e 2873 6574  ator and len(set
+00031a40: 2864 6973 616d 6269 6775 6174 696f 6e29  (disambiguation)
+00031a50: 2920 3e20 313a 0a20 2020 2020 2020 206c  ) > 1:.        l
+00031a60: 6f67 6765 722e 7761 726e 696e 6728 6622  ogger.warning(f"
+00031a70: 496e 636c 7564 696e 6720 7468 6520 6469  Including the di
+00031a80: 7361 6d62 6967 7561 746f 7220 7265 6d6f  sambiguator remo
+00031a90: 7665 7320 7468 6520 6661 6365 7420 6e61  ves the facet na
+00031aa0: 6d65 2c20 6275 7420 7468 6520 6669 6c65  me, but the file
+00031ab0: 7320 7065 7274 6169 6e20 746f 2022 0a20  s pertain to ". 
+00031ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031ad0: 2020 2020 6622 7365 7665 7261 6c20 6661      f"several fa
+00031ae0: 6365 7473 3a20 7b73 6574 2864 6973 616d  cets: {set(disam
+00031af0: 6269 6775 6174 696f 6e29 7d22 290a 2020  biguation)}").  
+00031b00: 2020 2320 6669 7273 742c 2074 7279 2074    # first, try t
+00031b10: 6f20 6469 7361 6d62 6967 7561 7465 2062  o disambiguate b
+00031b20: 6173 6564 206f 6e20 7468 6520 6669 6c65  ased on the file
+00031b30: 7327 2073 7562 2d64 6972 6563 746f 7269  s' sub-directori
+00031b40: 6573 0a20 2020 2073 7562 6469 7273 203d  es.    subdirs =
+00031b50: 205b 5d0a 2020 2020 666f 7220 6620 696e   [].    for f in
+00031b60: 2066 696c 6573 3a0a 2020 2020 2020 2020   files:.        
+00031b70: 6669 6c65 5f74 7970 6520 3d20 662e 7479  file_type = f.ty
+00031b80: 7065 0a20 2020 2020 2020 2073 7562 6469  pe.        subdi
+00031b90: 7220 3d20 662e 7375 6264 6972 2e73 7472  r = f.subdir.str
+00031ba0: 6970 2872 225c 2f2e 2229 0a20 2020 2020  ip(r"\/.").     
+00031bb0: 2020 2069 6620 7375 6264 6972 2e73 7461     if subdir.sta
+00031bc0: 7274 7377 6974 6828 6669 6c65 5f74 7970  rtswith(file_typ
+00031bd0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00031be0: 7375 6264 6972 203d 2073 7562 6469 725b  subdir = subdir[
+00031bf0: 6c65 6e28 6669 6c65 5f74 7970 6529 3a5d  len(file_type):]
+00031c00: 0a20 2020 2020 2020 2069 6620 7375 6264  .        if subd
+00031c10: 6972 2e73 7472 6970 2872 225c 2f22 2920  ir.strip(r"\/") 
+00031c20: 3d3d 2027 273a 0a20 2020 2020 2020 2020  == '':.         
+00031c30: 2020 2073 7562 6469 7220 3d20 2727 0a20     subdir = ''. 
+00031c40: 2020 2020 2020 2073 7562 6469 7273 2e61         subdirs.a
+00031c50: 7070 656e 6428 7375 6264 6972 290a 2020  ppend(subdir).  
+00031c60: 2020 6966 206c 656e 2873 6574 2873 7562    if len(set(sub
+00031c70: 6469 7273 2929 203e 2031 3a0a 2020 2020  dirs)) > 1:.    
+00031c80: 2020 2020 2320 6669 6c65 7320 6361 6e20      # files can 
+00031c90: 2870 6172 7469 616c 6c79 2920 6265 2064  (partially) be d
+00031ca0: 6973 616d 6269 6775 6174 6564 2062 6563  isambiguated bec
+00031cb0: 6175 7365 2074 6865 7920 6172 6520 696e  ause they are in
+00031cc0: 2064 6966 6665 7265 6e74 2073 7562 2d64   different sub-d
+00031cd0: 6972 6563 746f 7269 6573 0a20 2020 2020  irectories.     
+00031ce0: 2020 2069 6620 696e 636c 7564 655f 6469     if include_di
+00031cf0: 7361 6d62 6967 7561 746f 723a 0a20 2020  sambiguator:.   
+00031d00: 2020 2020 2020 2020 2064 6973 616d 6269           disambi
+00031d10: 6775 6174 696f 6e20 3d20 5b66 2273 7562  guation = [f"sub
+00031d20: 6469 723a 207b 272e 2720 6966 2073 7562  dir: {'.' if sub
+00031d30: 6469 7220 3d3d 2027 2720 656c 7365 2073  dir == '' else s
+00031d40: 7562 6469 727d 2220 666f 7220 6469 7361  ubdir}" for disa
+00031d50: 6d62 2c20 7375 6264 6972 2069 6e20 7a69  mb, subdir in zi
+00031d60: 7028 6469 7361 6d62 6967 7561 7469 6f6e  p(disambiguation
+00031d70: 2c20 7375 6264 6972 7329 5d0a 2020 2020  , subdirs)].    
+00031d80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00031d90: 2020 2020 2020 6469 7361 6d62 6967 7561        disambigua
+00031da0: 7469 6f6e 203d 205b 6f73 2e70 6174 682e  tion = [os.path.
+00031db0: 6a6f 696e 2864 6973 616d 622c 2073 7562  join(disamb, sub
+00031dc0: 6469 7229 2066 6f72 2064 6973 616d 622c  dir) for disamb,
+00031dd0: 2073 7562 6469 7220 696e 207a 6970 2864   subdir in zip(d
+00031de0: 6973 616d 6269 6775 6174 696f 6e2c 2073  isambiguation, s
+00031df0: 7562 6469 7273 295d 0a20 2020 2069 6620  ubdirs)].    if 
+00031e00: 6c65 6e28 7365 7428 6469 7361 6d62 6967  len(set(disambig
+00031e10: 7561 7469 6f6e 2929 203d 3d20 6e5f 6669  uation)) == n_fi
+00031e20: 6c65 733a 0a20 2020 2020 2020 2023 2064  les:.        # d
+00031e30: 6f6e 6520 6469 7361 6d62 6967 7561 7469  one disambiguati
+00031e40: 6e67 0a20 2020 2020 2020 2072 6574 7572  ng.        retur
+00031e50: 6e20 6469 6374 287a 6970 2864 6973 616d  n dict(zip(disam
+00031e60: 6269 6775 6174 696f 6e2c 2066 696c 6573  biguation, files
+00031e70: 2929 0a20 2020 2023 206e 6578 742c 2074  )).    # next, t
+00031e80: 7279 2061 6464 696e 6720 6465 7465 6374  ry adding detect
+00031e90: 6564 2073 7566 6669 7865 730a 2020 2020  ed suffixes.    
+00031ea0: 666f 7220 6978 2c20 6620 696e 2065 6e75  for ix, f in enu
+00031eb0: 6d65 7261 7465 2866 696c 6573 293a 0a20  merate(files):. 
+00031ec0: 2020 2020 2020 2069 6620 662e 7375 6666         if f.suff
+00031ed0: 6978 2021 3d20 2727 3a0a 2020 2020 2020  ix != '':.      
+00031ee0: 2020 2020 2020 6966 2069 6e63 6c75 6465        if include
+00031ef0: 5f64 6973 616d 6269 6775 6174 6f72 3a0a  _disambiguator:.
+00031f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031f10: 6469 7361 6d62 6967 7561 7469 6f6e 5b69  disambiguation[i
+00031f20: 785d 202b 3d20 6622 2c20 7375 6666 6978  x] += f", suffix
+00031f30: 3a20 7b66 2e73 7566 6669 787d 220a 2020  : {f.suffix}".  
+00031f40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00031f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031f60: 6469 7361 6d62 6967 7561 7469 6f6e 5b69  disambiguation[i
+00031f70: 785d 202b 3d20 6622 5b7b 662e 7375 6666  x] += f"[{f.suff
+00031f80: 6978 7d5d 220a 2020 2020 6966 206c 656e  ix}]".    if len
+00031f90: 2873 6574 2864 6973 616d 6269 6775 6174  (set(disambiguat
+00031fa0: 696f 6e29 2920 3d3d 206e 5f66 696c 6573  ion)) == n_files
+00031fb0: 3a0a 2020 2020 2020 2020 2320 646f 6e65  :.        # done
+00031fc0: 2064 6973 616d 6269 6775 6174 696e 670a   disambiguating.
+00031fd0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00031fe0: 6963 7428 7a69 7028 6469 7361 6d62 6967  ict(zip(disambig
+00031ff0: 7561 7469 6f6e 2c20 6669 6c65 7329 290a  uation, files)).
+00032000: 2020 2020 2320 6e6f 772c 2061 6464 2066      # now, add f
+00032010: 696c 6520 6578 7465 6e73 696f 6e73 2074  ile extensions t
+00032020: 6f20 6469 7361 6d62 6967 7561 7465 2066  o disambiguate f
+00032030: 7572 7468 6572 0a20 2020 2069 6620 6c65  urther.    if le
+00032040: 6e28 7365 7428 662e 6665 7874 2066 6f72  n(set(f.fext for
+00032050: 2066 2069 6e20 6669 6c65 7329 2920 3e20   f in files)) > 
+00032060: 313a 0a20 2020 2020 2020 2066 6f72 2069  1:.        for i
+00032070: 782c 2066 2069 6e20 656e 756d 6572 6174  x, f in enumerat
+00032080: 6528 6669 6c65 7329 3a0a 2020 2020 2020  e(files):.      
+00032090: 2020 2020 2020 6966 2069 6e63 6c75 6465        if include
+000320a0: 5f64 6973 616d 6269 6775 6174 6f72 3a0a  _disambiguator:.
+000320b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000320c0: 6469 7361 6d62 6967 7561 7469 6f6e 5b69  disambiguation[i
+000320d0: 785d 202b 3d20 6622 2c20 6665 7874 3a20  x] += f", fext: 
+000320e0: 7b66 2e66 6578 747d 220a 2020 2020 2020  {f.fext}".      
+000320f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00032100: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+00032110: 6d62 6967 7561 7469 6f6e 5b69 785d 202b  mbiguation[ix] +
+00032120: 3d20 662e 6665 7874 0a20 2020 2069 6620  = f.fext.    if 
+00032130: 6c65 6e28 7365 7428 6469 7361 6d62 6967  len(set(disambig
+00032140: 7561 7469 6f6e 2929 203d 3d20 6e5f 6669  uation)) == n_fi
+00032150: 6c65 733a 0a20 2020 2020 2020 2023 2064  les:.        # d
+00032160: 6f6e 6520 6469 7361 6d62 6967 7561 7469  one disambiguati
+00032170: 6e67 0a20 2020 2020 2020 2072 6574 7572  ng.        retur
+00032180: 6e20 6469 6374 287a 6970 2864 6973 616d  n dict(zip(disam
+00032190: 6269 6775 6174 696f 6e2c 2066 696c 6573  biguation, files
+000321a0: 2929 0a20 2020 2073 7472 5f63 6f75 6e74  )).    str_count
+000321b0: 7320 3d20 436f 756e 7465 7228 6469 7361  s = Counter(disa
+000321c0: 6d62 6967 7561 7469 6f6e 290a 2020 2020  mbiguation).    
+000321d0: 6475 706c 6963 6174 655f 6469 7361 6d62  duplicate_disamb
+000321e0: 6967 7561 7469 6f6e 5f73 7472 696e 6773  iguation_strings
+000321f0: 203d 205b 7320 666f 7220 732c 2063 6e74   = [s for s, cnt
+00032200: 2069 6e20 7374 725f 636f 756e 7473 2e69   in str_counts.i
+00032210: 7465 6d73 2829 2069 6620 636e 7420 3e20  tems() if cnt > 
+00032220: 315d 0a20 2020 2061 6d62 6967 7561 7465  1].    ambiguate
+00032230: 5f66 696c 6573 203d 207b 733a 205b 6620  _files = {s: [f 
+00032240: 666f 7220 6469 7361 6d62 2c20 6620 696e  for disamb, f in
+00032250: 207a 6970 2864 6973 616d 6269 6775 6174   zip(disambiguat
+00032260: 696f 6e2c 2066 696c 6573 2920 6966 2064  ion, files) if d
+00032270: 6973 616d 6220 3d3d 2073 5d20 666f 7220  isamb == s] for 
+00032280: 7320 696e 2064 7570 6c69 6361 7465 5f64  s in duplicate_d
+00032290: 6973 616d 6269 6775 6174 696f 6e5f 7374  isambiguation_st
+000322a0: 7269 6e67 737d 0a20 2020 2072 6573 756c  rings}.    resul
+000322b0: 7420 3d20 6469 6374 287a 6970 2864 6973  t = dict(zip(dis
+000322c0: 616d 6269 6775 6174 696f 6e2c 2066 696c  ambiguation, fil
+000322d0: 6573 2929 0a20 2020 2072 656d 6169 6e69  es)).    remaini
+000322e0: 6e67 5f6f 6e65 7320 3d20 7b73 3a20 7265  ng_ones = {s: re
+000322f0: 7375 6c74 5b73 5d20 666f 7220 7320 696e  sult[s] for s in
+00032300: 2064 7570 6c69 6361 7465 5f64 6973 616d   duplicate_disam
+00032310: 6269 6775 6174 696f 6e5f 7374 7269 6e67  biguation_string
+00032320: 737d 0a20 2020 206c 6f67 6765 722e 7761  s}.    logger.wa
+00032330: 726e 696e 6728 6622 5468 6520 666f 6c6c  rning(f"The foll
+00032340: 6f77 696e 6720 6669 6c65 7320 636f 756c  owing files coul
+00032350: 6420 6e6f 7420 6265 2061 6d62 6967 7561  d not be ambigua
+00032360: 7465 643a 207b 616d 6269 6775 6174 655f  ted: {ambiguate_
+00032370: 6669 6c65 737d 2e5c 6e22 0a20 2020 2020  files}.\n".     
+00032380: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00032390: 496e 2074 6865 2072 6573 756c 742c 206f  In the result, o
+000323a0: 6e6c 7920 7468 6573 6520 7265 6d61 696e  nly these remain
+000323b0: 3a20 7b72 656d 6169 6e69 6e67 5f6f 6e65  : {remaining_one
+000323c0: 737d 2e22 290a 2020 2020 7265 7475 726e  s}.").    return
+000323d0: 2072 6573 756c 740a 0a0a 6465 6620 6c69   result...def li
+000323e0: 7465 7261 6c5f 7479 7065 3274 7570 6c65  teral_type2tuple
+000323f0: 2874 7970 3a20 5479 7065 5661 7229 202d  (typ: TypeVar) -
+00032400: 3e20 5475 706c 655b 7374 725d 3a0a 2020  > Tuple[str]:.  
+00032410: 2020 2222 2254 7572 6e73 2074 6865 2066    """Turns the f
+00032420: 6972 7374 204c 6974 6572 616c 2069 6e63  irst Literal inc
+00032430: 6c75 6465 6420 696e 2074 6865 2054 7970  luded in the Typ
+00032440: 6556 6172 2069 6e74 6f20 6120 6c69 7374  eVar into a list
+00032450: 206f 6620 7661 6c75 6573 2e20 5468 6520   of values. The 
+00032460: 6669 7273 7420 6c69 7465 7261 6c20 7661  first literal va
+00032470: 6c75 650a 2020 2020 6e65 6564 7320 746f  lue.    needs to
+00032480: 2062 6520 6120 7374 7269 6e67 2c20 6f74   be a string, ot
+00032490: 6865 7277 6973 6520 7468 6520 6675 6e63  herwise the func
+000324a0: 7469 6f6e 206d 6179 206c 6561 6420 746f  tion may lead to
+000324b0: 2075 6e65 7870 6563 7465 6420 6265 6861   unexpected beha
+000324c0: 7669 6f75 722e 0a20 2020 2022 2222 0a20  viour..    """. 
+000324d0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000324e0: 2874 7970 2e5f 5f61 7267 735f 5f5b 305d  (typ.__args__[0]
+000324f0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+00032500: 7265 7475 726e 2074 7970 2e5f 5f61 7267  return typ.__arg
+00032510: 735f 5f0a 2020 2020 7265 7475 726e 206c  s__.    return l
+00032520: 6974 6572 616c 5f74 7970 6532 7475 706c  iteral_type2tupl
+00032530: 6528 7479 702e 5f5f 6172 6773 5f5f 5b30  e(typ.__args__[0
+00032540: 5d29 0a0a 0a40 6c72 755f 6361 6368 650a  ])...@lru_cache.
+00032550: 4066 756e 6374 696f 6e5f 6c6f 6767 6572  @function_logger
+00032560: 0a64 6566 2061 7267 756d 656e 745f 616e  .def argument_an
+00032570: 645f 6c69 7465 7261 6c5f 7479 7065 326c  d_literal_type2l
+00032580: 6973 7428 6172 6775 6d65 6e74 3a20 556e  ist(argument: Un
+00032590: 696f 6e5b 7374 722c 2054 7570 6c65 5b73  ion[str, Tuple[s
+000325a0: 7472 5d2c 204c 6974 6572 616c 5b4e 6f6e  tr], Literal[Non
+000325b0: 655d 5d2c 0a20 2020 2020 2020 2020 2020  e]],.           
+000325c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000325d0: 2020 2020 2020 2020 7479 703a 204f 7074          typ: Opt
+000325e0: 696f 6e61 6c5b 556e 696f 6e5b 5479 7065  ional[Union[Type
+000325f0: 5661 722c 2054 7570 6c65 5b73 7472 5d5d  Var, Tuple[str]]
+00032600: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
 00032610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032620: 2020 2020 2920 2d3e 204f 7074 696f 6e61      ) -> Optiona
-00032630: 6c5b 4c69 7374 5b73 7472 5d5d 3a0a 2020  l[List[str]]:.  
-00032640: 2020 2222 2220 4d61 6b65 7320 7375 7265    """ Makes sure
-00032650: 2074 6861 7420 616e 2069 6e70 7574 2076   that an input v
-00032660: 616c 7565 2069 7320 6120 6c69 7374 206f  alue is a list o
-00032670: 6620 7374 7269 6e67 7320 616e 6420 7468  f strings and th
-00032680: 6174 2061 6c6c 2073 7472 696e 6773 2061  at all strings a
-00032690: 7265 2076 616c 6964 2077 2e72 2e74 2e20  re valid w.r.t. 
-000326a0: 746f 0a20 2020 2074 6865 2074 7970 6527  to.    the type'
-000326b0: 7320 6578 7065 6374 6564 206c 6974 6572  s expected liter
-000326c0: 616c 2076 616c 7565 7320 2873 7472 696e  al values (strin
-000326d0: 6773 292e 0a0a 2020 2020 4172 6773 3a0a  gs)...    Args:.
-000326e0: 2020 2020 2020 6172 6775 6d65 6e74 3a0a        argument:.
-000326f0: 2020 2020 2020 2020 2020 4966 2073 7472            If str
-00032700: 696e 672c 2077 7261 7070 6564 2069 6e20  ing, wrapped in 
-00032710: 6120 6c69 7374 2c20 6f74 6865 7277 6973  a list, otherwis
-00032720: 6520 6578 7065 6374 6564 2074 6f20 6265  e expected to be
-00032730: 2061 2074 7570 6c65 206f 6620 7374 7269   a tuple of stri
-00032740: 6e67 7320 2870 6173 7369 6e67 2061 206c  ngs (passing a l
-00032750: 6973 7420 7769 6c6c 2066 6169 6c29 2e0a  ist will fail)..
-00032760: 2020 2020 2020 2020 2020 4966 204e 6f6e            If Non
-00032770: 652c 2061 206c 6973 7420 6f66 2061 6c6c  e, a list of all
-00032780: 2070 6f73 7369 626c 6520 7661 6c75 6573   possible values
-00032790: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
-000327a0: 6520 7479 7065 2069 7320 7265 7475 726e  e type is return
-000327b0: 6564 2069 6620 6e6f 6e65 5f6d 6561 6e73  ed if none_means
-000327c0: 5f61 6c6c 2e0a 2020 2020 2020 7479 703a  _all..      typ:
-000327d0: 0a20 2020 2020 2020 2020 2041 2074 7970  .          A typ
-000327e0: 696e 672e 4c69 7465 7261 6c20 6465 636c  ing.Literal decl
-000327f0: 6172 6174 696f 6e20 6f72 2061 2054 7970  aration or a Typ
-00032800: 6556 6172 2077 6865 7265 2074 6865 2066  eVar where the f
-00032810: 6972 7374 2063 6f6d 706f 6e65 6e74 2069  irst component i
-00032820: 7320 6f6e 652c 206f 7220 6120 7475 706c  s one, or a tupl
-00032830: 6520 6f66 2061 6c6c 6f77 6564 2076 616c  e of allowed val
-00032840: 7565 732e 0a20 2020 2020 2020 2020 2041  ues..          A
-00032850: 6c6c 2061 6c6c 6f77 6564 2076 616c 7565  ll allowed value
-00032860: 7320 7368 6f75 6c64 2062 6520 7374 7269  s should be stri
-00032870: 6e67 732e 0a20 2020 2020 206e 6f6e 655f  ngs..      none_
-00032880: 6d65 616e 735f 616c 6c3a 0a20 2020 2020  means_all:.     
-00032890: 2020 2020 2042 7920 6465 6661 756c 742c       By default,
-000328a0: 204e 6f6e 6520 7661 6c75 6573 2061 7265   None values are
-000328b0: 2072 6570 6c61 6365 6420 7769 7468 2061   replaced with a
-000328c0: 6c6c 2061 6c6c 6f77 6564 2076 616c 7565  ll allowed value
-000328d0: 732c 2069 6620 7370 6563 6966 6965 642e  s, if specified.
-000328e0: 0a20 2020 2020 2020 2020 2050 6173 7320  .          Pass 
-000328f0: 4661 6c73 6520 746f 2072 6574 7572 6e20  False to return 
-00032900: 4e6f 6e65 2069 6e20 7468 6973 2063 6173  None in this cas
-00032910: 652e 0a0a 2020 2020 5265 7475 726e 733a  e...    Returns:
-00032920: 0a20 2020 2020 2054 6865 206c 6973 7420  .      The list 
-00032930: 6f66 2061 6363 6570 7465 6420 7374 7269  of accepted stri
-00032940: 6e67 732e 0a20 2020 2020 2054 6865 206c  ngs..      The l
-00032950: 6973 7420 6f66 2072 656a 6563 7465 6420  ist of rejected 
-00032960: 7374 7269 6e67 732e 0a20 2020 2022 2222  strings..    """
-00032970: 0a20 2020 2069 6620 7479 7020 6973 204e  .    if typ is N
-00032980: 6f6e 653a 0a20 2020 2020 2020 2061 6c6c  one:.        all
-00032990: 6f77 6564 203d 204e 6f6e 650a 2020 2020  owed = None.    
-000329a0: 656c 7365 3a0a 2020 2020 2020 2020 6966  else:.        if
-000329b0: 2069 7369 6e73 7461 6e63 6528 7479 702c   isinstance(typ,
-000329c0: 2074 7570 6c65 293a 0a20 2020 2020 2020   tuple):.       
-000329d0: 2020 2020 2061 6c6c 6f77 6564 203d 2074       allowed = t
-000329e0: 7970 0a20 2020 2020 2020 2065 6c73 653a  yp.        else:
-000329f0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-00032a00: 6f77 6564 203d 206c 6974 6572 616c 5f74  owed = literal_t
-00032a10: 7970 6532 7475 706c 6528 7479 7029 0a20  ype2tuple(typ). 
-00032a20: 2020 2069 6620 6172 6775 6d65 6e74 2069     if argument i
-00032a30: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00032a40: 6966 206e 6f6e 655f 6d65 616e 735f 616c  if none_means_al
-00032a50: 6c20 616e 6420 616c 6c6f 7765 6420 6973  l and allowed is
-00032a60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00032a70: 2020 2020 2020 2072 6574 7572 6e20 6c69         return li
-00032a80: 7374 2861 6c6c 6f77 6564 290a 2020 2020  st(allowed).    
-00032a90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00032aa0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00032ab0: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
-00032ac0: 7267 756d 656e 742c 2073 7472 293a 0a20  rgument, str):. 
-00032ad0: 2020 2020 2020 2061 7267 756d 656e 7420         argument 
-00032ae0: 3d20 5b61 7267 756d 656e 745d 0a20 2020  = [argument].   
-00032af0: 2069 6620 616c 6c6f 7765 6420 6973 204e   if allowed is N
-00032b00: 6f6e 653a 0a20 2020 2020 2020 2072 6574  one:.        ret
-00032b10: 7572 6e20 6172 6775 6d65 6e74 0a20 2020  urn argument.   
-00032b20: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
-00032b30: 696e 6775 6c61 725f 6469 6374 203d 207b  ingular_dict = {
-00032b40: 616c 6c77 645b 3a2d 315d 3a20 616c 6c77  allwd[:-1]: allw
-00032b50: 6420 666f 7220 616c 6c77 6420 696e 2061  d for allwd in a
-00032b60: 6c6c 6f77 6564 7d0a 2020 2020 6163 6365  llowed}.    acce
-00032b70: 7074 6564 2c20 7265 6a65 6374 6564 203d  pted, rejected =
-00032b80: 205b 5d2c 205b 5d0a 2020 2020 666f 7220   [], [].    for 
-00032b90: 6172 6720 696e 2061 7267 756d 656e 743a  arg in argument:
-00032ba0: 0a20 2020 2020 2020 2069 6620 6172 6720  .        if arg 
-00032bb0: 696e 2061 6c6c 6f77 6564 3a0a 2020 2020  in allowed:.    
-00032bc0: 2020 2020 2020 2020 6163 6365 7074 6564          accepted
-00032bd0: 2e61 7070 656e 6428 6172 6729 0a20 2020  .append(arg).   
-00032be0: 2020 2020 2065 6c69 6620 6172 6720 696e       elif arg in
-00032bf0: 2073 696e 6775 6c61 725f 6469 6374 3a0a   singular_dict:.
-00032c00: 2020 2020 2020 2020 2020 2020 6163 6365              acce
-00032c10: 7074 6564 2e61 7070 656e 6428 7369 6e67  pted.append(sing
-00032c20: 756c 6172 5f64 6963 745b 6172 675d 290a  ular_dict[arg]).
-00032c30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00032c40: 2020 2020 2020 2020 2020 7265 6a65 6374            reject
-00032c50: 6564 2e61 7070 656e 6428 6172 6729 0a20  ed.append(arg). 
-00032c60: 2020 206e 5f72 656a 6563 7465 6420 3d20     n_rejected = 
-00032c70: 6c65 6e28 7265 6a65 6374 6564 290a 2020  len(rejected).  
-00032c80: 2020 6966 206e 5f72 656a 6563 7465 6420    if n_rejected 
-00032c90: 3e20 303a 0a20 2020 2020 2020 2069 6620  > 0:.        if 
-00032ca0: 6e5f 7265 6a65 6374 6564 203d 3d20 313a  n_rejected == 1:
-00032cb0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00032cc0: 6765 722e 7761 726e 696e 6728 6622 5468  ger.warning(f"Th
-00032cd0: 6973 2069 7320 6e6f 7420 616e 2061 6363  is is not an acc
-00032ce0: 6570 7465 6420 7661 6c75 653a 207b 7265  epted value: {re
-00032cf0: 6a65 6374 6564 5b30 5d7d 5c6e 220a 2020  jected[0]}\n".  
-00032d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032d10: 2020 2020 2020 2020 2066 2243 686f 6f73           f"Choos
-00032d20: 6520 6672 6f6d 207b 616c 6c6f 7765 647d  e from {allowed}
-00032d30: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
-00032d40: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00032d50: 6765 722e 7761 726e 696e 6728 6622 5468  ger.warning(f"Th
-00032d60: 6573 6520 6172 6520 6e6f 7420 6163 6365  ese are not acce
-00032d70: 7074 6564 2076 616c 7565 2c20 6f6e 6c79  pted value, only
-00032d80: 3a20 7b72 656a 6563 7465 647d 220a 2020  : {rejected}".  
-00032d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032da0: 2020 2020 2020 2020 2066 2243 686f 6f73           f"Choos
-00032db0: 6520 6672 6f6d 207b 616c 6c6f 7765 647d  e from {allowed}
-00032dc0: 2229 0a20 2020 2069 6620 6c65 6e28 6163  ").    if len(ac
-00032dd0: 6365 7074 6564 2920 3e20 303a 0a20 2020  cepted) > 0:.   
-00032de0: 2020 2020 2072 6574 7572 6e20 6163 6365       return acce
-00032df0: 7074 6564 0a20 2020 206c 6f67 6765 722e  pted.    logger.
-00032e00: 7761 726e 696e 6728 6622 5061 7373 2061  warning(f"Pass a
-00032e10: 7420 6c65 6173 7420 6f6e 6520 6f66 207b  t least one of {
-00032e20: 616c 6c6f 7765 647d 2e22 290a 2020 2020  allowed}.").    
-00032e30: 7265 7475 726e 0a0a 4c20 3d20 5479 7065  return..L = Type
-00032e40: 5661 7228 274c 2729 0a0a 4066 756e 6374  Var('L')..@funct
-00032e50: 696f 6e5f 6c6f 6767 6572 0a64 6566 2063  ion_logger.def c
-00032e60: 6865 636b 5f61 7267 756d 656e 745f 6167  heck_argument_ag
-00032e70: 6169 6e73 745f 6c69 7465 7261 6c5f 7479  ainst_literal_ty
-00032e80: 7065 2861 7267 756d 656e 743a 2073 7472  pe(argument: str
-00032e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00032ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032eb0: 2020 2020 2020 2020 2020 7479 703a 204c            typ: L
-00032ec0: 2920 2d3e 204f 7074 696f 6e61 6c5b 4c5d  ) -> Optional[L]
-00032ed0: 3a0a 2020 2020 6966 206e 6f74 2069 7369  :.    if not isi
-00032ee0: 6e73 7461 6e63 6528 6172 6775 6d65 6e74  nstance(argument
-00032ef0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00032f00: 6c6f 6767 6572 2e77 6172 6e69 6e67 2866  logger.warning(f
-00032f10: 2241 7267 756d 656e 7420 6e65 6564 7320  "Argument needs 
-00032f20: 746f 2062 6520 6120 7374 7269 6e67 2c20  to be a string, 
-00032f30: 6e6f 7420 277b 7479 7065 2861 7267 756d  not '{type(argum
-00032f40: 656e 7429 7d27 2229 0a20 2020 2020 2020  ent)}'").       
-00032f50: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
-00032f60: 2061 6c6c 6f77 6564 203d 206c 6974 6572   allowed = liter
-00032f70: 616c 5f74 7970 6532 7475 706c 6528 7479  al_type2tuple(ty
-00032f80: 7029 0a20 2020 2073 696e 6775 6c61 725f  p).    singular_
-00032f90: 6469 6374 203d 207b 616c 6c77 645b 3a2d  dict = {allwd[:-
-00032fa0: 315d 3a20 616c 6c77 6420 666f 7220 616c  1]: allwd for al
-00032fb0: 6c77 6420 696e 2061 6c6c 6f77 6564 7d0a  lwd in allowed}.
-00032fc0: 2020 2020 6966 2061 7267 756d 656e 7420      if argument 
-00032fd0: 6e6f 7420 696e 2061 6c6c 6f77 6564 2061  not in allowed a
-00032fe0: 6e64 2061 7267 756d 656e 7420 6e6f 7420  nd argument not 
-00032ff0: 696e 2073 696e 6775 6c61 725f 6469 6374  in singular_dict
-00033000: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
-00033010: 2e77 6172 6e69 6e67 2866 2249 6e76 616c  .warning(f"Inval
-00033020: 6964 2061 7267 756d 656e 7420 277b 6172  id argument '{ar
-00033030: 6775 6d65 6e74 7d27 2e20 5061 7373 206f  gument}'. Pass o
-00033040: 6e65 206f 6620 7b61 6c6c 6f77 6564 7d22  ne of {allowed}"
-00033050: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00033060: 204e 6f6e 650a 2020 2020 6966 2061 7267   None.    if arg
-00033070: 756d 656e 7420 696e 2073 696e 6775 6c61  ument in singula
-00033080: 725f 6469 6374 3a0a 2020 2020 2020 2020  r_dict:.        
-00033090: 7265 7475 726e 2073 696e 6775 6c61 725f  return singular_
-000330a0: 6469 6374 5b61 7267 756d 656e 745d 0a20  dict[argument]. 
-000330b0: 2020 2072 6574 7572 6e20 6172 6775 6d65     return argume
-000330c0: 6e74 0a0a 4066 756e 6374 696f 6e5f 6c6f  nt..@function_lo
-000330d0: 6767 6572 0a64 6566 2072 6573 6f6c 7665  gger.def resolve
-000330e0: 5f66 6163 6574 735f 7061 7261 6d28 6661  _facets_param(fa
-000330f0: 6365 7473 2c20 6661 6365 745f 7479 7065  cets, facet_type
-00033100: 5f76 6172 3a20 5479 7065 5661 7220 3d20  _var: TypeVar = 
-00033110: 4661 6365 742c 206e 6f6e 655f 6d65 616e  Facet, none_mean
-00033120: 735f 616c 6c3d 5472 7565 293a 0a20 2020  s_all=True):.   
-00033130: 2022 2222 4c69 6b65 203a 6675 6e63 3a60   """Like :func:`
-00033140: 6172 6775 6d65 6e74 5f61 6e64 5f6c 6974  argument_and_lit
-00033150: 6572 616c 5f74 7970 6532 6c69 7374 602c  eral_type2list`,
-00033160: 2062 7574 2061 6c73 6f20 7265 736f 6c76   but also resolv
-00033170: 6573 2027 7473 7627 2074 6f20 616c 6c20  es 'tsv' to all 
-00033180: 6e6f 6e2d 7363 6f72 6520 6661 6365 7473  non-score facets
-00033190: 2e22 2222 0a20 2020 2069 6620 6973 696e  .""".    if isin
-000331a0: 7374 616e 6365 2866 6163 6574 732c 2073  stance(facets, s
-000331b0: 7472 2920 616e 6420 6661 6365 7473 2069  tr) and facets i
-000331c0: 6e20 2827 7473 7627 2c20 2774 7376 7327  n ('tsv', 'tsvs'
-000331d0: 293a 0a20 2020 2020 2020 2073 656c 6563  ):.        selec
-000331e0: 7465 645f 6661 6365 7473 203d 206c 6973  ted_facets = lis
-000331f0: 7428 6c69 7465 7261 6c5f 7479 7065 3274  t(literal_type2t
-00033200: 7570 6c65 2866 6163 6574 5f74 7970 655f  uple(facet_type_
-00033210: 7661 7229 290a 2020 2020 2020 2020 6966  var)).        if
-00033220: 2027 7363 6f72 6573 2720 696e 2073 656c   'scores' in sel
-00033230: 6563 7465 645f 6661 6365 7473 3a0a 2020  ected_facets:.  
-00033240: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-00033250: 6564 5f66 6163 6574 732e 7265 6d6f 7665  ed_facets.remove
-00033260: 2827 7363 6f72 6573 2729 0a20 2020 2065  ('scores').    e
-00033270: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
-00033280: 6973 696e 7374 616e 6365 2866 6163 6574  isinstance(facet
-00033290: 732c 206c 6973 7429 3a0a 2020 2020 2020  s, list):.      
-000332a0: 2020 2020 2020 6661 6365 7473 203d 2074        facets = t
-000332b0: 7570 6c65 2866 6163 6574 7329 0a20 2020  uple(facets).   
-000332c0: 2020 2020 2073 656c 6563 7465 645f 6661       selected_fa
-000332d0: 6365 7473 203d 2061 7267 756d 656e 745f  cets = argument_
-000332e0: 616e 645f 6c69 7465 7261 6c5f 7479 7065  and_literal_type
-000332f0: 326c 6973 7428 6661 6365 7473 2c20 6661  2list(facets, fa
-00033300: 6365 745f 7479 7065 5f76 6172 2c20 6e6f  cet_type_var, no
-00033310: 6e65 5f6d 6561 6e73 5f61 6c6c 3d6e 6f6e  ne_means_all=non
-00033320: 655f 6d65 616e 735f 616c 6c2c 206c 6f67  e_means_all, log
-00033330: 6765 723d 6c6f 6767 6572 290a 2020 2020  ger=logger).    
-00033340: 236c 6f67 6765 722e 6465 6275 6728 6622  #logger.debug(f"
-00033350: 5265 736f 6c76 6564 2061 7267 756d 656e  Resolved argumen
-00033360: 7420 277b 6661 6365 7473 7d27 2074 6f20  t '{facets}' to 
-00033370: 7b73 656c 6563 7465 645f 6661 6365 7473  {selected_facets
-00033380: 7d2e 2229 0a20 2020 2072 6574 7572 6e20  }.").    return 
-00033390: 7365 6c65 6374 6564 5f66 6163 6574 730a  selected_facets.
-000333a0: 0a64 6566 2062 6f6c 645f 666f 6e74 2873  .def bold_font(s
-000333b0: 293a 0a20 2020 2072 6574 7572 6e20 6622  ):.    return f"
-000333c0: 5c30 3333 5b31 6d7b 737d 5c30 3333 5b30  \033[1m{s}\033[0
-000333d0: 3b30 6d22 0a0a 6465 6620 6176 6169 6c61  ;0m"..def availa
-000333e0: 626c 655f 7669 6577 7332 7374 7228 7669  ble_views2str(vi
-000333f0: 6577 735f 6469 6374 3a20 5669 6577 4469  ews_dict: ViewDi
-00033400: 6374 2c20 6163 7469 7665 5f76 6965 775f  ct, active_view_
-00033410: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-00033420: 2920 2d3e 2073 7472 3a0a 2020 2020 7669  ) -> str:.    vi
-00033430: 6577 5f6e 616d 6573 203d 207b 6b65 793a  ew_names = {key:
-00033440: 2076 6965 772e 6e61 6d65 2069 6620 6b65   view.name if ke
-00033450: 7920 6973 204e 6f6e 6520 656c 7365 206b  y is None else k
-00033460: 6579 2066 6f72 206b 6579 2c20 7669 6577  ey for key, view
-00033470: 2069 6e20 7669 6577 735f 6469 6374 2e69   in views_dict.i
-00033480: 7465 6d73 2829 7d0a 2020 2020 6375 7272  tems()}.    curr
-00033490: 656e 745f 7669 6577 203d 2076 6965 775f  ent_view = view_
-000334a0: 6e61 6d65 735b 6163 7469 7665 5f76 6965  names[active_vie
-000334b0: 775f 6e61 6d65 5d0a 2020 2020 7669 6577  w_name].    view
-000334c0: 5f6c 6973 7420 3d20 5b62 6f6c 645f 666f  _list = [bold_fo
-000334d0: 6e74 2863 7572 7265 6e74 5f76 6965 7729  nt(current_view)
-000334e0: 5d20 2b20 5b6e 616d 6520 666f 7220 6e61  ] + [name for na
-000334f0: 6d65 2069 6e20 7669 6577 5f6e 616d 6573  me in view_names
-00033500: 2e76 616c 7565 7328 2920 6966 206e 616d  .values() if nam
-00033510: 6520 213d 2063 7572 7265 6e74 5f76 6965  e != current_vie
-00033520: 775d 0a20 2020 2072 6574 7572 6e20 6622  w].    return f"
-00033530: 5b7b 277c 272e 6a6f 696e 2876 6965 775f  [{'|'.join(view_
-00033540: 6c69 7374 297d 5d5c 6e22 0a0a 0a40 6675  list)}]\n"...@fu
-00033550: 6e63 7469 6f6e 5f6c 6f67 6765 720a 6465  nction_logger.de
-00033560: 6620 756e 7061 636b 5f6a 736f 6e5f 7061  f unpack_json_pa
-00033570: 7468 7328 7061 7468 733a 2043 6f6c 6c65  ths(paths: Colle
-00033580: 6374 696f 6e5b 7374 725d 2920 2d3e 204e  ction[str]) -> N
-00033590: 6f6e 653a 0a20 2020 2022 2222 4d75 7461  one:.    """Muta
-000335a0: 7465 7320 7468 6520 6c69 7374 2077 6974  tes the list wit
-000335b0: 6820 7061 7468 7320 6279 2072 6570 6c61  h paths by repla
-000335c0: 6369 6e67 202e 6a73 6f6e 2066 696c 6573  cing .json files
-000335d0: 2077 6974 6820 7468 6520 6c69 7374 2028   with the list (
-000335e0: 6f66 2070 6174 6873 2920 636f 6e74 6169  of paths) contai
-000335f0: 6e65 6420 696e 2074 6865 6d2e 2222 220a  ned in them.""".
-00033600: 2020 2020 6a73 6f6e 5f69 7873 203d 205b      json_ixs = [
-00033610: 6920 666f 7220 692c 2070 2069 6e20 656e  i for i, p in en
-00033620: 756d 6572 6174 6528 7061 7468 7329 2069  umerate(paths) i
-00033630: 6620 702e 656e 6473 7769 7468 2827 2e6a  f p.endswith('.j
-00033640: 736f 6e27 295d 0a20 2020 2069 6620 6c65  son')].    if le
-00033650: 6e28 6a73 6f6e 5f69 7873 2920 3e20 303a  n(json_ixs) > 0:
-00033660: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-00033670: 6e20 7265 7665 7273 6564 286a 736f 6e5f  n reversed(json_
-00033680: 6978 7329 3a0a 2020 2020 2020 2020 2020  ixs):.          
-00033690: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-000336a0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-000336b0: 2870 6174 6873 5b69 5d29 2061 7320 663a  (paths[i]) as f:
-000336c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000336d0: 2020 2020 206c 6f61 6465 645f 7061 7468       loaded_path
-000336e0: 7320 3d20 6a73 6f6e 2e6c 6f61 6428 6629  s = json.load(f)
-000336f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00033700: 2070 6174 6873 2e65 7874 656e 6428 6c6f   paths.extend(lo
-00033710: 6164 6564 5f70 6174 6873 290a 2020 2020  aded_paths).    
-00033720: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00033730: 6572 2e69 6e66 6f28 6622 556e 7061 636b  er.info(f"Unpack
-00033740: 6564 2074 6865 207b 6c65 6e28 6c6f 6164  ed the {len(load
-00033750: 6564 5f70 6174 6873 297d 2070 6174 6873  ed_paths)} paths
-00033760: 2066 6f75 6e64 2069 6e20 7b70 6174 6873   found in {paths
-00033770: 5b69 5d7d 2e22 290a 2020 2020 2020 2020  [i]}.").        
-00033780: 2020 2020 2020 2020 6465 6c20 2870 6174          del (pat
-00033790: 6873 5b69 5d29 0a20 2020 2020 2020 2020  hs[i]).         
-000337a0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000337b0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-000337c0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-000337d0: 2866 2243 6f75 6c64 206e 6f74 206c 6f61  (f"Could not loa
-000337e0: 6420 7061 7468 7320 6672 6f6d 207b 7061  d paths from {pa
-000337f0: 7468 735b 695d 7d20 6265 6361 7573 6520  ths[i]} because 
-00033800: 6f66 2074 6865 2066 6f6c 6c6f 7769 6e67  of the following
-00033810: 2065 7272 6f72 2873 293a 5c6e 7b73 7973   error(s):\n{sys
-00033820: 2e65 7863 5f69 6e66 6f28 295b 315d 7d22  .exc_info()[1]}"
-00033830: 290a 0a0a 4066 756e 6374 696f 6e5f 6c6f  )...@function_lo
-00033840: 6767 6572 0a64 6566 2072 6573 6f6c 7665  gger.def resolve
-00033850: 5f70 6174 6873 5f61 7267 756d 656e 7428  _paths_argument(
-00033860: 7061 7468 733a 2055 6e69 6f6e 5b73 7472  paths: Union[str
-00033870: 2c20 436f 6c6c 6563 7469 6f6e 5b73 7472  , Collection[str
-00033880: 5d5d 2c0a 2020 2020 2020 2020 2020 2020  ]],.            
-00033890: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000338a0: 696c 6573 3a20 626f 6f6c 203d 2054 7275  iles: bool = Tru
-000338b0: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-000338c0: 0a20 2020 2022 2222 204d 616b 6573 2073  .    """ Makes s
-000338d0: 7572 6520 7468 6174 2074 6865 2067 6976  ure that the giv
-000338e0: 656e 2070 6174 6828 7329 2065 7869 7374  en path(s) exist
-000338f0: 7328 7329 2061 6e64 2066 696c 7465 7273  s(s) and filters
-00033900: 206f 7574 2074 686f 7365 2074 6861 7420   out those that 
-00033910: 646f 6e27 742e 0a0a 2020 2020 4172 6773  don't...    Args
-00033920: 3a0a 2020 2020 2020 7061 7468 733a 204f  :.      paths: O
-00033930: 6e65 206f 7220 7365 7665 7261 6c20 7061  ne or several pa
-00033940: 7468 7320 6769 7665 6e20 6173 2073 7472  ths given as str
-00033950: 696e 6773 2e0a 2020 2020 2020 6669 6c65  ings..      file
-00033960: 733a 2042 7920 6465 6661 756c 742c 206f  s: By default, o
-00033970: 6e6c 7920 6669 6c65 2070 6174 6873 2061  nly file paths a
-00033980: 7265 2072 6574 7572 6e65 642e 2053 6574  re returned. Set
-00033990: 2074 6f20 4661 6c73 6520 746f 2072 6574   to False to ret
-000339a0: 7572 6e20 6f6e 6c79 2066 6f6c 6465 7273  urn only folders
-000339b0: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
-000339c0: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-000339d0: 6973 696e 7374 616e 6365 2870 6174 6873  isinstance(paths
-000339e0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-000339f0: 7061 7468 7320 3d20 5b70 6174 6873 5d0a  paths = [paths].
-00033a00: 2020 2020 7265 736f 6c76 6564 5f70 6174      resolved_pat
-00033a10: 6873 203d 205b 7265 736f 6c76 655f 6469  hs = [resolve_di
-00033a20: 7228 7029 2066 6f72 2070 2069 6e20 7061  r(p) for p in pa
-00033a30: 7468 735d 0a20 2020 2069 6620 6669 6c65  ths].    if file
-00033a40: 733a 0a20 2020 2020 2020 206e 6f74 5f61  s:.        not_a
-00033a50: 5f66 696c 6520 3d20 5b70 2066 6f72 2070  _file = [p for p
-00033a60: 2069 6e20 7265 736f 6c76 6564 5f70 6174   in resolved_pat
-00033a70: 6873 2069 6620 6e6f 7420 6f73 2e70 6174  hs if not os.pat
-00033a80: 682e 6973 6669 6c65 2870 295d 0a20 2020  h.isfile(p)].   
-00033a90: 2020 2020 2069 6620 6c65 6e28 6e6f 745f       if len(not_
-00033aa0: 615f 6669 6c65 2920 3e20 303a 0a20 2020  a_file) > 0:.   
-00033ab0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00033ac0: 6e6f 745f 615f 6669 6c65 2920 3d3d 2031  not_a_file) == 1
-00033ad0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00033ae0: 2020 6d73 6720 3d20 6622 4e6f 2065 7869    msg = f"No exi
-00033af0: 7374 696e 6720 6669 6c65 2061 7420 7b6e  sting file at {n
-00033b00: 6f74 5f61 5f66 696c 655b 305d 7d2e 220a  ot_a_file[0]}.".
-00033b10: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00033b20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00033b30: 2020 6d73 6720 3d20 6622 5468 6573 6520    msg = f"These 
-00033b40: 6172 6520 6e6f 7420 7061 7468 7320 6f66  are not paths of
-00033b50: 2065 7869 7374 696e 6720 6669 6c65 733a   existing files:
-00033b60: 207b 6e6f 745f 615f 6669 6c65 7d22 0a20   {not_a_file}". 
-00033b70: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00033b80: 722e 7761 726e 696e 6728 6d73 6729 0a20  r.warning(msg). 
-00033b90: 2020 2020 2020 2020 2020 2072 6573 6f6c             resol
-00033ba0: 7665 645f 7061 7468 7320 3d20 5b70 2066  ved_paths = [p f
-00033bb0: 6f72 2070 2069 6e20 7265 736f 6c76 6564  or p in resolved
-00033bc0: 5f70 6174 6873 2069 6620 6f73 2e70 6174  _paths if os.pat
-00033bd0: 682e 6973 6669 6c65 2870 295d 0a20 2020  h.isfile(p)].   
-00033be0: 2065 6c73 653a 0a20 2020 2020 2020 206e   else:.        n
-00033bf0: 6f74 5f61 5f66 6f6c 6465 7220 3d20 5b70  ot_a_folder = [p
-00033c00: 2066 6f72 2070 2069 6e20 7265 736f 6c76   for p in resolv
-00033c10: 6564 5f70 6174 6873 2069 6620 6e6f 7420  ed_paths if not 
-00033c20: 6f73 2e70 6174 682e 6973 6469 7228 7029  os.path.isdir(p)
-00033c30: 5d0a 2020 2020 2020 2020 6966 206c 656e  ].        if len
-00033c40: 286e 6f74 5f61 5f66 6f6c 6465 7229 203e  (not_a_folder) >
-00033c50: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00033c60: 6966 206c 656e 286e 6f74 5f61 5f66 6f6c  if len(not_a_fol
-00033c70: 6465 7229 203d 3d20 313a 0a20 2020 2020  der) == 1:.     
-00033c80: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
-00033c90: 2066 227b 6e6f 745f 615f 666f 6c64 6572   f"{not_a_folder
-00033ca0: 5b30 5d7d 2069 7320 6e6f 7420 6120 7061  [0]} is not a pa
-00033cb0: 7468 2074 6f20 616e 2065 7869 7374 696e  th to an existin
-00033cc0: 6720 666f 6c64 6572 2e22 0a20 2020 2020  g folder.".     
-00033cd0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00033ce0: 2020 2020 2020 2020 2020 2020 206d 7367               msg
-00033cf0: 203d 2066 2254 6865 7365 2061 7265 206e   = f"These are n
-00033d00: 6f74 2070 6174 6873 206f 6620 6578 6973  ot paths of exis
-00033d10: 7469 6e67 2066 6f6c 6465 7273 3a20 7b6e  ting folders: {n
-00033d20: 6f74 5f61 5f66 6f6c 6465 727d 220a 2020  ot_a_folder}".  
-00033d30: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00033d40: 2e77 6172 6e69 6e67 286d 7367 290a 2020  .warning(msg).  
-00033d50: 2020 2020 2020 2020 2020 7265 736f 6c76            resolv
-00033d60: 6564 5f70 6174 6873 203d 205b 7020 666f  ed_paths = [p fo
-00033d70: 7220 7020 696e 2072 6573 6f6c 7665 645f  r p in resolved_
-00033d80: 7061 7468 7320 6966 206f 732e 7061 7468  paths if os.path
-00033d90: 2e69 7364 6972 2870 295d 0a20 2020 2072  .isdir(p)].    r
-00033da0: 6574 7572 6e20 7265 736f 6c76 6564 5f70  eturn resolved_p
-00033db0: 6174 6873 0a0a 4066 756e 6374 696f 6e5f  aths..@function_
-00033dc0: 6c6f 6767 6572 0a64 6566 2063 6f6d 7075  logger.def compu
-00033dd0: 7465 5f70 6174 685f 6672 6f6d 5f66 696c  te_path_from_fil
-00033de0: 6528 6669 6c65 3a20 4669 6c65 2c0a 2020  e(file: File,.  
-00033df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033e00: 2020 2020 2020 2020 2072 6f6f 745f 6469           root_di
-00033e10: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
-00033e20: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00033e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033e40: 2020 2020 666f 6c64 6572 3a20 4f70 7469      folder: Opti
-00033e50: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00033e60: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-00033e70: 220a 2020 2020 436f 6e73 7472 7563 7473  ".    Constructs
-00033e80: 2061 2070 6174 6820 6261 7365 6420 6f6e   a path based on
-00033e90: 2074 6865 2061 7267 756d 656e 7473 2e0a   the arguments..
-00033ea0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00033eb0: 2066 696c 653a 2054 6869 7320 6675 6e63   file: This func
-00033ec0: 7469 6f6e 2075 7365 7320 7468 6520 6669  tion uses the fi
-00033ed0: 656c 6473 2063 6f72 7075 735f 7061 7468  elds corpus_path
-00033ee0: 2c20 7375 6264 6972 2c20 616e 6420 7479  , subdir, and ty
-00033ef0: 7065 2e0a 2020 2020 2020 726f 6f74 5f64  pe..      root_d
-00033f00: 6972 3a0a 2020 2020 2020 2020 2020 4465  ir:.          De
-00033f10: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
-00033f20: 6d65 616e 696e 6720 7468 6174 2074 6865  meaning that the
-00033f30: 2070 6174 6820 6973 2063 6f6e 7374 7275   path is constru
-00033f40: 6374 6564 2062 6173 6564 206f 6e20 7468  cted based on th
-00033f50: 6520 636f 7270 7573 5f70 6174 682e 0a20  e corpus_path.. 
-00033f60: 2020 2020 2020 2020 2050 6173 7320 6120           Pass a 
-00033f70: 6469 7265 6374 6f72 7920 746f 2063 6f6e  directory to con
-00033f80: 7374 7275 6374 2074 6865 2070 6174 6820  struct the path 
-00033f90: 7265 6c61 7469 7665 2074 6f20 6974 2069  relative to it i
-00033fa0: 6e73 7465 6164 2e20 4966 2060 6066 6f6c  nstead. If ``fol
-00033fb0: 6465 7260 6020 6973 2061 6e20 6162 736f  der`` is an abso
-00033fc0: 6c75 7465 2070 6174 682c 0a20 2020 2020  lute path,.     
-00033fd0: 2020 2020 2060 6072 6f6f 745f 6469 7260       ``root_dir`
-00033fe0: 6020 6973 2069 676e 6f72 6564 2e0a 2020  ` is ignored..  
-00033ff0: 2020 2020 666f 6c64 6572 3a0a 2020 2020      folder:.    
-00034000: 2020 2020 2020 2a20 4966 2060 6066 6f6c        * If ``fol
-00034010: 6465 7260 6020 6973 204e 6f6e 6520 2864  der`` is None (d
-00034020: 6566 6175 6c74 292c 2074 6865 2066 696c  efault), the fil
-00034030: 6573 2720 7479 7065 2077 696c 6c20 6265  es' type will be
-00034040: 2061 7070 656e 6465 6420 746f 2074 6865   appended to the
-00034050: 2060 6072 6f6f 745f 6469 7260 602e 0a20   ``root_dir``.. 
-00034060: 2020 2020 2020 2020 202a 2049 6620 6060           * If ``
-00034070: 666f 6c64 6572 6060 2069 7320 616e 2061  folder`` is an a
-00034080: 6273 6f6c 7574 6520 7061 7468 2c20 6060  bsolute path, ``
-00034090: 726f 6f74 5f64 6972 6060 2077 696c 6c20  root_dir`` will 
-000340a0: 6265 2069 676e 6f72 6564 2e0a 2020 2020  be ignored..    
-000340b0: 2020 2020 2020 2a20 4966 2060 6066 6f6c        * If ``fol
-000340c0: 6465 7260 6020 6973 2061 2072 656c 6174  der`` is a relat
-000340d0: 6976 6520 7061 7468 2073 7461 7274 696e  ive path startin
-000340e0: 6720 7769 7468 2061 2064 6f74 2060 602e  g with a dot ``.
-000340f0: 6060 2074 6865 2072 656c 6174 6976 6520  `` the relative 
-00034100: 7061 7468 2069 7320 6170 7065 6e64 6564  path is appended
-00034110: 2074 6f20 7468 6520 6669 6c65 2773 2073   to the file's s
-00034120: 7562 6469 722e 0a20 2020 2020 2020 2020  ubdir..         
-00034130: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
-00034140: 6060 2e2e 5c6e 6f74 6573 6060 2077 696c  ``..\notes`` wil
-00034150: 6c20 7265 736f 6c76 6520 746f 2061 2073  l resolve to a s
-00034160: 6962 6c69 6e67 2064 6972 6563 746f 7279  ibling directory
-00034170: 206f 6620 7468 6520 6f6e 6520 7768 6572   of the one wher
-00034180: 6520 7468 6520 6060 6669 6c65 6060 2069  e the ``file`` i
-00034190: 7320 6c6f 6361 7465 642e 0a20 2020 2020  s located..     
-000341a0: 2020 2020 202a 2049 6620 6060 666f 6c64       * If ``fold
-000341b0: 6572 6060 2069 7320 6120 7265 6c61 7469  er`` is a relati
-000341c0: 7665 2070 6174 6820 7468 6174 2064 6f65  ve path that doe
-000341d0: 7320 6e6f 7420 6265 6769 6e20 7769 7468  s not begin with
-000341e0: 2061 2064 6f74 2060 602e 6060 2c20 6974   a dot ``.``, it
-000341f0: 2077 696c 6c20 6265 2061 7070 656e 6465   will be appende
-00034200: 6420 746f 2074 6865 0a20 2020 2020 2020  d to the.       
-00034210: 2020 2020 2060 6072 6f6f 745f 6469 7260       ``root_dir`
-00034220: 602e 0a20 2020 2020 2020 2020 202a 2049  `..          * I
-00034230: 6620 6060 666f 6c64 6572 6060 203d 3d20  f ``folder`` == 
-00034240: 2727 2028 656d 7074 7920 7374 7269 6e67  '' (empty string
-00034250: 292c 2074 6865 2072 6573 756c 7420 7769  ), the result wi
-00034260: 6c6c 2062 6520 6072 6f6f 745f 6469 7260  ll be `root_dir`
-00034270: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
-00034280: 2020 2020 2020 5468 6520 636f 6e73 7472        The constr
-00034290: 7563 7465 6420 6469 7265 6374 6f72 7920  ucted directory 
-000342a0: 7061 7468 2e0a 2020 2020 2222 220a 2020  path..    """.  
-000342b0: 2020 6966 2066 6f6c 6465 7220 6973 206e    if folder is n
-000342c0: 6f74 204e 6f6e 6520 616e 6420 286f 732e  ot None and (os.
-000342d0: 7061 7468 2e69 7361 6273 2866 6f6c 6465  path.isabs(folde
-000342e0: 7229 206f 7220 277e 2720 696e 2066 6f6c  r) or '~' in fol
-000342f0: 6465 7229 3a0a 2020 2020 2020 2020 666f  der):.        fo
-00034300: 6c64 6572 203d 2072 6573 6f6c 7665 5f64  lder = resolve_d
-00034310: 6972 2866 6f6c 6465 7229 0a20 2020 2020  ir(folder).     
-00034320: 2020 2070 6174 6820 3d20 666f 6c64 6572     path = folder
-00034330: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00034340: 2020 2072 6f6f 7420 3d20 6669 6c65 2e63     root = file.c
-00034350: 6f72 7075 735f 7061 7468 2069 6620 726f  orpus_path if ro
-00034360: 6f74 5f64 6972 2069 7320 4e6f 6e65 2065  ot_dir is None e
-00034370: 6c73 6520 7265 736f 6c76 655f 6469 7228  lse resolve_dir(
-00034380: 726f 6f74 5f64 6972 290a 2020 2020 2020  root_dir).      
-00034390: 2020 6966 2066 6f6c 6465 7220 6973 204e    if folder is N
-000343a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000343b0: 2070 6174 6820 3d20 6f73 2e70 6174 682e   path = os.path.
-000343c0: 6a6f 696e 2872 6f6f 742c 2066 696c 652e  join(root, file.
-000343d0: 7479 7065 290a 2020 2020 2020 2020 656c  type).        el
-000343e0: 6966 2066 6f6c 6465 7220 3d3d 2027 273a  if folder == '':
-000343f0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-00034400: 6820 3d20 726f 6f74 0a20 2020 2020 2020  h = root.       
-00034410: 2065 6c69 6620 666f 6c64 6572 5b30 5d20   elif folder[0] 
-00034420: 3d3d 2027 2e27 3a0a 2020 2020 2020 2020  == '.':.        
-00034430: 2020 2020 7061 7468 203d 206f 732e 7061      path = os.pa
-00034440: 7468 2e61 6273 7061 7468 286f 732e 7061  th.abspath(os.pa
-00034450: 7468 2e6a 6f69 6e28 726f 6f74 2c20 6669  th.join(root, fi
-00034460: 6c65 2e73 7562 6469 722c 2066 6f6c 6465  le.subdir, folde
-00034470: 7229 290a 2020 2020 2020 2020 656c 7365  r)).        else
-00034480: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00034490: 7468 203d 206f 732e 7061 7468 2e61 6273  th = os.path.abs
-000344a0: 7061 7468 286f 732e 7061 7468 2e6a 6f69  path(os.path.joi
-000344b0: 6e28 726f 6f74 2c20 666f 6c64 6572 2929  n(root, folder))
-000344c0: 0a20 2020 2072 6574 7572 6e20 7061 7468  .    return path
-000344d0: 0a0a 6465 6620 6d61 6b65 5f66 696c 655f  ..def make_file_
-000344e0: 7061 7468 2866 696c 653a 2046 696c 652c  path(file: File,
-000344f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00034500: 2020 2020 726f 6f74 5f64 6972 3d4e 6f6e      root_dir=Non
-00034510: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00034520: 2020 2020 2020 666f 6c64 6572 3a20 7374        folder: st
-00034530: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00034540: 2020 2020 2020 2020 2020 2020 2073 7566               suf
-00034550: 6669 783a 2073 7472 203d 2027 272c 0a20  fix: str = '',. 
-00034560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034570: 2020 6665 7874 3a20 7374 7220 3d20 272e    fext: str = '.
-00034580: 7473 7627 293a 0a20 2020 2022 2222 2043  tsv'):.    """ C
-00034590: 6f6e 7374 7275 6374 7320 6120 6669 6c65  onstructs a file
-000345a0: 2070 6174 6820 6261 7365 6420 6f6e 2074   path based on t
-000345b0: 6865 2061 7267 756d 656e 7473 2e0a 0a20  he arguments... 
-000345c0: 2020 2041 7267 733a 0a20 2020 2020 2066     Args:.      f
-000345d0: 696c 653a 2054 6869 7320 6675 6e63 7469  ile: This functi
-000345e0: 6f6e 2075 7365 7320 7468 6520 6669 656c  on uses the fiel
-000345f0: 6473 2066 6e61 6d65 2c20 636f 7270 7573  ds fname, corpus
-00034600: 5f70 6174 682c 2073 7562 6469 722c 2061  _path, subdir, a
-00034610: 6e64 2074 7970 652e 0a20 2020 2020 2072  nd type..      r
-00034620: 6f6f 745f 6469 723a 0a20 2020 2020 2020  oot_dir:.       
-00034630: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00034640: 652c 206d 6561 6e69 6e67 2074 6861 7420  e, meaning that 
-00034650: 7468 6520 7061 7468 2069 7320 636f 6e73  the path is cons
-00034660: 7472 7563 7465 6420 6261 7365 6420 6f6e  tructed based on
-00034670: 2074 6865 2063 6f72 7075 735f 7061 7468   the corpus_path
-00034680: 2e0a 2020 2020 2020 2020 5061 7373 2061  ..        Pass a
-00034690: 2064 6972 6563 746f 7279 2074 6f20 636f   directory to co
-000346a0: 6e73 7472 7563 7420 7468 6520 7061 7468  nstruct the path
-000346b0: 2072 656c 6174 6976 6520 746f 2069 7420   relative to it 
-000346c0: 696e 7374 6561 642e 2049 6620 6060 666f  instead. If ``fo
-000346d0: 6c64 6572 6060 2069 7320 616e 2061 6273  lder`` is an abs
-000346e0: 6f6c 7574 6520 7061 7468 2c0a 2020 2020  olute path,.    
-000346f0: 2020 2020 6060 726f 6f74 5f64 6972 6060      ``root_dir``
-00034700: 2069 7320 6967 6e6f 7265 642e 0a20 2020   is ignored..   
-00034710: 2020 2066 6f6c 6465 723a 0a20 2020 2020     folder:.     
-00034720: 2020 2044 6966 6665 7265 6e74 2062 6568     Different beh
-00034730: 6176 696f 7572 7320 6172 6520 6176 6169  aviours are avai
-00034740: 6c61 626c 652e 204e 6f74 6520 7468 6174  lable. Note that
-00034750: 206f 6e6c 7920 7468 6520 7468 6972 6420   only the third 
-00034760: 6f70 7469 6f6e 2065 6e73 7572 6573 2074  option ensures t
-00034770: 6861 7420 6669 6c65 2070 6174 6873 2061  hat file paths a
-00034780: 7265 2064 6973 7469 6e63 7420 666f 720a  re distinct for.
-00034790: 2020 2020 2020 2020 6669 6c65 7320 7468          files th
-000347a0: 6174 2068 6176 6520 6964 656e 7469 6361  at have identica
-000347b0: 6c20 666e 616d 6573 2062 7574 2061 7265  l fnames but are
-000347c0: 206c 6f63 6174 6564 2069 6e20 6469 6666   located in diff
-000347d0: 6572 656e 7420 7375 6264 6972 6563 746f  erent subdirecto
-000347e0: 7269 6573 206f 6620 7468 6520 7361 6d65  ries of the same
-000347f0: 2063 6f72 7075 732e 0a20 2020 2020 2020   corpus..       
-00034800: 202a 2049 6620 6060 666f 6c64 6572 6060   * If ``folder``
-00034810: 2069 7320 4e6f 6e65 2028 6465 6661 756c   is None (defaul
-00034820: 7429 2c20 7468 6520 6669 6c65 7327 2074  t), the files' t
-00034830: 7970 6520 7769 6c6c 2062 6520 6170 7065  ype will be appe
-00034840: 6e64 6564 2074 6f20 7468 6520 6060 726f  nded to the ``ro
-00034850: 6f74 5f64 6972 6060 2e0a 2020 2020 2020  ot_dir``..      
-00034860: 2020 2a20 4966 2060 6066 6f6c 6465 7260    * If ``folder`
-00034870: 6020 6973 2061 6e20 6162 736f 6c75 7465  ` is an absolute
-00034880: 2070 6174 682c 2060 6072 6f6f 745f 6469   path, ``root_di
-00034890: 7260 6020 7769 6c6c 2062 6520 6967 6e6f  r`` will be igno
-000348a0: 7265 642e 0a20 2020 2020 2020 202a 2049  red..        * I
-000348b0: 6620 6060 666f 6c64 6572 6060 2069 7320  f ``folder`` is 
-000348c0: 6120 7265 6c61 7469 7665 2070 6174 6820  a relative path 
-000348d0: 7374 6172 7469 6e67 2077 6974 6820 6120  starting with a 
-000348e0: 646f 7420 6060 2e60 6020 7468 6520 7265  dot ``.`` the re
-000348f0: 6c61 7469 7665 2070 6174 6820 6973 2061  lative path is a
-00034900: 7070 656e 6465 6420 746f 2074 6865 2066  ppended to the f
-00034910: 696c 6527 7320 7375 6264 6972 2e0a 2020  ile's subdir..  
-00034920: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
-00034930: 706c 652c 2060 602e 2e5c 6e6f 7465 7360  ple, ``..\notes`
-00034940: 6020 7769 6c6c 2072 6573 6f6c 7665 2074  ` will resolve t
-00034950: 6f20 6120 7369 626c 696e 6720 6469 7265  o a sibling dire
-00034960: 6374 6f72 7920 6f66 2074 6865 206f 6e65  ctory of the one
-00034970: 2077 6865 7265 2074 6865 2060 6066 696c   where the ``fil
-00034980: 6560 6020 6973 206c 6f63 6174 6564 2e0a  e`` is located..
-00034990: 2020 2020 2020 2020 2a20 4966 2060 6066          * If ``f
-000349a0: 6f6c 6465 7260 6020 6973 2061 2072 656c  older`` is a rel
-000349b0: 6174 6976 6520 7061 7468 2074 6861 7420  ative path that 
-000349c0: 646f 6573 206e 6f74 2062 6567 696e 2077  does not begin w
-000349d0: 6974 6820 6120 646f 7420 6060 2e60 602c  ith a dot ``.``,
-000349e0: 2069 7420 7769 6c6c 2062 6520 6170 7065   it will be appe
-000349f0: 6e64 6564 2074 6f20 7468 650a 2020 2020  nded to the.    
-00034a00: 2020 2020 2020 6060 726f 6f74 5f64 6972        ``root_dir
-00034a10: 6060 2e0a 2020 2020 2020 7375 6666 6978  ``..      suffix
-00034a20: 3a20 5374 7269 6e67 2074 6f20 6170 7065  : String to appe
-00034a30: 6e64 2074 6f20 7468 6520 6669 6c65 2773  nd to the file's
-00034a40: 2066 6e61 6d65 2e0a 2020 2020 2020 6665   fname..      fe
-00034a50: 7874 3a20 4669 6c65 2065 7874 656e 7369  xt: File extensi
-00034a60: 6f6e 2074 6f20 6170 7065 6e64 2074 6f20  on to append to 
-00034a70: 7468 6520 2866 6e61 6d65 2b73 7566 6669  the (fname+suffi
-00034a80: 7829 2e20 4465 6661 756c 7473 2074 6f20  x). Defaults to 
-00034a90: 6060 2e74 7376 6060 2e0a 0a20 2020 2052  ``.tsv``...    R
-00034aa0: 6574 7572 6e73 3a0a 2020 2020 2020 5468  eturns:.      Th
-00034ab0: 6520 636f 6e73 7472 7563 7465 6420 6669  e constructed fi
-00034ac0: 6c65 2070 6174 682e 0a20 2020 2022 2222  le path..    """
-00034ad0: 0a20 2020 2061 7373 6572 7420 6665 7874  .    assert fext
-00034ae0: 2069 7320 6e6f 7420 4e6f 6e65 2c20 2222   is not None, ""
-00034af0: 0a20 2020 2070 6174 6820 3d20 636f 6d70  .    path = comp
-00034b00: 7574 655f 7061 7468 5f66 726f 6d5f 6669  ute_path_from_fi
-00034b10: 6c65 2866 696c 652c 2072 6f6f 745f 6469  le(file, root_di
-00034b20: 723d 726f 6f74 5f64 6972 2c20 666f 6c64  r=root_dir, fold
-00034b30: 6572 3d66 6f6c 6465 7229 0a20 2020 2069  er=folder).    i
-00034b40: 6620 7375 6666 6978 2069 7320 4e6f 6e65  f suffix is None
-00034b50: 3a0a 2020 2020 2020 2020 7375 6666 6978  :.        suffix
-00034b60: 203d 2027 270a 2020 2020 666e 616d 6520   = ''.    fname 
-00034b70: 3d20 6669 6c65 2e66 6e61 6d65 202b 2073  = file.fname + s
-00034b80: 7566 6669 7820 2b20 6665 7874 0a20 2020  uffix + fext.   
-00034b90: 2072 6574 7572 6e20 6f73 2e70 6174 682e   return os.path.
-00034ba0: 6a6f 696e 2870 6174 682c 2066 6e61 6d65  join(path, fname
-00034bb0: 290a 0a64 6566 2073 7472 696e 6732 6964  )..def string2id
-00034bc0: 656e 7469 6669 6572 2873 3a20 7374 722c  entifier(s: str,
-00034bd0: 2072 656d 6f76 655f 6c65 6164 696e 675f   remove_leading_
-00034be0: 756e 6465 7273 636f 7265 3a20 626f 6f6c  underscore: bool
-00034bf0: 203d 2054 7275 6529 202d 3e20 7374 723a   = True) -> str:
-00034c00: 0a20 2020 2022 2222 5472 616e 7366 6f72  .    """Transfor
-00034c10: 6d20 6120 7374 7269 6e67 2069 6e20 6120  m a string in a 
-00034c20: 7761 7920 7468 6174 2069 7420 6361 6e20  way that it can 
-00034c30: 6265 2075 7365 6420 6173 2069 6465 6e74  be used as ident
-00034c40: 6966 6965 7220 2876 6172 6961 626c 6520  ifier (variable 
-00034c50: 6f72 2061 7474 7269 6275 7465 206e 616d  or attribute nam
-00034c60: 6529 2e0a 2020 2020 536f 6c75 7469 6f6e  e)..    Solution
-00034c70: 2062 7920 4b65 6e61 6e20 4261 6e6b 7320   by Kenan Banks 
-00034c80: 6f6e 2068 7474 7073 3a2f 2f73 7461 636b  on https://stack
-00034c90: 6f76 6572 666c 6f77 2e63 6f6d 2f61 2f33  overflow.com/a/3
-00034ca0: 3330 3333 3631 0a20 2020 2022 2222 0a20  303361.    """. 
-00034cb0: 2020 2023 2052 656d 6f76 6520 696e 7661     # Remove inva
-00034cc0: 6c69 6420 6368 6172 6163 7465 7273 0a20  lid characters. 
-00034cd0: 2020 2073 203d 2072 652e 7375 6228 275b     s = re.sub('[
-00034ce0: 5e30 2d39 612d 7a41 2d5a 5f5d 272c 2027  ^0-9a-zA-Z_]', '
-00034cf0: 272c 2073 290a 0a20 2020 2023 2052 656d  ', s)..    # Rem
-00034d00: 6f76 6520 6c65 6164 696e 6720 6368 6172  ove leading char
-00034d10: 6163 7465 7273 2075 6e74 696c 2077 6520  acters until we 
-00034d20: 6669 6e64 2061 206c 6574 7465 7220 6f72  find a letter or
-00034d30: 2075 6e64 6572 7363 6f72 650a 2020 2020   underscore.    
-00034d40: 7265 6765 7820 3d20 275e 5b5e 612d 7a41  regex = '^[^a-zA
-00034d50: 2d5a 5d2b 2720 6966 2072 656d 6f76 655f  -Z]+' if remove_
-00034d60: 6c65 6164 696e 675f 756e 6465 7273 636f  leading_undersco
-00034d70: 7265 2065 6c73 6520 275e 5b5e 612d 7a41  re else '^[^a-zA
-00034d80: 2d5a 5f5d 2b27 0a20 2020 2073 203d 2072  -Z_]+'.    s = r
-00034d90: 652e 7375 6228 7265 6765 782c 2027 272c  e.sub(regex, '',
-00034da0: 2073 290a 0a20 2020 2072 6574 7572 6e20   s)..    return 
-00034db0: 730a 0a40 6c72 755f 6361 6368 6528 290a  s..@lru_cache().
-00034dc0: 4066 756e 6374 696f 6e5f 6c6f 6767 6572  @function_logger
-00034dd0: 0a64 6566 2067 6574 5f67 6974 5f63 6f6d  .def get_git_com
-00034de0: 6d69 7428 7265 706f 5f70 6174 683a 2073  mit(repo_path: s
-00034df0: 7472 2c20 6769 745f 7265 7669 7369 6f6e  tr, git_revision
-00034e00: 3a20 7374 7229 202d 3e20 4f70 7469 6f6e  : str) -> Option
-00034e10: 616c 5b67 6974 2e43 6f6d 6d69 745d 3a0a  al[git.Commit]:.
-00034e20: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00034e30: 2072 6570 6f20 3d20 6769 742e 5265 706f   repo = git.Repo
-00034e40: 2872 6570 6f5f 7061 7468 2c20 7365 6172  (repo_path, sear
-00034e50: 6368 5f70 6172 656e 745f 6469 7265 6374  ch_parent_direct
-00034e60: 6f72 6965 733d 5472 7565 290a 2020 2020  ories=True).    
-00034e70: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00034e80: 2061 7320 653a 0a20 2020 2020 2020 206c   as e:.        l
-00034e90: 6f67 6765 722e 6572 726f 7228 6622 7b72  ogger.error(f"{r
-00034ea0: 6570 6f5f 7061 7468 7d20 6973 206e 6f74  epo_path} is not
-00034eb0: 2061 6e20 6578 6973 7469 6e67 2067 6974   an existing git
-00034ec0: 2072 6570 6f73 6974 6f72 793a 207b 657d   repository: {e}
-00034ed0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00034ee0: 6e0a 2020 2020 7472 793a 0a20 2020 2020  n.    try:.     
-00034ef0: 2020 2072 6574 7572 6e20 7265 706f 2e63     return repo.c
-00034f00: 6f6d 6d69 7428 6769 745f 7265 7669 7369  ommit(git_revisi
-00034f10: 6f6e 290a 2020 2020 6578 6365 7074 2042  on).    except B
-00034f20: 6164 4e61 6d65 3a0a 2020 2020 2020 2020  adName:.        
-00034f30: 6c6f 6767 6572 2e65 7272 6f72 2866 227b  logger.error(f"{
-00034f40: 6769 745f 7265 7669 7369 6f6e 7d20 646f  git_revision} do
-00034f50: 6573 206e 6f74 2072 6573 6f6c 7665 2074  es not resolve t
-00034f60: 6f20 6120 636f 6d6d 6974 2066 6f72 2072  o a commit for r
-00034f70: 6570 6f20 7b6f 732e 7061 7468 2e62 6173  epo {os.path.bas
-00034f80: 656e 616d 6528 7265 706f 5f70 6174 6829  ename(repo_path)
-00034f90: 7d2e 2229 0a0a 0a40 6675 6e63 7469 6f6e  }.")...@function
-00034fa0: 5f6c 6f67 6765 720a 6465 6620 7061 7273  _logger.def pars
-00034fb0: 655f 7473 765f 6669 6c65 5f61 745f 6769  e_tsv_file_at_gi
-00034fc0: 745f 7265 7669 7369 6f6e 2866 696c 653a  t_revision(file:
-00034fd0: 2046 696c 652c 0a20 2020 2020 2020 2020   File,.         
-00034fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034ff0: 2020 2020 2020 2020 2020 6769 745f 7265            git_re
-00035000: 7669 7369 6f6e 3a20 7374 722c 0a20 2020  vision: str,.   
-00035010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032620: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00032630: 655f 6d65 616e 735f 616c 6c3a 2062 6f6f  e_means_all: boo
+00032640: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+00032650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032660: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+00032670: 3e20 4f70 7469 6f6e 616c 5b4c 6973 745b  > Optional[List[
+00032680: 7374 725d 5d3a 0a20 2020 2022 2222 204d  str]]:.    """ M
+00032690: 616b 6573 2073 7572 6520 7468 6174 2061  akes sure that a
+000326a0: 6e20 696e 7075 7420 7661 6c75 6520 6973  n input value is
+000326b0: 2061 206c 6973 7420 6f66 2073 7472 696e   a list of strin
+000326c0: 6773 2061 6e64 2074 6861 7420 616c 6c20  gs and that all 
+000326d0: 7374 7269 6e67 7320 6172 6520 7661 6c69  strings are vali
+000326e0: 6420 772e 722e 742e 2074 6f0a 2020 2020  d w.r.t. to.    
+000326f0: 7468 6520 7479 7065 2773 2065 7870 6563  the type's expec
+00032700: 7465 6420 6c69 7465 7261 6c20 7661 6c75  ted literal valu
+00032710: 6573 2028 7374 7269 6e67 7329 2e0a 0a20  es (strings)... 
+00032720: 2020 2041 7267 733a 0a20 2020 2020 2061     Args:.      a
+00032730: 7267 756d 656e 743a 0a20 2020 2020 2020  rgument:.       
+00032740: 2020 2049 6620 7374 7269 6e67 2c20 7772     If string, wr
+00032750: 6170 7065 6420 696e 2061 206c 6973 742c  apped in a list,
+00032760: 206f 7468 6572 7769 7365 2065 7870 6563   otherwise expec
+00032770: 7465 6420 746f 2062 6520 6120 7475 706c  ted to be a tupl
+00032780: 6520 6f66 2073 7472 696e 6773 2028 7061  e of strings (pa
+00032790: 7373 696e 6720 6120 6c69 7374 2077 696c  ssing a list wil
+000327a0: 6c20 6661 696c 292e 0a20 2020 2020 2020  l fail)..       
+000327b0: 2020 2049 6620 4e6f 6e65 2c20 6120 6c69     If None, a li
+000327c0: 7374 206f 6620 616c 6c20 706f 7373 6962  st of all possib
+000327d0: 6c65 2076 616c 7565 7320 6163 636f 7264  le values accord
+000327e0: 696e 6720 746f 2074 6865 2074 7970 6520  ing to the type 
+000327f0: 6973 2072 6574 7572 6e65 6420 6966 206e  is returned if n
+00032800: 6f6e 655f 6d65 616e 735f 616c 6c2e 0a20  one_means_all.. 
+00032810: 2020 2020 2074 7970 3a0a 2020 2020 2020       typ:.      
+00032820: 2020 2020 4120 7479 7069 6e67 2e4c 6974      A typing.Lit
+00032830: 6572 616c 2064 6563 6c61 7261 7469 6f6e  eral declaration
+00032840: 206f 7220 6120 5479 7065 5661 7220 7768   or a TypeVar wh
+00032850: 6572 6520 7468 6520 6669 7273 7420 636f  ere the first co
+00032860: 6d70 6f6e 656e 7420 6973 206f 6e65 2c20  mponent is one, 
+00032870: 6f72 2061 2074 7570 6c65 206f 6620 616c  or a tuple of al
+00032880: 6c6f 7765 6420 7661 6c75 6573 2e0a 2020  lowed values..  
+00032890: 2020 2020 2020 2020 416c 6c20 616c 6c6f          All allo
+000328a0: 7765 6420 7661 6c75 6573 2073 686f 756c  wed values shoul
+000328b0: 6420 6265 2073 7472 696e 6773 2e0a 2020  d be strings..  
+000328c0: 2020 2020 6e6f 6e65 5f6d 6561 6e73 5f61      none_means_a
+000328d0: 6c6c 3a0a 2020 2020 2020 2020 2020 4279  ll:.          By
+000328e0: 2064 6566 6175 6c74 2c20 4e6f 6e65 2076   default, None v
+000328f0: 616c 7565 7320 6172 6520 7265 706c 6163  alues are replac
+00032900: 6564 2077 6974 6820 616c 6c20 616c 6c6f  ed with all allo
+00032910: 7765 6420 7661 6c75 6573 2c20 6966 2073  wed values, if s
+00032920: 7065 6369 6669 6564 2e0a 2020 2020 2020  pecified..      
+00032930: 2020 2020 5061 7373 2046 616c 7365 2074      Pass False t
+00032940: 6f20 7265 7475 726e 204e 6f6e 6520 696e  o return None in
+00032950: 2074 6869 7320 6361 7365 2e0a 0a20 2020   this case...   
+00032960: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00032970: 5468 6520 6c69 7374 206f 6620 6163 6365  The list of acce
+00032980: 7074 6564 2073 7472 696e 6773 2e0a 2020  pted strings..  
+00032990: 2020 2020 5468 6520 6c69 7374 206f 6620      The list of 
+000329a0: 7265 6a65 6374 6564 2073 7472 696e 6773  rejected strings
+000329b0: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
+000329c0: 2074 7970 2069 7320 4e6f 6e65 3a0a 2020   typ is None:.  
+000329d0: 2020 2020 2020 616c 6c6f 7765 6420 3d20        allowed = 
+000329e0: 4e6f 6e65 0a20 2020 2065 6c73 653a 0a20  None.    else:. 
+000329f0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00032a00: 616e 6365 2874 7970 2c20 7475 706c 6529  ance(typ, tuple)
+00032a10: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+00032a20: 6c6f 7765 6420 3d20 7479 700a 2020 2020  lowed = typ.    
+00032a30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00032a40: 2020 2020 2020 616c 6c6f 7765 6420 3d20        allowed = 
+00032a50: 6c69 7465 7261 6c5f 7479 7065 3274 7570  literal_type2tup
+00032a60: 6c65 2874 7970 290a 2020 2020 6966 2061  le(typ).    if a
+00032a70: 7267 756d 656e 7420 6973 204e 6f6e 653a  rgument is None:
+00032a80: 0a20 2020 2020 2020 2069 6620 6e6f 6e65  .        if none
+00032a90: 5f6d 6561 6e73 5f61 6c6c 2061 6e64 2061  _means_all and a
+00032aa0: 6c6c 6f77 6564 2069 7320 6e6f 7420 4e6f  llowed is not No
+00032ab0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00032ac0: 7265 7475 726e 206c 6973 7428 616c 6c6f  return list(allo
+00032ad0: 7765 6429 0a20 2020 2020 2020 2065 6c73  wed).        els
+00032ae0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00032af0: 6574 7572 6e0a 2020 2020 6966 2069 7369  eturn.    if isi
+00032b00: 6e73 7461 6e63 6528 6172 6775 6d65 6e74  nstance(argument
+00032b10: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+00032b20: 6172 6775 6d65 6e74 203d 205b 6172 6775  argument = [argu
+00032b30: 6d65 6e74 5d0a 2020 2020 6966 2061 6c6c  ment].    if all
+00032b40: 6f77 6564 2069 7320 4e6f 6e65 3a0a 2020  owed is None:.  
+00032b50: 2020 2020 2020 7265 7475 726e 2061 7267        return arg
+00032b60: 756d 656e 740a 2020 2020 656c 7365 3a0a  ument.    else:.
+00032b70: 2020 2020 2020 2020 7369 6e67 756c 6172          singular
+00032b80: 5f64 6963 7420 3d20 7b61 6c6c 7764 5b3a  _dict = {allwd[:
+00032b90: 2d31 5d3a 2061 6c6c 7764 2066 6f72 2061  -1]: allwd for a
+00032ba0: 6c6c 7764 2069 6e20 616c 6c6f 7765 647d  llwd in allowed}
+00032bb0: 0a20 2020 2061 6363 6570 7465 642c 2072  .    accepted, r
+00032bc0: 656a 6563 7465 6420 3d20 5b5d 2c20 5b5d  ejected = [], []
+00032bd0: 0a20 2020 2066 6f72 2061 7267 2069 6e20  .    for arg in 
+00032be0: 6172 6775 6d65 6e74 3a0a 2020 2020 2020  argument:.      
+00032bf0: 2020 6966 2061 7267 2069 6e20 616c 6c6f    if arg in allo
+00032c00: 7765 643a 0a20 2020 2020 2020 2020 2020  wed:.           
+00032c10: 2061 6363 6570 7465 642e 6170 7065 6e64   accepted.append
+00032c20: 2861 7267 290a 2020 2020 2020 2020 656c  (arg).        el
+00032c30: 6966 2061 7267 2069 6e20 7369 6e67 756c  if arg in singul
+00032c40: 6172 5f64 6963 743a 0a20 2020 2020 2020  ar_dict:.       
+00032c50: 2020 2020 2061 6363 6570 7465 642e 6170       accepted.ap
+00032c60: 7065 6e64 2873 696e 6775 6c61 725f 6469  pend(singular_di
+00032c70: 6374 5b61 7267 5d29 0a20 2020 2020 2020  ct[arg]).       
+00032c80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00032c90: 2020 2072 656a 6563 7465 642e 6170 7065     rejected.appe
+00032ca0: 6e64 2861 7267 290a 2020 2020 6e5f 7265  nd(arg).    n_re
+00032cb0: 6a65 6374 6564 203d 206c 656e 2872 656a  jected = len(rej
+00032cc0: 6563 7465 6429 0a20 2020 2069 6620 6e5f  ected).    if n_
+00032cd0: 7265 6a65 6374 6564 203e 2030 3a0a 2020  rejected > 0:.  
+00032ce0: 2020 2020 2020 6966 206e 5f72 656a 6563        if n_rejec
+00032cf0: 7465 6420 3d3d 2031 3a0a 2020 2020 2020  ted == 1:.      
+00032d00: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+00032d10: 6e69 6e67 2866 2254 6869 7320 6973 206e  ning(f"This is n
+00032d20: 6f74 2061 6e20 6163 6365 7074 6564 2076  ot an accepted v
+00032d30: 616c 7565 3a20 7b72 656a 6563 7465 645b  alue: {rejected[
+00032d40: 305d 7d5c 6e22 0a20 2020 2020 2020 2020  0]}\n".         
+00032d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032d60: 2020 6622 4368 6f6f 7365 2066 726f 6d20    f"Choose from 
+00032d70: 7b61 6c6c 6f77 6564 7d22 290a 2020 2020  {allowed}").    
+00032d80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00032d90: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+00032da0: 6e69 6e67 2866 2254 6865 7365 2061 7265  ning(f"These are
+00032db0: 206e 6f74 2061 6363 6570 7465 6420 7661   not accepted va
+00032dc0: 6c75 652c 206f 6e6c 793a 207b 7265 6a65  lue, only: {reje
+00032dd0: 6374 6564 7d22 0a20 2020 2020 2020 2020  cted}".         
+00032de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032df0: 2020 6622 4368 6f6f 7365 2066 726f 6d20    f"Choose from 
+00032e00: 7b61 6c6c 6f77 6564 7d22 290a 2020 2020  {allowed}").    
+00032e10: 6966 206c 656e 2861 6363 6570 7465 6429  if len(accepted)
+00032e20: 203e 2030 3a0a 2020 2020 2020 2020 7265   > 0:.        re
+00032e30: 7475 726e 2061 6363 6570 7465 640a 2020  turn accepted.  
+00032e40: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
+00032e50: 2866 2250 6173 7320 6174 206c 6561 7374  (f"Pass at least
+00032e60: 206f 6e65 206f 6620 7b61 6c6c 6f77 6564   one of {allowed
+00032e70: 7d2e 2229 0a20 2020 2072 6574 7572 6e0a  }.").    return.
+00032e80: 0a4c 203d 2054 7970 6556 6172 2827 4c27  .L = TypeVar('L'
+00032e90: 290a 0a40 6675 6e63 7469 6f6e 5f6c 6f67  )..@function_log
+00032ea0: 6765 720a 6465 6620 6368 6563 6b5f 6172  ger.def check_ar
+00032eb0: 6775 6d65 6e74 5f61 6761 696e 7374 5f6c  gument_against_l
+00032ec0: 6974 6572 616c 5f74 7970 6528 6172 6775  iteral_type(argu
+00032ed0: 6d65 6e74 3a20 7374 722c 0a20 2020 2020  ment: str,.     
+00032ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032f00: 2020 2074 7970 3a20 4c29 202d 3e20 4f70     typ: L) -> Op
+00032f10: 7469 6f6e 616c 5b4c 5d3a 0a20 2020 2069  tional[L]:.    i
+00032f20: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00032f30: 2861 7267 756d 656e 742c 2073 7472 293a  (argument, str):
+00032f40: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00032f50: 7761 726e 696e 6728 6622 4172 6775 6d65  warning(f"Argume
+00032f60: 6e74 206e 6565 6473 2074 6f20 6265 2061  nt needs to be a
+00032f70: 2073 7472 696e 672c 206e 6f74 2027 7b74   string, not '{t
+00032f80: 7970 6528 6172 6775 6d65 6e74 297d 2722  ype(argument)}'"
+00032f90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00032fa0: 204e 6f6e 650a 2020 2020 616c 6c6f 7765   None.    allowe
+00032fb0: 6420 3d20 6c69 7465 7261 6c5f 7479 7065  d = literal_type
+00032fc0: 3274 7570 6c65 2874 7970 290a 2020 2020  2tuple(typ).    
+00032fd0: 7369 6e67 756c 6172 5f64 6963 7420 3d20  singular_dict = 
+00032fe0: 7b61 6c6c 7764 5b3a 2d31 5d3a 2061 6c6c  {allwd[:-1]: all
+00032ff0: 7764 2066 6f72 2061 6c6c 7764 2069 6e20  wd for allwd in 
+00033000: 616c 6c6f 7765 647d 0a20 2020 2069 6620  allowed}.    if 
+00033010: 6172 6775 6d65 6e74 206e 6f74 2069 6e20  argument not in 
+00033020: 616c 6c6f 7765 6420 616e 6420 6172 6775  allowed and argu
+00033030: 6d65 6e74 206e 6f74 2069 6e20 7369 6e67  ment not in sing
+00033040: 756c 6172 5f64 6963 743a 0a20 2020 2020  ular_dict:.     
+00033050: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+00033060: 6728 6622 496e 7661 6c69 6420 6172 6775  g(f"Invalid argu
+00033070: 6d65 6e74 2027 7b61 7267 756d 656e 747d  ment '{argument}
+00033080: 272e 2050 6173 7320 6f6e 6520 6f66 207b  '. Pass one of {
+00033090: 616c 6c6f 7765 647d 2229 0a20 2020 2020  allowed}").     
+000330a0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+000330b0: 2020 2069 6620 6172 6775 6d65 6e74 2069     if argument i
+000330c0: 6e20 7369 6e67 756c 6172 5f64 6963 743a  n singular_dict:
+000330d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000330e0: 7369 6e67 756c 6172 5f64 6963 745b 6172  singular_dict[ar
+000330f0: 6775 6d65 6e74 5d0a 2020 2020 7265 7475  gument].    retu
+00033100: 726e 2061 7267 756d 656e 740a 0a40 6675  rn argument..@fu
+00033110: 6e63 7469 6f6e 5f6c 6f67 6765 720a 6465  nction_logger.de
+00033120: 6620 7265 736f 6c76 655f 6661 6365 7473  f resolve_facets
+00033130: 5f70 6172 616d 2866 6163 6574 732c 2066  _param(facets, f
+00033140: 6163 6574 5f74 7970 655f 7661 723a 2054  acet_type_var: T
+00033150: 7970 6556 6172 203d 2046 6163 6574 2c20  ypeVar = Facet, 
+00033160: 6e6f 6e65 5f6d 6561 6e73 5f61 6c6c 3d54  none_means_all=T
+00033170: 7275 6529 3a0a 2020 2020 2222 224c 696b  rue):.    """Lik
+00033180: 6520 3a66 756e 633a 6061 7267 756d 656e  e :func:`argumen
+00033190: 745f 616e 645f 6c69 7465 7261 6c5f 7479  t_and_literal_ty
+000331a0: 7065 326c 6973 7460 2c20 6275 7420 616c  pe2list`, but al
+000331b0: 736f 2072 6573 6f6c 7665 7320 2774 7376  so resolves 'tsv
+000331c0: 2720 746f 2061 6c6c 206e 6f6e 2d73 636f  ' to all non-sco
+000331d0: 7265 2066 6163 6574 732e 2222 220a 2020  re facets.""".  
+000331e0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000331f0: 6661 6365 7473 2c20 7374 7229 2061 6e64  facets, str) and
+00033200: 2066 6163 6574 7320 696e 2028 2774 7376   facets in ('tsv
+00033210: 272c 2027 7473 7673 2729 3a0a 2020 2020  ', 'tsvs'):.    
+00033220: 2020 2020 7365 6c65 6374 6564 5f66 6163      selected_fac
+00033230: 6574 7320 3d20 6c69 7374 286c 6974 6572  ets = list(liter
+00033240: 616c 5f74 7970 6532 7475 706c 6528 6661  al_type2tuple(fa
+00033250: 6365 745f 7479 7065 5f76 6172 2929 0a20  cet_type_var)). 
+00033260: 2020 2020 2020 2069 6620 2773 636f 7265         if 'score
+00033270: 7327 2069 6e20 7365 6c65 6374 6564 5f66  s' in selected_f
+00033280: 6163 6574 733a 0a20 2020 2020 2020 2020  acets:.         
+00033290: 2020 2073 656c 6563 7465 645f 6661 6365     selected_face
+000332a0: 7473 2e72 656d 6f76 6528 2773 636f 7265  ts.remove('score
+000332b0: 7327 290a 2020 2020 656c 7365 3a0a 2020  s').    else:.  
+000332c0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+000332d0: 6e63 6528 6661 6365 7473 2c20 6c69 7374  nce(facets, list
+000332e0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+000332f0: 6163 6574 7320 3d20 7475 706c 6528 6661  acets = tuple(fa
+00033300: 6365 7473 290a 2020 2020 2020 2020 7365  cets).        se
+00033310: 6c65 6374 6564 5f66 6163 6574 7320 3d20  lected_facets = 
+00033320: 6172 6775 6d65 6e74 5f61 6e64 5f6c 6974  argument_and_lit
+00033330: 6572 616c 5f74 7970 6532 6c69 7374 2866  eral_type2list(f
+00033340: 6163 6574 732c 2066 6163 6574 5f74 7970  acets, facet_typ
+00033350: 655f 7661 722c 206e 6f6e 655f 6d65 616e  e_var, none_mean
+00033360: 735f 616c 6c3d 6e6f 6e65 5f6d 6561 6e73  s_all=none_means
+00033370: 5f61 6c6c 2c20 6c6f 6767 6572 3d6c 6f67  _all, logger=log
+00033380: 6765 7229 0a20 2020 2023 6c6f 6767 6572  ger).    #logger
+00033390: 2e64 6562 7567 2866 2252 6573 6f6c 7665  .debug(f"Resolve
+000333a0: 6420 6172 6775 6d65 6e74 2027 7b66 6163  d argument '{fac
+000333b0: 6574 737d 2720 746f 207b 7365 6c65 6374  ets}' to {select
+000333c0: 6564 5f66 6163 6574 737d 2e22 290a 2020  ed_facets}.").  
+000333d0: 2020 7265 7475 726e 2073 656c 6563 7465    return selecte
+000333e0: 645f 6661 6365 7473 0a0a 6465 6620 626f  d_facets..def bo
+000333f0: 6c64 5f66 6f6e 7428 7329 3a0a 2020 2020  ld_font(s):.    
+00033400: 7265 7475 726e 2066 225c 3033 335b 316d  return f"\033[1m
+00033410: 7b73 7d5c 3033 335b 303b 306d 220a 0a64  {s}\033[0;0m"..d
+00033420: 6566 2061 7661 696c 6162 6c65 5f76 6965  ef available_vie
+00033430: 7773 3273 7472 2876 6965 7773 5f64 6963  ws2str(views_dic
+00033440: 743a 2056 6965 7744 6963 742c 2061 6374  t: ViewDict, act
+00033450: 6976 655f 7669 6577 5f6e 616d 653a 2073  ive_view_name: s
+00033460: 7472 203d 204e 6f6e 6529 202d 3e20 7374  tr = None) -> st
+00033470: 723a 0a20 2020 2076 6965 775f 6e61 6d65  r:.    view_name
+00033480: 7320 3d20 7b6b 6579 3a20 7669 6577 2e6e  s = {key: view.n
+00033490: 616d 6520 6966 206b 6579 2069 7320 4e6f  ame if key is No
+000334a0: 6e65 2065 6c73 6520 6b65 7920 666f 7220  ne else key for 
+000334b0: 6b65 792c 2076 6965 7720 696e 2076 6965  key, view in vie
+000334c0: 7773 5f64 6963 742e 6974 656d 7328 297d  ws_dict.items()}
+000334d0: 0a20 2020 2063 7572 7265 6e74 5f76 6965  .    current_vie
+000334e0: 7720 3d20 7669 6577 5f6e 616d 6573 5b61  w = view_names[a
+000334f0: 6374 6976 655f 7669 6577 5f6e 616d 655d  ctive_view_name]
+00033500: 0a20 2020 2076 6965 775f 6c69 7374 203d  .    view_list =
+00033510: 205b 626f 6c64 5f66 6f6e 7428 6375 7272   [bold_font(curr
+00033520: 656e 745f 7669 6577 295d 202b 205b 6e61  ent_view)] + [na
+00033530: 6d65 2066 6f72 206e 616d 6520 696e 2076  me for name in v
+00033540: 6965 775f 6e61 6d65 732e 7661 6c75 6573  iew_names.values
+00033550: 2829 2069 6620 6e61 6d65 2021 3d20 6375  () if name != cu
+00033560: 7272 656e 745f 7669 6577 5d0a 2020 2020  rrent_view].    
+00033570: 7265 7475 726e 2066 225b 7b27 7c27 2e6a  return f"[{'|'.j
+00033580: 6f69 6e28 7669 6577 5f6c 6973 7429 7d5d  oin(view_list)}]
+00033590: 5c6e 220a 0a0a 4066 756e 6374 696f 6e5f  \n"...@function_
+000335a0: 6c6f 6767 6572 0a64 6566 2075 6e70 6163  logger.def unpac
+000335b0: 6b5f 6a73 6f6e 5f70 6174 6873 2870 6174  k_json_paths(pat
+000335c0: 6873 3a20 436f 6c6c 6563 7469 6f6e 5b73  hs: Collection[s
+000335d0: 7472 5d29 202d 3e20 4e6f 6e65 3a0a 2020  tr]) -> None:.  
+000335e0: 2020 2222 224d 7574 6174 6573 2074 6865    """Mutates the
+000335f0: 206c 6973 7420 7769 7468 2070 6174 6873   list with paths
+00033600: 2062 7920 7265 706c 6163 696e 6720 2e6a   by replacing .j
+00033610: 736f 6e20 6669 6c65 7320 7769 7468 2074  son files with t
+00033620: 6865 206c 6973 7420 286f 6620 7061 7468  he list (of path
+00033630: 7329 2063 6f6e 7461 696e 6564 2069 6e20  s) contained in 
+00033640: 7468 656d 2e22 2222 0a20 2020 206a 736f  them.""".    jso
+00033650: 6e5f 6978 7320 3d20 5b69 2066 6f72 2069  n_ixs = [i for i
+00033660: 2c20 7020 696e 2065 6e75 6d65 7261 7465  , p in enumerate
+00033670: 2870 6174 6873 2920 6966 2070 2e65 6e64  (paths) if p.end
+00033680: 7377 6974 6828 272e 6a73 6f6e 2729 5d0a  swith('.json')].
+00033690: 2020 2020 6966 206c 656e 286a 736f 6e5f      if len(json_
+000336a0: 6978 7329 203e 2030 3a0a 2020 2020 2020  ixs) > 0:.      
+000336b0: 2020 666f 7220 6920 696e 2072 6576 6572    for i in rever
+000336c0: 7365 6428 6a73 6f6e 5f69 7873 293a 0a20  sed(json_ixs):. 
+000336d0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000336e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000336f0: 7769 7468 206f 7065 6e28 7061 7468 735b  with open(paths[
+00033700: 695d 2920 6173 2066 3a0a 2020 2020 2020  i]) as f:.      
+00033710: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00033720: 6164 6564 5f70 6174 6873 203d 206a 736f  aded_paths = jso
+00033730: 6e2e 6c6f 6164 2866 290a 2020 2020 2020  n.load(f).      
+00033740: 2020 2020 2020 2020 2020 7061 7468 732e            paths.
+00033750: 6578 7465 6e64 286c 6f61 6465 645f 7061  extend(loaded_pa
+00033760: 7468 7329 0a20 2020 2020 2020 2020 2020  ths).           
+00033770: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+00033780: 2866 2255 6e70 6163 6b65 6420 7468 6520  (f"Unpacked the 
+00033790: 7b6c 656e 286c 6f61 6465 645f 7061 7468  {len(loaded_path
+000337a0: 7329 7d20 7061 7468 7320 666f 756e 6420  s)} paths found 
+000337b0: 696e 207b 7061 7468 735b 695d 7d2e 2229  in {paths[i]}.")
+000337c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000337d0: 2064 656c 2028 7061 7468 735b 695d 290a   del (paths[i]).
+000337e0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000337f0: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
+00033800: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00033810: 6767 6572 2e69 6e66 6f28 6622 436f 756c  gger.info(f"Coul
+00033820: 6420 6e6f 7420 6c6f 6164 2070 6174 6873  d not load paths
+00033830: 2066 726f 6d20 7b70 6174 6873 5b69 5d7d   from {paths[i]}
+00033840: 2062 6563 6175 7365 206f 6620 7468 6520   because of the 
+00033850: 666f 6c6c 6f77 696e 6720 6572 726f 7228  following error(
+00033860: 7329 3a5c 6e7b 7379 732e 6578 635f 696e  s):\n{sys.exc_in
+00033870: 666f 2829 5b31 5d7d 2229 0a0a 0a40 6675  fo()[1]}")...@fu
+00033880: 6e63 7469 6f6e 5f6c 6f67 6765 720a 6465  nction_logger.de
+00033890: 6620 7265 736f 6c76 655f 7061 7468 735f  f resolve_paths_
+000338a0: 6172 6775 6d65 6e74 2870 6174 6873 3a20  argument(paths: 
+000338b0: 556e 696f 6e5b 7374 722c 2043 6f6c 6c65  Union[str, Colle
+000338c0: 6374 696f 6e5b 7374 725d 5d2c 0a20 2020  ction[str]],.   
+000338d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000338e0: 2020 2020 2020 2020 6669 6c65 733a 2062          files: b
+000338f0: 6f6f 6c20 3d20 5472 7565 2920 2d3e 204c  ool = True) -> L
+00033900: 6973 745b 7374 725d 3a0a 2020 2020 2222  ist[str]:.    ""
+00033910: 2220 4d61 6b65 7320 7375 7265 2074 6861  " Makes sure tha
+00033920: 7420 7468 6520 6769 7665 6e20 7061 7468  t the given path
+00033930: 2873 2920 6578 6973 7473 2873 2920 616e  (s) exists(s) an
+00033940: 6420 6669 6c74 6572 7320 6f75 7420 7468  d filters out th
+00033950: 6f73 6520 7468 6174 2064 6f6e 2774 2e0a  ose that don't..
+00033960: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+00033970: 2070 6174 6873 3a20 4f6e 6520 6f72 2073   paths: One or s
+00033980: 6576 6572 616c 2070 6174 6873 2067 6976  everal paths giv
+00033990: 656e 2061 7320 7374 7269 6e67 732e 0a20  en as strings.. 
+000339a0: 2020 2020 2066 696c 6573 3a20 4279 2064       files: By d
+000339b0: 6566 6175 6c74 2c20 6f6e 6c79 2066 696c  efault, only fil
+000339c0: 6520 7061 7468 7320 6172 6520 7265 7475  e paths are retu
+000339d0: 726e 6564 2e20 5365 7420 746f 2046 616c  rned. Set to Fal
+000339e0: 7365 2074 6f20 7265 7475 726e 206f 6e6c  se to return onl
+000339f0: 7920 666f 6c64 6572 732e 0a0a 2020 2020  y folders...    
+00033a00: 5265 7475 726e 733a 0a0a 2020 2020 2222  Returns:..    ""
+00033a10: 220a 2020 2020 6966 2069 7369 6e73 7461  ".    if isinsta
+00033a20: 6e63 6528 7061 7468 732c 2073 7472 293a  nce(paths, str):
+00033a30: 0a20 2020 2020 2020 2070 6174 6873 203d  .        paths =
+00033a40: 205b 7061 7468 735d 0a20 2020 2072 6573   [paths].    res
+00033a50: 6f6c 7665 645f 7061 7468 7320 3d20 5b72  olved_paths = [r
+00033a60: 6573 6f6c 7665 5f64 6972 2870 2920 666f  esolve_dir(p) fo
+00033a70: 7220 7020 696e 2070 6174 6873 5d0a 2020  r p in paths].  
+00033a80: 2020 6966 2066 696c 6573 3a0a 2020 2020    if files:.    
+00033a90: 2020 2020 6e6f 745f 615f 6669 6c65 203d      not_a_file =
+00033aa0: 205b 7020 666f 7220 7020 696e 2072 6573   [p for p in res
+00033ab0: 6f6c 7665 645f 7061 7468 7320 6966 206e  olved_paths if n
+00033ac0: 6f74 206f 732e 7061 7468 2e69 7366 696c  ot os.path.isfil
+00033ad0: 6528 7029 5d0a 2020 2020 2020 2020 6966  e(p)].        if
+00033ae0: 206c 656e 286e 6f74 5f61 5f66 696c 6529   len(not_a_file)
+00033af0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00033b00: 2020 6966 206c 656e 286e 6f74 5f61 5f66    if len(not_a_f
+00033b10: 696c 6529 203d 3d20 313a 0a20 2020 2020  ile) == 1:.     
+00033b20: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+00033b30: 2066 224e 6f20 6578 6973 7469 6e67 2066   f"No existing f
+00033b40: 696c 6520 6174 207b 6e6f 745f 615f 6669  ile at {not_a_fi
+00033b50: 6c65 5b30 5d7d 2e22 0a20 2020 2020 2020  le[0]}.".       
+00033b60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00033b70: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+00033b80: 2066 2254 6865 7365 2061 7265 206e 6f74   f"These are not
+00033b90: 2070 6174 6873 206f 6620 6578 6973 7469   paths of existi
+00033ba0: 6e67 2066 696c 6573 3a20 7b6e 6f74 5f61  ng files: {not_a
+00033bb0: 5f66 696c 657d 220a 2020 2020 2020 2020  _file}".        
+00033bc0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+00033bd0: 6e67 286d 7367 290a 2020 2020 2020 2020  ng(msg).        
+00033be0: 2020 2020 7265 736f 6c76 6564 5f70 6174      resolved_pat
+00033bf0: 6873 203d 205b 7020 666f 7220 7020 696e  hs = [p for p in
+00033c00: 2072 6573 6f6c 7665 645f 7061 7468 7320   resolved_paths 
+00033c10: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
+00033c20: 6528 7029 5d0a 2020 2020 656c 7365 3a0a  e(p)].    else:.
+00033c30: 2020 2020 2020 2020 6e6f 745f 615f 666f          not_a_fo
+00033c40: 6c64 6572 203d 205b 7020 666f 7220 7020  lder = [p for p 
+00033c50: 696e 2072 6573 6f6c 7665 645f 7061 7468  in resolved_path
+00033c60: 7320 6966 206e 6f74 206f 732e 7061 7468  s if not os.path
+00033c70: 2e69 7364 6972 2870 295d 0a20 2020 2020  .isdir(p)].     
+00033c80: 2020 2069 6620 6c65 6e28 6e6f 745f 615f     if len(not_a_
+00033c90: 666f 6c64 6572 2920 3e20 303a 0a20 2020  folder) > 0:.   
+00033ca0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00033cb0: 6e6f 745f 615f 666f 6c64 6572 2920 3d3d  not_a_folder) ==
+00033cc0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00033cd0: 2020 2020 6d73 6720 3d20 6622 7b6e 6f74      msg = f"{not
+00033ce0: 5f61 5f66 6f6c 6465 725b 305d 7d20 6973  _a_folder[0]} is
+00033cf0: 206e 6f74 2061 2070 6174 6820 746f 2061   not a path to a
+00033d00: 6e20 6578 6973 7469 6e67 2066 6f6c 6465  n existing folde
+00033d10: 722e 220a 2020 2020 2020 2020 2020 2020  r.".            
+00033d20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00033d30: 2020 2020 2020 6d73 6720 3d20 6622 5468        msg = f"Th
+00033d40: 6573 6520 6172 6520 6e6f 7420 7061 7468  ese are not path
+00033d50: 7320 6f66 2065 7869 7374 696e 6720 666f  s of existing fo
+00033d60: 6c64 6572 733a 207b 6e6f 745f 615f 666f  lders: {not_a_fo
+00033d70: 6c64 6572 7d22 0a20 2020 2020 2020 2020  lder}".         
+00033d80: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+00033d90: 6728 6d73 6729 0a20 2020 2020 2020 2020  g(msg).         
+00033da0: 2020 2072 6573 6f6c 7665 645f 7061 7468     resolved_path
+00033db0: 7320 3d20 5b70 2066 6f72 2070 2069 6e20  s = [p for p in 
+00033dc0: 7265 736f 6c76 6564 5f70 6174 6873 2069  resolved_paths i
+00033dd0: 6620 6f73 2e70 6174 682e 6973 6469 7228  f os.path.isdir(
+00033de0: 7029 5d0a 2020 2020 7265 7475 726e 2072  p)].    return r
+00033df0: 6573 6f6c 7665 645f 7061 7468 730a 0a40  esolved_paths..@
+00033e00: 6675 6e63 7469 6f6e 5f6c 6f67 6765 720a  function_logger.
+00033e10: 6465 6620 636f 6d70 7574 655f 7061 7468  def compute_path
+00033e20: 5f66 726f 6d5f 6669 6c65 2866 696c 653a  _from_file(file:
+00033e30: 2046 696c 652c 0a20 2020 2020 2020 2020   File,.         
+00033e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033e50: 2020 726f 6f74 5f64 6972 3a20 4f70 7469    root_dir: Opti
+00033e60: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00033e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00033e80: 2020 2020 2020 2020 2020 2020 2066 6f6c               fol
+00033e90: 6465 723a 204f 7074 696f 6e61 6c5b 7374  der: Optional[st
+00033ea0: 725d 203d 204e 6f6e 6529 202d 3e20 7374  r] = None) -> st
+00033eb0: 723a 0a20 2020 2022 2222 0a20 2020 2043  r:.    """.    C
+00033ec0: 6f6e 7374 7275 6374 7320 6120 7061 7468  onstructs a path
+00033ed0: 2062 6173 6564 206f 6e20 7468 6520 6172   based on the ar
+00033ee0: 6775 6d65 6e74 732e 0a0a 2020 2020 4172  guments...    Ar
+00033ef0: 6773 3a0a 2020 2020 2020 6669 6c65 3a20  gs:.      file: 
+00033f00: 5468 6973 2066 756e 6374 696f 6e20 7573  This function us
+00033f10: 6573 2074 6865 2066 6965 6c64 7320 636f  es the fields co
+00033f20: 7270 7573 5f70 6174 682c 2073 7562 6469  rpus_path, subdi
+00033f30: 722c 2061 6e64 2074 7970 652e 0a20 2020  r, and type..   
+00033f40: 2020 2072 6f6f 745f 6469 723a 0a20 2020     root_dir:.   
+00033f50: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00033f60: 746f 204e 6f6e 652c 206d 6561 6e69 6e67  to None, meaning
+00033f70: 2074 6861 7420 7468 6520 7061 7468 2069   that the path i
+00033f80: 7320 636f 6e73 7472 7563 7465 6420 6261  s constructed ba
+00033f90: 7365 6420 6f6e 2074 6865 2063 6f72 7075  sed on the corpu
+00033fa0: 735f 7061 7468 2e0a 2020 2020 2020 2020  s_path..        
+00033fb0: 2020 5061 7373 2061 2064 6972 6563 746f    Pass a directo
+00033fc0: 7279 2074 6f20 636f 6e73 7472 7563 7420  ry to construct 
+00033fd0: 7468 6520 7061 7468 2072 656c 6174 6976  the path relativ
+00033fe0: 6520 746f 2069 7420 696e 7374 6561 642e  e to it instead.
+00033ff0: 2049 6620 6060 666f 6c64 6572 6060 2069   If ``folder`` i
+00034000: 7320 616e 2061 6273 6f6c 7574 6520 7061  s an absolute pa
+00034010: 7468 2c0a 2020 2020 2020 2020 2020 6060  th,.          ``
+00034020: 726f 6f74 5f64 6972 6060 2069 7320 6967  root_dir`` is ig
+00034030: 6e6f 7265 642e 0a20 2020 2020 2066 6f6c  nored..      fol
+00034040: 6465 723a 0a20 2020 2020 2020 2020 202a  der:.          *
+00034050: 2049 6620 6060 666f 6c64 6572 6060 2069   If ``folder`` i
+00034060: 7320 4e6f 6e65 2028 6465 6661 756c 7429  s None (default)
+00034070: 2c20 7468 6520 6669 6c65 7327 2074 7970  , the files' typ
+00034080: 6520 7769 6c6c 2062 6520 6170 7065 6e64  e will be append
+00034090: 6564 2074 6f20 7468 6520 6060 726f 6f74  ed to the ``root
+000340a0: 5f64 6972 6060 2e0a 2020 2020 2020 2020  _dir``..        
+000340b0: 2020 2a20 4966 2060 6066 6f6c 6465 7260    * If ``folder`
+000340c0: 6020 6973 2061 6e20 6162 736f 6c75 7465  ` is an absolute
+000340d0: 2070 6174 682c 2060 6072 6f6f 745f 6469   path, ``root_di
+000340e0: 7260 6020 7769 6c6c 2062 6520 6967 6e6f  r`` will be igno
+000340f0: 7265 642e 0a20 2020 2020 2020 2020 202a  red..          *
+00034100: 2049 6620 6060 666f 6c64 6572 6060 2069   If ``folder`` i
+00034110: 7320 6120 7265 6c61 7469 7665 2070 6174  s a relative pat
+00034120: 6820 7374 6172 7469 6e67 2077 6974 6820  h starting with 
+00034130: 6120 646f 7420 6060 2e60 6020 7468 6520  a dot ``.`` the 
+00034140: 7265 6c61 7469 7665 2070 6174 6820 6973  relative path is
+00034150: 2061 7070 656e 6465 6420 746f 2074 6865   appended to the
+00034160: 2066 696c 6527 7320 7375 6264 6972 2e0a   file's subdir..
+00034170: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+00034180: 6578 616d 706c 652c 2060 602e 2e5c 6e6f  example, ``..\no
+00034190: 7465 7360 6020 7769 6c6c 2072 6573 6f6c  tes`` will resol
+000341a0: 7665 2074 6f20 6120 7369 626c 696e 6720  ve to a sibling 
+000341b0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+000341c0: 206f 6e65 2077 6865 7265 2074 6865 2060   one where the `
+000341d0: 6066 696c 6560 6020 6973 206c 6f63 6174  `file`` is locat
+000341e0: 6564 2e0a 2020 2020 2020 2020 2020 2a20  ed..          * 
+000341f0: 4966 2060 6066 6f6c 6465 7260 6020 6973  If ``folder`` is
+00034200: 2061 2072 656c 6174 6976 6520 7061 7468   a relative path
+00034210: 2074 6861 7420 646f 6573 206e 6f74 2062   that does not b
+00034220: 6567 696e 2077 6974 6820 6120 646f 7420  egin with a dot 
+00034230: 6060 2e60 602c 2069 7420 7769 6c6c 2062  ``.``, it will b
+00034240: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
+00034250: 650a 2020 2020 2020 2020 2020 2020 6060  e.            ``
+00034260: 726f 6f74 5f64 6972 6060 2e0a 2020 2020  root_dir``..    
+00034270: 2020 2020 2020 2a20 4966 2060 6066 6f6c        * If ``fol
+00034280: 6465 7260 6020 3d3d 2027 2720 2865 6d70  der`` == '' (emp
+00034290: 7479 2073 7472 696e 6729 2c20 7468 6520  ty string), the 
+000342a0: 7265 7375 6c74 2077 696c 6c20 6265 2060  result will be `
+000342b0: 726f 6f74 5f64 6972 602e 0a0a 2020 2020  root_dir`...    
+000342c0: 5265 7475 726e 733a 0a20 2020 2020 2054  Returns:.      T
+000342d0: 6865 2063 6f6e 7374 7275 6374 6564 2064  he constructed d
+000342e0: 6972 6563 746f 7279 2070 6174 682e 0a20  irectory path.. 
+000342f0: 2020 2022 2222 0a20 2020 2069 6620 666f     """.    if fo
+00034300: 6c64 6572 2069 7320 6e6f 7420 4e6f 6e65  lder is not None
+00034310: 2061 6e64 2028 6f73 2e70 6174 682e 6973   and (os.path.is
+00034320: 6162 7328 666f 6c64 6572 2920 6f72 2027  abs(folder) or '
+00034330: 7e27 2069 6e20 666f 6c64 6572 293a 0a20  ~' in folder):. 
+00034340: 2020 2020 2020 2066 6f6c 6465 7220 3d20         folder = 
+00034350: 7265 736f 6c76 655f 6469 7228 666f 6c64  resolve_dir(fold
+00034360: 6572 290a 2020 2020 2020 2020 7061 7468  er).        path
+00034370: 203d 2066 6f6c 6465 720a 2020 2020 656c   = folder.    el
+00034380: 7365 3a0a 2020 2020 2020 2020 726f 6f74  se:.        root
+00034390: 203d 2066 696c 652e 636f 7270 7573 5f70   = file.corpus_p
+000343a0: 6174 6820 6966 2072 6f6f 745f 6469 7220  ath if root_dir 
+000343b0: 6973 204e 6f6e 6520 656c 7365 2072 6573  is None else res
+000343c0: 6f6c 7665 5f64 6972 2872 6f6f 745f 6469  olve_dir(root_di
+000343d0: 7229 0a20 2020 2020 2020 2069 6620 666f  r).        if fo
+000343e0: 6c64 6572 2069 7320 4e6f 6e65 3a0a 2020  lder is None:.  
+000343f0: 2020 2020 2020 2020 2020 7061 7468 203d            path =
+00034400: 206f 732e 7061 7468 2e6a 6f69 6e28 726f   os.path.join(ro
+00034410: 6f74 2c20 6669 6c65 2e74 7970 6529 0a20  ot, file.type). 
+00034420: 2020 2020 2020 2065 6c69 6620 666f 6c64         elif fold
+00034430: 6572 203d 3d20 2727 3a0a 2020 2020 2020  er == '':.      
+00034440: 2020 2020 2020 7061 7468 203d 2072 6f6f        path = roo
+00034450: 740a 2020 2020 2020 2020 656c 6966 2066  t.        elif f
+00034460: 6f6c 6465 725b 305d 203d 3d20 272e 273a  older[0] == '.':
+00034470: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+00034480: 6820 3d20 6f73 2e70 6174 682e 6162 7370  h = os.path.absp
+00034490: 6174 6828 6f73 2e70 6174 682e 6a6f 696e  ath(os.path.join
+000344a0: 2872 6f6f 742c 2066 696c 652e 7375 6264  (root, file.subd
+000344b0: 6972 2c20 666f 6c64 6572 2929 0a20 2020  ir, folder)).   
+000344c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000344d0: 2020 2020 2020 2070 6174 6820 3d20 6f73         path = os
+000344e0: 2e70 6174 682e 6162 7370 6174 6828 6f73  .path.abspath(os
+000344f0: 2e70 6174 682e 6a6f 696e 2872 6f6f 742c  .path.join(root,
+00034500: 2066 6f6c 6465 7229 290a 2020 2020 7265   folder)).    re
+00034510: 7475 726e 2070 6174 680a 0a64 6566 206d  turn path..def m
+00034520: 616b 655f 6669 6c65 5f70 6174 6828 6669  ake_file_path(fi
+00034530: 6c65 3a20 4669 6c65 2c0a 2020 2020 2020  le: File,.      
+00034540: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00034550: 745f 6469 723d 4e6f 6e65 2c0a 2020 2020  t_dir=None,.    
+00034560: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00034570: 6f6c 6465 723a 2073 7472 203d 204e 6f6e  older: str = Non
+00034580: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00034590: 2020 2020 2020 7375 6666 6978 3a20 7374        suffix: st
+000345a0: 7220 3d20 2727 2c0a 2020 2020 2020 2020  r = '',.        
+000345b0: 2020 2020 2020 2020 2020 2066 6578 743a             fext:
+000345c0: 2073 7472 203d 2027 2e74 7376 2729 3a0a   str = '.tsv'):.
+000345d0: 2020 2020 2222 2220 436f 6e73 7472 7563      """ Construc
+000345e0: 7473 2061 2066 696c 6520 7061 7468 2062  ts a file path b
+000345f0: 6173 6564 206f 6e20 7468 6520 6172 6775  ased on the argu
+00034600: 6d65 6e74 732e 0a0a 2020 2020 4172 6773  ments...    Args
+00034610: 3a0a 2020 2020 2020 6669 6c65 3a20 5468  :.      file: Th
+00034620: 6973 2066 756e 6374 696f 6e20 7573 6573  is function uses
+00034630: 2074 6865 2066 6965 6c64 7320 666e 616d   the fields fnam
+00034640: 652c 2063 6f72 7075 735f 7061 7468 2c20  e, corpus_path, 
+00034650: 7375 6264 6972 2c20 616e 6420 7479 7065  subdir, and type
+00034660: 2e0a 2020 2020 2020 726f 6f74 5f64 6972  ..      root_dir
+00034670: 3a0a 2020 2020 2020 2020 4465 6661 756c  :.        Defaul
+00034680: 7473 2074 6f20 4e6f 6e65 2c20 6d65 616e  ts to None, mean
+00034690: 696e 6720 7468 6174 2074 6865 2070 6174  ing that the pat
+000346a0: 6820 6973 2063 6f6e 7374 7275 6374 6564  h is constructed
+000346b0: 2062 6173 6564 206f 6e20 7468 6520 636f   based on the co
+000346c0: 7270 7573 5f70 6174 682e 0a20 2020 2020  rpus_path..     
+000346d0: 2020 2050 6173 7320 6120 6469 7265 6374     Pass a direct
+000346e0: 6f72 7920 746f 2063 6f6e 7374 7275 6374  ory to construct
+000346f0: 2074 6865 2070 6174 6820 7265 6c61 7469   the path relati
+00034700: 7665 2074 6f20 6974 2069 6e73 7465 6164  ve to it instead
+00034710: 2e20 4966 2060 6066 6f6c 6465 7260 6020  . If ``folder`` 
+00034720: 6973 2061 6e20 6162 736f 6c75 7465 2070  is an absolute p
+00034730: 6174 682c 0a20 2020 2020 2020 2060 6072  ath,.        ``r
+00034740: 6f6f 745f 6469 7260 6020 6973 2069 676e  oot_dir`` is ign
+00034750: 6f72 6564 2e0a 2020 2020 2020 666f 6c64  ored..      fold
+00034760: 6572 3a0a 2020 2020 2020 2020 4469 6666  er:.        Diff
+00034770: 6572 656e 7420 6265 6861 7669 6f75 7273  erent behaviours
+00034780: 2061 7265 2061 7661 696c 6162 6c65 2e20   are available. 
+00034790: 4e6f 7465 2074 6861 7420 6f6e 6c79 2074  Note that only t
+000347a0: 6865 2074 6869 7264 206f 7074 696f 6e20  he third option 
+000347b0: 656e 7375 7265 7320 7468 6174 2066 696c  ensures that fil
+000347c0: 6520 7061 7468 7320 6172 6520 6469 7374  e paths are dist
+000347d0: 696e 6374 2066 6f72 0a20 2020 2020 2020  inct for.       
+000347e0: 2066 696c 6573 2074 6861 7420 6861 7665   files that have
+000347f0: 2069 6465 6e74 6963 616c 2066 6e61 6d65   identical fname
+00034800: 7320 6275 7420 6172 6520 6c6f 6361 7465  s but are locate
+00034810: 6420 696e 2064 6966 6665 7265 6e74 2073  d in different s
+00034820: 7562 6469 7265 6374 6f72 6965 7320 6f66  ubdirectories of
+00034830: 2074 6865 2073 616d 6520 636f 7270 7573   the same corpus
+00034840: 2e0a 2020 2020 2020 2020 2a20 4966 2060  ..        * If `
+00034850: 6066 6f6c 6465 7260 6020 6973 204e 6f6e  `folder`` is Non
+00034860: 6520 2864 6566 6175 6c74 292c 2074 6865  e (default), the
+00034870: 2066 696c 6573 2720 7479 7065 2077 696c   files' type wil
+00034880: 6c20 6265 2061 7070 656e 6465 6420 746f  l be appended to
+00034890: 2074 6865 2060 6072 6f6f 745f 6469 7260   the ``root_dir`
+000348a0: 602e 0a20 2020 2020 2020 202a 2049 6620  `..        * If 
+000348b0: 6060 666f 6c64 6572 6060 2069 7320 616e  ``folder`` is an
+000348c0: 2061 6273 6f6c 7574 6520 7061 7468 2c20   absolute path, 
+000348d0: 6060 726f 6f74 5f64 6972 6060 2077 696c  ``root_dir`` wil
+000348e0: 6c20 6265 2069 676e 6f72 6564 2e0a 2020  l be ignored..  
+000348f0: 2020 2020 2020 2a20 4966 2060 6066 6f6c        * If ``fol
+00034900: 6465 7260 6020 6973 2061 2072 656c 6174  der`` is a relat
+00034910: 6976 6520 7061 7468 2073 7461 7274 696e  ive path startin
+00034920: 6720 7769 7468 2061 2064 6f74 2060 602e  g with a dot ``.
+00034930: 6060 2074 6865 2072 656c 6174 6976 6520  `` the relative 
+00034940: 7061 7468 2069 7320 6170 7065 6e64 6564  path is appended
+00034950: 2074 6f20 7468 6520 6669 6c65 2773 2073   to the file's s
+00034960: 7562 6469 722e 0a20 2020 2020 2020 2020  ubdir..         
+00034970: 2046 6f72 2065 7861 6d70 6c65 2c20 6060   For example, ``
+00034980: 2e2e 5c6e 6f74 6573 6060 2077 696c 6c20  ..\notes`` will 
+00034990: 7265 736f 6c76 6520 746f 2061 2073 6962  resolve to a sib
+000349a0: 6c69 6e67 2064 6972 6563 746f 7279 206f  ling directory o
+000349b0: 6620 7468 6520 6f6e 6520 7768 6572 6520  f the one where 
+000349c0: 7468 6520 6060 6669 6c65 6060 2069 7320  the ``file`` is 
+000349d0: 6c6f 6361 7465 642e 0a20 2020 2020 2020  located..       
+000349e0: 202a 2049 6620 6060 666f 6c64 6572 6060   * If ``folder``
+000349f0: 2069 7320 6120 7265 6c61 7469 7665 2070   is a relative p
+00034a00: 6174 6820 7468 6174 2064 6f65 7320 6e6f  ath that does no
+00034a10: 7420 6265 6769 6e20 7769 7468 2061 2064  t begin with a d
+00034a20: 6f74 2060 602e 6060 2c20 6974 2077 696c  ot ``.``, it wil
+00034a30: 6c20 6265 2061 7070 656e 6465 6420 746f  l be appended to
+00034a40: 2074 6865 0a20 2020 2020 2020 2020 2060   the.          `
+00034a50: 6072 6f6f 745f 6469 7260 602e 0a20 2020  `root_dir``..   
+00034a60: 2020 2073 7566 6669 783a 2053 7472 696e     suffix: Strin
+00034a70: 6720 746f 2061 7070 656e 6420 746f 2074  g to append to t
+00034a80: 6865 2066 696c 6527 7320 666e 616d 652e  he file's fname.
+00034a90: 0a20 2020 2020 2066 6578 743a 2046 696c  .      fext: Fil
+00034aa0: 6520 6578 7465 6e73 696f 6e20 746f 2061  e extension to a
+00034ab0: 7070 656e 6420 746f 2074 6865 2028 666e  ppend to the (fn
+00034ac0: 616d 652b 7375 6666 6978 292e 2044 6566  ame+suffix). Def
+00034ad0: 6175 6c74 7320 746f 2060 602e 7473 7660  aults to ``.tsv`
+00034ae0: 602e 0a0a 2020 2020 5265 7475 726e 733a  `...    Returns:
+00034af0: 0a20 2020 2020 2054 6865 2063 6f6e 7374  .      The const
+00034b00: 7275 6374 6564 2066 696c 6520 7061 7468  ructed file path
+00034b10: 2e0a 2020 2020 2222 220a 2020 2020 6173  ..    """.    as
+00034b20: 7365 7274 2066 6578 7420 6973 206e 6f74  sert fext is not
+00034b30: 204e 6f6e 652c 2022 220a 2020 2020 7061   None, "".    pa
+00034b40: 7468 203d 2063 6f6d 7075 7465 5f70 6174  th = compute_pat
+00034b50: 685f 6672 6f6d 5f66 696c 6528 6669 6c65  h_from_file(file
+00034b60: 2c20 726f 6f74 5f64 6972 3d72 6f6f 745f  , root_dir=root_
+00034b70: 6469 722c 2066 6f6c 6465 723d 666f 6c64  dir, folder=fold
+00034b80: 6572 290a 2020 2020 6966 2073 7566 6669  er).    if suffi
+00034b90: 7820 6973 204e 6f6e 653a 0a20 2020 2020  x is None:.     
+00034ba0: 2020 2073 7566 6669 7820 3d20 2727 0a20     suffix = ''. 
+00034bb0: 2020 2066 6e61 6d65 203d 2066 696c 652e     fname = file.
+00034bc0: 666e 616d 6520 2b20 7375 6666 6978 202b  fname + suffix +
+00034bd0: 2066 6578 740a 2020 2020 7265 7475 726e   fext.    return
+00034be0: 206f 732e 7061 7468 2e6a 6f69 6e28 7061   os.path.join(pa
+00034bf0: 7468 2c20 666e 616d 6529 0a0a 6465 6620  th, fname)..def 
+00034c00: 7374 7269 6e67 3269 6465 6e74 6966 6965  string2identifie
+00034c10: 7228 733a 2073 7472 2c20 7265 6d6f 7665  r(s: str, remove
+00034c20: 5f6c 6561 6469 6e67 5f75 6e64 6572 7363  _leading_undersc
+00034c30: 6f72 653a 2062 6f6f 6c20 3d20 5472 7565  ore: bool = True
+00034c40: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
+00034c50: 2254 7261 6e73 666f 726d 2061 2073 7472  "Transform a str
+00034c60: 696e 6720 696e 2061 2077 6179 2074 6861  ing in a way tha
+00034c70: 7420 6974 2063 616e 2062 6520 7573 6564  t it can be used
+00034c80: 2061 7320 6964 656e 7469 6669 6572 2028   as identifier (
+00034c90: 7661 7269 6162 6c65 206f 7220 6174 7472  variable or attr
+00034ca0: 6962 7574 6520 6e61 6d65 292e 0a20 2020  ibute name)..   
+00034cb0: 2053 6f6c 7574 696f 6e20 6279 204b 656e   Solution by Ken
+00034cc0: 616e 2042 616e 6b73 206f 6e20 6874 7470  an Banks on http
+00034cd0: 733a 2f2f 7374 6163 6b6f 7665 7266 6c6f  s://stackoverflo
+00034ce0: 772e 636f 6d2f 612f 3333 3033 3336 310a  w.com/a/3303361.
+00034cf0: 2020 2020 2222 220a 2020 2020 2320 5265      """.    # Re
+00034d00: 6d6f 7665 2069 6e76 616c 6964 2063 6861  move invalid cha
+00034d10: 7261 6374 6572 730a 2020 2020 7320 3d20  racters.    s = 
+00034d20: 7265 2e73 7562 2827 5b5e 302d 3961 2d7a  re.sub('[^0-9a-z
+00034d30: 412d 5a5f 5d27 2c20 2727 2c20 7329 0a0a  A-Z_]', '', s)..
+00034d40: 2020 2020 2320 5265 6d6f 7665 206c 6561      # Remove lea
+00034d50: 6469 6e67 2063 6861 7261 6374 6572 7320  ding characters 
+00034d60: 756e 7469 6c20 7765 2066 696e 6420 6120  until we find a 
+00034d70: 6c65 7474 6572 206f 7220 756e 6465 7273  letter or unders
+00034d80: 636f 7265 0a20 2020 2072 6567 6578 203d  core.    regex =
+00034d90: 2027 5e5b 5e61 2d7a 412d 5a5d 2b27 2069   '^[^a-zA-Z]+' i
+00034da0: 6620 7265 6d6f 7665 5f6c 6561 6469 6e67  f remove_leading
+00034db0: 5f75 6e64 6572 7363 6f72 6520 656c 7365  _underscore else
+00034dc0: 2027 5e5b 5e61 2d7a 412d 5a5f 5d2b 270a   '^[^a-zA-Z_]+'.
+00034dd0: 2020 2020 7320 3d20 7265 2e73 7562 2872      s = re.sub(r
+00034de0: 6567 6578 2c20 2727 2c20 7329 0a0a 2020  egex, '', s)..  
+00034df0: 2020 7265 7475 726e 2073 0a0a 406c 7275    return s..@lru
+00034e00: 5f63 6163 6865 2829 0a40 6675 6e63 7469  _cache().@functi
+00034e10: 6f6e 5f6c 6f67 6765 720a 6465 6620 6765  on_logger.def ge
+00034e20: 745f 6769 745f 636f 6d6d 6974 2872 6570  t_git_commit(rep
+00034e30: 6f5f 7061 7468 3a20 7374 722c 2067 6974  o_path: str, git
+00034e40: 5f72 6576 6973 696f 6e3a 2073 7472 2920  _revision: str) 
+00034e50: 2d3e 204f 7074 696f 6e61 6c5b 6769 742e  -> Optional[git.
+00034e60: 436f 6d6d 6974 5d3a 0a20 2020 2074 7279  Commit]:.    try
+00034e70: 3a0a 2020 2020 2020 2020 7265 706f 203d  :.        repo =
+00034e80: 2067 6974 2e52 6570 6f28 7265 706f 5f70   git.Repo(repo_p
+00034e90: 6174 682c 2073 6561 7263 685f 7061 7265  ath, search_pare
+00034ea0: 6e74 5f64 6972 6563 746f 7269 6573 3d54  nt_directories=T
+00034eb0: 7275 6529 0a20 2020 2065 7863 6570 7420  rue).    except 
+00034ec0: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
+00034ed0: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+00034ee0: 7272 6f72 2866 227b 7265 706f 5f70 6174  rror(f"{repo_pat
+00034ef0: 687d 2069 7320 6e6f 7420 616e 2065 7869  h} is not an exi
+00034f00: 7374 696e 6720 6769 7420 7265 706f 7369  sting git reposi
+00034f10: 746f 7279 3a20 7b65 7d22 290a 2020 2020  tory: {e}").    
+00034f20: 2020 2020 7265 7475 726e 0a20 2020 2074      return.    t
+00034f30: 7279 3a0a 2020 2020 2020 2020 7265 7475  ry:.        retu
+00034f40: 726e 2072 6570 6f2e 636f 6d6d 6974 2867  rn repo.commit(g
+00034f50: 6974 5f72 6576 6973 696f 6e29 0a20 2020  it_revision).   
+00034f60: 2065 7863 6570 7420 4261 644e 616d 653a   except BadName:
+00034f70: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00034f80: 6572 726f 7228 6622 7b67 6974 5f72 6576  error(f"{git_rev
+00034f90: 6973 696f 6e7d 2064 6f65 7320 6e6f 7420  ision} does not 
+00034fa0: 7265 736f 6c76 6520 746f 2061 2063 6f6d  resolve to a com
+00034fb0: 6d69 7420 666f 7220 7265 706f 207b 6f73  mit for repo {os
+00034fc0: 2e70 6174 682e 6261 7365 6e61 6d65 2872  .path.basename(r
+00034fd0: 6570 6f5f 7061 7468 297d 2e22 290a 0a0a  epo_path)}.")...
+00034fe0: 4066 756e 6374 696f 6e5f 6c6f 6767 6572  @function_logger
+00034ff0: 0a64 6566 2070 6172 7365 5f74 7376 5f66  .def parse_tsv_f
+00035000: 696c 655f 6174 5f67 6974 5f72 6576 6973  ile_at_git_revis
+00035010: 696f 6e28 6669 6c65 3a20 4669 6c65 2c0a  ion(file: File,.
 00035020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035030: 7265 706f 5f70 6174 683a 204f 7074 696f  repo_path: Optio
-00035040: 6e61 6c5b 7374 725d 203d 204e 6f6e 6529  nal[str] = None)
-00035050: 202d 3e20 4669 6c65 4461 7461 6672 616d   -> FileDatafram
-00035060: 6554 7570 6c65 4d61 7962 653a 0a20 2020  eTupleMaybe:.   
-00035070: 2022 2222 0a20 2020 2050 6173 7320 6120   """.    Pass a 
-00035080: 4669 6c65 206f 626a 6563 7420 6f66 2061  File object of a
-00035090: 2054 5356 2066 696c 6520 616e 6420 616e   TSV file and an
-000350a0: 2069 6465 6e74 6966 6965 7220 666f 7220   identifier for 
-000350b0: 6120 6769 7420 7265 7669 7369 6f6e 2074  a git revision t
-000350c0: 6f20 7265 7472 6965 7665 2074 6865 2070  o retrieve the p
-000350d0: 6172 7365 6420 5453 5620 6669 6c65 2061  arsed TSV file a
-000350e0: 7420 7468 6174 2063 6f6d 6d69 742e 0a20  t that commit.. 
-000350f0: 2020 2054 6865 2066 696c 6520 6e65 6564     The file need
-00035100: 7320 746f 2068 6176 6520 6578 6973 7465  s to have existe
-00035110: 6420 6174 2074 6865 2072 6576 6973 696f  d at the revisio
-00035120: 6e20 696e 2071 7565 7374 696f 6e2e 0a0a  n in question...
-00035130: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00035140: 6669 6c65 3a0a 2020 2020 2020 6769 745f  file:.      git_
-00035150: 7265 7669 7369 6f6e 3a0a 2020 2020 2020  revision:.      
-00035160: 7265 706f 5f70 6174 683a 0a0a 2020 2020  repo_path:..    
-00035170: 5265 7475 726e 733a 0a0a 2020 2020 2222  Returns:..    ""
-00035180: 220a 2020 2020 6966 2066 696c 652e 7479  ".    if file.ty
-00035190: 7065 203d 3d20 2773 636f 7265 7327 3a0a  pe == 'scores':.
-000351a0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-000351b0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-000351c0: 7228 6622 5061 7273 696e 6720 6f6c 6465  r(f"Parsing olde
-000351d0: 7220 7265 7669 7369 6f6e 7320 6f66 2073  r revisions of s
-000351e0: 636f 7265 7320 6973 206e 6f74 2069 6d70  cores is not imp
-000351f0: 6c65 6d65 6e74 6564 2e20 4368 6563 6b6f  lemented. Checko
-00035200: 7574 2074 6865 2072 6576 6973 696f 6e20  ut the revision 
-00035210: 796f 7572 7365 6c66 2e22 290a 2020 2020  yourself.").    
-00035220: 6966 2072 6570 6f5f 7061 7468 2069 7320  if repo_path is 
-00035230: 4e6f 6e65 3a0a 2020 2020 2020 2020 7265  None:.        re
-00035240: 706f 5f70 6174 6820 3d20 6669 6c65 2e63  po_path = file.c
-00035250: 6f72 7075 735f 7061 7468 0a20 2020 2063  orpus_path.    c
-00035260: 6f6d 6d69 7420 3d20 6765 745f 6769 745f  ommit = get_git_
-00035270: 636f 6d6d 6974 2872 6570 6f5f 7061 7468  commit(repo_path
-00035280: 2c20 6769 745f 7265 7669 7369 6f6e 2c20  , git_revision, 
-00035290: 6c6f 6767 6572 3d6c 6f67 6765 7229 0a20  logger=logger). 
-000352a0: 2020 2069 6620 636f 6d6d 6974 2069 7320     if commit is 
-000352b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7265  None:.        re
-000352c0: 7475 726e 204e 6f6e 652c 204e 6f6e 650a  turn None, None.
-000352d0: 2020 2020 636f 6d6d 6974 5f73 6861 203d      commit_sha =
-000352e0: 2063 6f6d 6d69 742e 6865 7873 6861 0a20   commit.hexsha. 
-000352f0: 2020 2073 686f 7274 5f73 6861 203d 2063     short_sha = c
-00035300: 6f6d 6d69 745f 7368 615b 3a37 5d0a 2020  ommit_sha[:7].  
-00035310: 2020 636f 6d6d 6974 5f69 6e66 6f20 3d20    commit_info = 
-00035320: 6622 7b73 686f 7274 5f73 6861 7d20 7769  f"{short_sha} wi
-00035330: 7468 206d 6573 7361 6765 2027 7b63 6f6d  th message '{com
-00035340: 6d69 742e 6d65 7373 6167 652e 7374 7269  mit.message.stri
-00035350: 7028 297d 2722 0a20 2020 2069 6620 7368  p()}'".    if sh
-00035360: 6f72 745f 7368 6120 213d 2067 6974 5f72  ort_sha != git_r
-00035370: 6576 6973 696f 6e3a 0a20 2020 2020 2020  evision:.       
-00035380: 206c 6f67 6765 722e 6465 6275 6728 6622   logger.debug(f"
-00035390: 5265 736f 6c76 6564 2027 7b67 6974 5f72  Resolved '{git_r
-000353a0: 6576 6973 696f 6e7d 2720 746f 2027 7b73  evision}' to '{s
-000353b0: 686f 7274 5f73 6861 7d27 2e22 290a 2020  hort_sha}'.").  
-000353c0: 2020 7265 6c5f 7061 7468 203d 206f 732e    rel_path = os.
-000353d0: 7061 7468 2e6e 6f72 6d70 6174 6828 6669  path.normpath(fi
-000353e0: 6c65 2e72 656c 5f70 6174 6829 0a20 2020  le.rel_path).   
-000353f0: 2074 7279 3a0a 2020 2020 2020 2020 7461   try:.        ta
-00035400: 7267 6574 6669 6c65 203d 2063 6f6d 6d69  rgetfile = commi
-00035410: 742e 7472 6565 202f 2072 656c 5f70 6174  t.tree / rel_pat
-00035420: 680a 2020 2020 6578 6365 7074 204b 6579  h.    except Key
-00035430: 4572 726f 723a 0a20 2020 2020 2020 2023  Error:.        #
-00035440: 2061 6464 206c 6f67 6963 2068 6572 6520   add logic here 
-00035450: 746f 2066 696e 6420 6f6c 6465 7220 7061  to find older pa
-00035460: 7468 2077 6865 6e20 7468 6520 6669 6c65  th when the file
-00035470: 2068 6173 2062 6565 6e20 6d6f 7665 6420   has been moved 
-00035480: 6f72 2072 656e 616d 6564 0a20 2020 2020  or renamed.     
-00035490: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
-000354a0: 6622 7b72 656c 5f70 6174 687d 2064 6964  f"{rel_path} did
-000354b0: 206e 6f74 2065 7869 7374 2061 7420 636f   not exist at co
-000354c0: 6d6d 6974 207b 636f 6d6d 6974 5f69 6e66  mmit {commit_inf
-000354d0: 6f7d 2e22 290a 2020 2020 2020 2020 7265  o}.").        re
-000354e0: 7475 726e 204e 6f6e 652c 204e 6f6e 650a  turn None, None.
-000354f0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00035500: 2077 6974 6820 696f 2e42 7974 6573 494f   with io.BytesIO
-00035510: 2874 6172 6765 7466 696c 652e 6461 7461  (targetfile.data
-00035520: 5f73 7472 6561 6d2e 7265 6164 2829 2920  _stream.read()) 
-00035530: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
-00035540: 2020 7061 7273 6564 203d 206c 6f61 645f    parsed = load_
-00035550: 7473 7628 6629 0a20 2020 2065 7863 6570  tsv(f).    excep
-00035560: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00035570: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
-00035580: 2e65 7272 6f72 2866 2250 6172 7369 6e67  .error(f"Parsing
-00035590: 207b 7265 6c5f 7061 7468 7d20 4020 636f   {rel_path} @ co
-000355a0: 6d6d 6974 207b 636f 6d6d 6974 5f69 6e66  mmit {commit_inf
-000355b0: 6f7d 2066 6169 6c65 6420 7769 7468 2074  o} failed with t
-000355c0: 6865 2066 6f6c 6c6f 7769 6e67 2065 7863  he following exc
-000355d0: 6570 7469 6f6e 3a5c 6e7b 657d 2229 0a20  eption:\n{e}"). 
-000355e0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000355f0: 6e65 2c20 4e6f 6e65 0a20 2020 206e 6577  ne, None.    new
-00035600: 5f66 696c 6520 3d20 7265 706c 6163 6528  _file = replace(
-00035610: 6669 6c65 2c20 636f 6d6d 6974 5f73 6861  file, commit_sha
-00035620: 3d63 6f6d 6d69 745f 7368 6129 0a20 2020  =commit_sha).   
-00035630: 2072 6574 7572 6e20 6e65 775f 6669 6c65   return new_file
-00035640: 2c20 7061 7273 6564 0a0a 0a40 6675 6e63  , parsed...@func
-00035650: 7469 6f6e 5f6c 6f67 6765 720a 6465 6620  tion_logger.def 
-00035660: 6368 6563 6b5f 7068 7261 7365 5f61 6e6e  check_phrase_ann
-00035670: 6f74 6174 696f 6e73 2864 663a 2070 642e  otations(df: pd.
-00035680: 4461 7461 4672 616d 652c 0a20 2020 2020  DataFrame,.     
-00035690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000356a0: 2020 2020 2020 2020 636f 6c75 6d6e 3a20          column: 
-000356b0: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
-000356c0: 2020 2222 2222 2222 0a20 2020 2070 5f63    """""".    p_c
-000356d0: 6f6c 203d 2064 665b 636f 6c75 6d6e 5d0a  ol = df[column].
-000356e0: 2020 2020 6f70 656e 696e 6720 3d20 705f      opening = p_
-000356f0: 636f 6c2e 6669 6c6c 6e61 2827 2729 2e73  col.fillna('').s
-00035700: 7472 2e63 6f75 6e74 2827 7b27 290a 2020  tr.count('{').  
-00035710: 2020 636c 6f73 696e 6720 3d20 705f 636f    closing = p_co
-00035720: 6c2e 6669 6c6c 6e61 2827 2729 2e73 7472  l.fillna('').str
-00035730: 2e63 6f75 6e74 2827 7d27 290a 2020 2020  .count('}').    
-00035740: 6966 2027 6d6e 5f70 6c61 7974 6872 6f75  if 'mn_playthrou
-00035750: 6768 2720 696e 2064 662e 636f 6c75 6d6e  gh' in df.column
-00035760: 733a 0a20 2020 2020 2020 2070 6f73 6974  s:.        posit
-00035770: 696f 6e5f 636f 6c20 3d20 276d 6e5f 706c  ion_col = 'mn_pl
-00035780: 6179 7468 726f 7567 6827 0a20 2020 2065  aythrough'.    e
-00035790: 6c73 653a 0a20 2020 2020 2020 206c 6f67  lse:.        log
-000357a0: 6765 722e 696e 666f 2866 2243 6f6c 756d  ger.info(f"Colum
-000357b0: 6e20 276d 6e5f 706c 6179 7468 726f 7567  n 'mn_playthroug
-000357c0: 6827 2069 7320 6d69 7373 696e 672c 2073  h' is missing, s
-000357d0: 6f20 6d79 2061 7373 6573 736d 656e 7420  o my assessment 
-000357e0: 6f66 2074 6865 2070 6872 6173 6520 616e  of the phrase an
-000357f0: 6e6f 7461 7469 6f6e 7320 6d69 6768 7420  notations might 
-00035800: 6265 2077 726f 6e67 2e22 290a 2020 2020  be wrong.").    
-00035810: 2020 2020 706f 7369 7469 6f6e 5f63 6f6c      position_col
-00035820: 203d 2027 6d6e 270a 2020 2020 636f 6c75   = 'mn'.    colu
-00035830: 6d6e 7320 3d20 5b70 6f73 6974 696f 6e5f  mns = [position_
-00035840: 636f 6c2c 2063 6f6c 756d 6e5d 0a20 2020  col, column].   
-00035850: 2069 6620 6f70 656e 696e 672e 7375 6d28   if opening.sum(
-00035860: 2920 213d 2063 6c6f 7369 6e67 2e73 756d  ) != closing.sum
-00035870: 2829 3a0a 2020 2020 2020 2020 6f20 3d20  ():.        o = 
-00035880: 6466 2e6c 6f63 5b28 6f70 656e 696e 6720  df.loc[(opening 
-00035890: 3e20 3029 2c20 636f 6c75 6d6e 735d 0a20  > 0), columns]. 
-000358a0: 2020 2020 2020 2063 203d 2064 662e 6c6f         c = df.lo
-000358b0: 635b 2863 6c6f 7369 6e67 203e 2030 292c  c[(closing > 0),
-000358c0: 2063 6f6c 756d 6e73 5d0a 2020 2020 2020   columns].      
-000358d0: 2020 636f 6d70 6172 6520 3d20 7064 2e63    compare = pd.c
-000358e0: 6f6e 6361 7428 5b6f 2e72 6573 6574 5f69  oncat([o.reset_i
-000358f0: 6e64 6578 2864 726f 703d 5472 7565 292c  ndex(drop=True),
-00035900: 2063 2e72 6573 6574 5f69 6e64 6578 2864   c.reset_index(d
-00035910: 726f 703d 5472 7565 295d 2c20 6178 6973  rop=True)], axis
-00035920: 3d31 290a 2020 2020 2020 2020 6966 2027  =1).        if '
-00035930: 6d6e 2720 696e 2063 6f6d 7061 7265 3a0a  mn' in compare:.
-00035940: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-00035950: 6172 6520 3d20 636f 6d70 6172 652e 6173  are = compare.as
-00035960: 7479 7065 287b 276d 6e27 3a20 2749 6e74  type({'mn': 'Int
-00035970: 3634 277d 290a 2020 2020 2020 2020 6c6f  64'}).        lo
-00035980: 6767 6572 2e77 6172 6e69 6e67 2866 2250  gger.warning(f"P
-00035990: 6872 6173 6520 6265 6769 6e6e 696e 6720  hrase beginning 
-000359a0: 616e 6420 656e 6469 6e67 7320 646f 6e27  and endings don'
-000359b0: 7420 6d61 7463 683a 5c6e 7b63 6f6d 7061  t match:\n{compa
-000359c0: 7265 2e74 6f5f 7374 7269 6e67 2869 6e64  re.to_string(ind
-000359d0: 6578 3d46 616c 7365 297d 222c 2065 7874  ex=False)}", ext
-000359e0: 7261 3d7b 226d 6573 7361 6765 5f69 6422  ra={"message_id"
-000359f0: 3a20 2831 362c 297d 290a 2020 2020 2020  : (16,)}).      
-00035a00: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-00035a10: 2020 2072 6574 7572 6e20 5472 7565 0a       return True.
+00035030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035040: 2020 2067 6974 5f72 6576 6973 696f 6e3a     git_revision:
+00035050: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+00035060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035070: 2020 2020 2020 2020 2072 6570 6f5f 7061           repo_pa
+00035080: 7468 3a20 4f70 7469 6f6e 616c 5b73 7472  th: Optional[str
+00035090: 5d20 3d20 4e6f 6e65 2920 2d3e 2046 696c  ] = None) -> Fil
+000350a0: 6544 6174 6166 7261 6d65 5475 706c 654d  eDataframeTupleM
+000350b0: 6179 6265 3a0a 2020 2020 2222 220a 2020  aybe:.    """.  
+000350c0: 2020 5061 7373 2061 2046 696c 6520 6f62    Pass a File ob
+000350d0: 6a65 6374 206f 6620 6120 5453 5620 6669  ject of a TSV fi
+000350e0: 6c65 2061 6e64 2061 6e20 6964 656e 7469  le and an identi
+000350f0: 6669 6572 2066 6f72 2061 2067 6974 2072  fier for a git r
+00035100: 6576 6973 696f 6e20 746f 2072 6574 7269  evision to retri
+00035110: 6576 6520 7468 6520 7061 7273 6564 2054  eve the parsed T
+00035120: 5356 2066 696c 6520 6174 2074 6861 7420  SV file at that 
+00035130: 636f 6d6d 6974 2e0a 2020 2020 5468 6520  commit..    The 
+00035140: 6669 6c65 206e 6565 6473 2074 6f20 6861  file needs to ha
+00035150: 7665 2065 7869 7374 6564 2061 7420 7468  ve existed at th
+00035160: 6520 7265 7669 7369 6f6e 2069 6e20 7175  e revision in qu
+00035170: 6573 7469 6f6e 2e0a 0a20 2020 2041 7267  estion...    Arg
+00035180: 733a 0a20 2020 2020 2066 696c 653a 0a20  s:.      file:. 
+00035190: 2020 2020 2067 6974 5f72 6576 6973 696f       git_revisio
+000351a0: 6e3a 0a20 2020 2020 2072 6570 6f5f 7061  n:.      repo_pa
+000351b0: 7468 3a0a 0a20 2020 2052 6574 7572 6e73  th:..    Returns
+000351c0: 3a0a 0a20 2020 2022 2222 0a20 2020 2069  :..    """.    i
+000351d0: 6620 6669 6c65 2e74 7970 6520 3d3d 2027  f file.type == '
+000351e0: 7363 6f72 6573 273a 0a20 2020 2020 2020  scores':.       
+000351f0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+00035200: 656e 7465 6445 7272 6f72 2866 2250 6172  entedError(f"Par
+00035210: 7369 6e67 206f 6c64 6572 2072 6576 6973  sing older revis
+00035220: 696f 6e73 206f 6620 7363 6f72 6573 2069  ions of scores i
+00035230: 7320 6e6f 7420 696d 706c 656d 656e 7465  s not implemente
+00035240: 642e 2043 6865 636b 6f75 7420 7468 6520  d. Checkout the 
+00035250: 7265 7669 7369 6f6e 2079 6f75 7273 656c  revision yoursel
+00035260: 662e 2229 0a20 2020 2069 6620 7265 706f  f.").    if repo
+00035270: 5f70 6174 6820 6973 204e 6f6e 653a 0a20  _path is None:. 
+00035280: 2020 2020 2020 2072 6570 6f5f 7061 7468         repo_path
+00035290: 203d 2066 696c 652e 636f 7270 7573 5f70   = file.corpus_p
+000352a0: 6174 680a 2020 2020 636f 6d6d 6974 203d  ath.    commit =
+000352b0: 2067 6574 5f67 6974 5f63 6f6d 6d69 7428   get_git_commit(
+000352c0: 7265 706f 5f70 6174 682c 2067 6974 5f72  repo_path, git_r
+000352d0: 6576 6973 696f 6e2c 206c 6f67 6765 723d  evision, logger=
+000352e0: 6c6f 6767 6572 290a 2020 2020 6966 2063  logger).    if c
+000352f0: 6f6d 6d69 7420 6973 204e 6f6e 653a 0a20  ommit is None:. 
+00035300: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00035310: 6e65 2c20 4e6f 6e65 0a20 2020 2063 6f6d  ne, None.    com
+00035320: 6d69 745f 7368 6120 3d20 636f 6d6d 6974  mit_sha = commit
+00035330: 2e68 6578 7368 610a 2020 2020 7368 6f72  .hexsha.    shor
+00035340: 745f 7368 6120 3d20 636f 6d6d 6974 5f73  t_sha = commit_s
+00035350: 6861 5b3a 375d 0a20 2020 2063 6f6d 6d69  ha[:7].    commi
+00035360: 745f 696e 666f 203d 2066 227b 7368 6f72  t_info = f"{shor
+00035370: 745f 7368 617d 2077 6974 6820 6d65 7373  t_sha} with mess
+00035380: 6167 6520 277b 636f 6d6d 6974 2e6d 6573  age '{commit.mes
+00035390: 7361 6765 2e73 7472 6970 2829 7d27 220a  sage.strip()}'".
+000353a0: 2020 2020 6966 2073 686f 7274 5f73 6861      if short_sha
+000353b0: 2021 3d20 6769 745f 7265 7669 7369 6f6e   != git_revision
+000353c0: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
+000353d0: 2e64 6562 7567 2866 2252 6573 6f6c 7665  .debug(f"Resolve
+000353e0: 6420 277b 6769 745f 7265 7669 7369 6f6e  d '{git_revision
+000353f0: 7d27 2074 6f20 277b 7368 6f72 745f 7368  }' to '{short_sh
+00035400: 617d 272e 2229 0a20 2020 2072 656c 5f70  a}'.").    rel_p
+00035410: 6174 6820 3d20 6f73 2e70 6174 682e 6e6f  ath = os.path.no
+00035420: 726d 7061 7468 2866 696c 652e 7265 6c5f  rmpath(file.rel_
+00035430: 7061 7468 292e 7265 706c 6163 6528 225c  path).replace("\
+00035440: 5c22 2c20 222f 2229 0a20 2020 2074 7279  \", "/").    try
+00035450: 3a0a 2020 2020 2020 2020 7461 7267 6574  :.        target
+00035460: 6669 6c65 203d 2063 6f6d 6d69 742e 7472  file = commit.tr
+00035470: 6565 202f 2072 656c 5f70 6174 680a 2020  ee / rel_path.  
+00035480: 2020 6578 6365 7074 204b 6579 4572 726f    except KeyErro
+00035490: 723a 0a20 2020 2020 2020 2023 2061 6464  r:.        # add
+000354a0: 206c 6f67 6963 2068 6572 6520 746f 2066   logic here to f
+000354b0: 696e 6420 6f6c 6465 7220 7061 7468 2077  ind older path w
+000354c0: 6865 6e20 7468 6520 6669 6c65 2068 6173  hen the file has
+000354d0: 2062 6565 6e20 6d6f 7665 6420 6f72 2072   been moved or r
+000354e0: 656e 616d 6564 0a20 2020 2020 2020 206c  enamed.        l
+000354f0: 6f67 6765 722e 6572 726f 7228 6622 7b72  ogger.error(f"{r
+00035500: 656c 5f70 6174 687d 2064 6964 206e 6f74  el_path} did not
+00035510: 2065 7869 7374 2061 7420 636f 6d6d 6974   exist at commit
+00035520: 207b 636f 6d6d 6974 5f69 6e66 6f7d 2e22   {commit_info}."
+00035530: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00035540: 204e 6f6e 652c 204e 6f6e 650a 2020 2020   None, None.    
+00035550: 7472 793a 0a20 2020 2020 2020 2077 6974  try:.        wit
+00035560: 6820 696f 2e42 7974 6573 494f 2874 6172  h io.BytesIO(tar
+00035570: 6765 7466 696c 652e 6461 7461 5f73 7472  getfile.data_str
+00035580: 6561 6d2e 7265 6164 2829 2920 6173 2066  eam.read()) as f
+00035590: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+000355a0: 7273 6564 203d 206c 6f61 645f 7473 7628  rsed = load_tsv(
+000355b0: 6629 0a20 2020 2065 7863 6570 7420 4578  f).    except Ex
+000355c0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+000355d0: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
+000355e0: 6f72 2866 2250 6172 7369 6e67 207b 7265  or(f"Parsing {re
+000355f0: 6c5f 7061 7468 7d20 4020 636f 6d6d 6974  l_path} @ commit
+00035600: 207b 636f 6d6d 6974 5f69 6e66 6f7d 2066   {commit_info} f
+00035610: 6169 6c65 6420 7769 7468 2074 6865 2066  ailed with the f
+00035620: 6f6c 6c6f 7769 6e67 2065 7863 6570 7469  ollowing excepti
+00035630: 6f6e 3a5c 6e7b 657d 2229 0a20 2020 2020  on:\n{e}").     
+00035640: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
+00035650: 4e6f 6e65 0a20 2020 206e 6577 5f66 696c  None.    new_fil
+00035660: 6520 3d20 7265 706c 6163 6528 6669 6c65  e = replace(file
+00035670: 2c20 636f 6d6d 6974 5f73 6861 3d63 6f6d  , commit_sha=com
+00035680: 6d69 745f 7368 6129 0a20 2020 2072 6574  mit_sha).    ret
+00035690: 7572 6e20 6e65 775f 6669 6c65 2c20 7061  urn new_file, pa
+000356a0: 7273 6564 0a0a 0a40 6675 6e63 7469 6f6e  rsed...@function
+000356b0: 5f6c 6f67 6765 720a 6465 6620 6368 6563  _logger.def chec
+000356c0: 6b5f 7068 7261 7365 5f61 6e6e 6f74 6174  k_phrase_annotat
+000356d0: 696f 6e73 2864 663a 2070 642e 4461 7461  ions(df: pd.Data
+000356e0: 4672 616d 652c 0a20 2020 2020 2020 2020  Frame,.         
+000356f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035700: 2020 2020 636f 6c75 6d6e 3a20 7374 7229      column: str)
+00035710: 202d 3e20 626f 6f6c 3a0a 2020 2020 2222   -> bool:.    ""
+00035720: 2222 2222 0a20 2020 2070 5f63 6f6c 203d  """".    p_col =
+00035730: 2064 665b 636f 6c75 6d6e 5d0a 2020 2020   df[column].    
+00035740: 6f70 656e 696e 6720 3d20 705f 636f 6c2e  opening = p_col.
+00035750: 6669 6c6c 6e61 2827 2729 2e73 7472 2e63  fillna('').str.c
+00035760: 6f75 6e74 2827 7b27 290a 2020 2020 636c  ount('{').    cl
+00035770: 6f73 696e 6720 3d20 705f 636f 6c2e 6669  osing = p_col.fi
+00035780: 6c6c 6e61 2827 2729 2e73 7472 2e63 6f75  llna('').str.cou
+00035790: 6e74 2827 7d27 290a 2020 2020 6966 2027  nt('}').    if '
+000357a0: 6d6e 5f70 6c61 7974 6872 6f75 6768 2720  mn_playthrough' 
+000357b0: 696e 2064 662e 636f 6c75 6d6e 733a 0a20  in df.columns:. 
+000357c0: 2020 2020 2020 2070 6f73 6974 696f 6e5f         position_
+000357d0: 636f 6c20 3d20 276d 6e5f 706c 6179 7468  col = 'mn_playth
+000357e0: 726f 7567 6827 0a20 2020 2065 6c73 653a  rough'.    else:
+000357f0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00035800: 696e 666f 2866 2243 6f6c 756d 6e20 276d  info(f"Column 'm
+00035810: 6e5f 706c 6179 7468 726f 7567 6827 2069  n_playthrough' i
+00035820: 7320 6d69 7373 696e 672c 2073 6f20 6d79  s missing, so my
+00035830: 2061 7373 6573 736d 656e 7420 6f66 2074   assessment of t
+00035840: 6865 2070 6872 6173 6520 616e 6e6f 7461  he phrase annota
+00035850: 7469 6f6e 7320 6d69 6768 7420 6265 2077  tions might be w
+00035860: 726f 6e67 2e22 290a 2020 2020 2020 2020  rong.").        
+00035870: 706f 7369 7469 6f6e 5f63 6f6c 203d 2027  position_col = '
+00035880: 6d6e 270a 2020 2020 636f 6c75 6d6e 7320  mn'.    columns 
+00035890: 3d20 5b70 6f73 6974 696f 6e5f 636f 6c2c  = [position_col,
+000358a0: 2063 6f6c 756d 6e5d 0a20 2020 2069 6620   column].    if 
+000358b0: 6f70 656e 696e 672e 7375 6d28 2920 213d  opening.sum() !=
+000358c0: 2063 6c6f 7369 6e67 2e73 756d 2829 3a0a   closing.sum():.
+000358d0: 2020 2020 2020 2020 6f20 3d20 6466 2e6c          o = df.l
+000358e0: 6f63 5b28 6f70 656e 696e 6720 3e20 3029  oc[(opening > 0)
+000358f0: 2c20 636f 6c75 6d6e 735d 0a20 2020 2020  , columns].     
+00035900: 2020 2063 203d 2064 662e 6c6f 635b 2863     c = df.loc[(c
+00035910: 6c6f 7369 6e67 203e 2030 292c 2063 6f6c  losing > 0), col
+00035920: 756d 6e73 5d0a 2020 2020 2020 2020 636f  umns].        co
+00035930: 6d70 6172 6520 3d20 7064 2e63 6f6e 6361  mpare = pd.conca
+00035940: 7428 5b6f 2e72 6573 6574 5f69 6e64 6578  t([o.reset_index
+00035950: 2864 726f 703d 5472 7565 292c 2063 2e72  (drop=True), c.r
+00035960: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
+00035970: 5472 7565 295d 2c20 6178 6973 3d31 290a  True)], axis=1).
+00035980: 2020 2020 2020 2020 6966 2027 6d6e 2720          if 'mn' 
+00035990: 696e 2063 6f6d 7061 7265 3a0a 2020 2020  in compare:.    
+000359a0: 2020 2020 2020 2020 636f 6d70 6172 6520          compare 
+000359b0: 3d20 636f 6d70 6172 652e 6173 7479 7065  = compare.astype
+000359c0: 287b 276d 6e27 3a20 2749 6e74 3634 277d  ({'mn': 'Int64'}
+000359d0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+000359e0: 2e77 6172 6e69 6e67 2866 2250 6872 6173  .warning(f"Phras
+000359f0: 6520 6265 6769 6e6e 696e 6720 616e 6420  e beginning and 
+00035a00: 656e 6469 6e67 7320 646f 6e27 7420 6d61  endings don't ma
+00035a10: 7463 683a 5c6e 7b63 6f6d 7061 7265 2e74  tch:\n{compare.t
+00035a20: 6f5f 7374 7269 6e67 2869 6e64 6578 3d46  o_string(index=F
+00035a30: 616c 7365 297d 222c 2065 7874 7261 3d7b  alse)}", extra={
+00035a40: 226d 6573 7361 6765 5f69 6422 3a20 2831  "message_id": (1
+00035a50: 362c 297d 290a 2020 2020 2020 2020 7265  6,)}).        re
+00035a60: 7475 726e 2046 616c 7365 0a20 2020 2072  turn False.    r
+00035a70: 6574 7572 6e20 5472 7565 0a              eturn True.
```

### Comparing `ms3-1.2.8/src/ms3/view.py` & `ms3-1.2.9/src/ms3/view.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -420,16 +420,14 @@
                 return msg
             print(msg)
             return
         if not self.fnames_in_metadata:
             msg_components.append("excludes fnames that are contained in the metadata")
         if not self.fnames_not_in_metadata:
             msg_components.append("excludes fnames that are not contained in the metadata")
-        if not self.fnames_with_incomplete_facets:
-            msg_components.append(f"excludes pieces that do not have at least one file per selected facet ({', '.join(self.selected_facets)})")
         if not self.include_convertible:
             msg_components.append("filters out file extensions requiring conversion (such as .xml)")
         if not self.include_tsv:
             msg_components.append("disregards all TSV files")
         if self.exclude_review:
             msg_components.append("excludes review files and folders")
         included_re = {what_to_include: [rgx for rgx in regexes if rgx not in self.registered_regexes]
@@ -456,14 +454,16 @@
                 excluded = f"'{re_strings[0]}'"
             elif n_excluded < 11:
                 excluded = 'one of ' + str(re_strings)
             else:
                 excluded = 'one of [' + ', '.join(f"'{regex}'" for regex in re_strings[:10]) + '... '
                 excluded += f" ({n_excluded - 10} more, see filtering_report())"
             msg_components.append(f"excludes any {what_to_exclude} containing {excluded}")
+        if not self.fnames_with_incomplete_facets:
+            msg_components.append(f"excludes pieces that do not have at least one file per selected facet ({', '.join(self.selected_facets)})")
         if len(self.excluded_file_paths) > 0:
             msg_components.append(f"excludes {len(self.excluded_file_paths)} files based on user input")
         msg = f"This view is called '{self.name}'. It "
         n_components = len(msg_components)
         if n_components == 0:
             msg += "selects everything."
         elif n_components == 1:
```

### Comparing `ms3-1.2.8/src/ms3.egg-info/PKG-INFO` & `ms3-1.2.9/src/ms3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms3
-Version: 1.2.8
+Version: 1.2.9
 Summary: A parser for annotated MuseScore 3 files.
 Home-page: https://github.com/johentsch/ms3
 Author: Johannes Hentschel
 Author-email: johannes.hentschel@epfl.ch
 License: gpl3
 Project-URL: Documentation, https://johentsch.github.io/ms3/
 Platform: any
```

### Comparing `ms3-1.2.8/src/ms3.egg-info/SOURCES.txt` & `ms3-1.2.9/src/ms3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

