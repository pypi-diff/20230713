# Comparing `tmp/pytango-9.4.1rc1.tar.gz` & `tmp/pytango-9.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytango-9.4.1rc1.tar", last modified: Fri Mar  3 14:37:11 2023, max compression
+gzip compressed data, was "pytango-9.4.2rc1.tar", last modified: Thu Jul 13 09:38:37 2023, max compression
```

## Comparing `pytango-9.4.1rc1.tar` & `pytango-9.4.2rc1.tar`

### file list

```diff
@@ -1,407 +1,412 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.761637 pytango-9.4.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     7879 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     8584 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/Makefile
--rw-r--r--   0 root         (0) root         (0)     6386 2023-03-03 14:37:11.765637 pytango-9.4.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/PyTango.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.725637 pytango-9.4.1rc1/cmake/
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/cmake/project_version.cc.in
--rw-rw-rw-   0 root         (0) root         (0)     7407 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/cmake/project_version.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/cmake/project_version.h.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.729637 pytango-9.4.1rc1/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.729637 pytango-9.4.1rc1/doc/.devcontainer/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/.devcontainer/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/.devcontainer/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.737637 pytango-9.4.1rc1/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)     5669 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/arrow03.png
--rw-rw-rw-   0 root         (0) root         (0)   237697 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/banner1.png
--rw-rw-rw-   0 root         (0) root         (0)    73015 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/banner2.png
--rw-rw-rw-   0 root         (0) root         (0)    83303 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/banner3.png
--rw-rw-rw-   0 root         (0) root         (0)     7419 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/boost_python_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.737637 pytango-9.4.1rc1/doc/_static/css/
--rw-rw-rw-   0 root         (0) root         (0)   132306 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/css/tango_cs_theme.css
--rw-rw-rw-   0 root         (0) root         (0)    13726 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/database.png
--rw-rw-rw-   0 root         (0) root         (0)    65909 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/device.png
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/gallery.js
--rw-rw-rw-   0 root         (0) root         (0)   603593 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/green_python.png
--rw-rw-rw-   0 root         (0) root         (0)  1684994 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/green_python_original.png
--rw-rw-rw-   0 root         (0) root         (0)     2765 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/ipython_db.html
--rw-rw-rw-   0 root         (0) root         (0)     3829 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/ipython_motor.html
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/ipython_serial.html
--rw-rw-rw-   0 root         (0) root         (0)    20483 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/ipython_tango.html
--rw-rw-rw-   0 root         (0) root         (0)    30674 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/itango00.png
--rw-rw-rw-   0 root         (0) root         (0)    14791 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/jive_powersupply.png
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/jssor.css
--rw-rw-rw-   0 root         (0) root         (0)    92207 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/jssor.js
--rw-rw-rw-   0 root         (0) root         (0)   170401 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/jssor.slider.js
--rw-rw-rw-   0 root         (0) root         (0)   172668 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/logo-medium.png
--rwxrwxrwx   0 root         (0) root         (0)     4030 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/logo.ico
--rw-rw-rw-   0 root         (0) root         (0)    99573 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/logo.png
--rw-rw-rw-   0 root         (0) root         (0)   221457 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/mocking-tango-db-access-crossed-out.png
--rw-rw-rw-   0 root         (0) root         (0)   145562 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/mocking-tango-db-access.png
--rw-rw-rw-   0 root         (0) root         (0)    63184 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/mocking-tango-test-case-not-mocked.png
--rw-rw-rw-   0 root         (0) root         (0)    54671 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/mocking-tango-test-case-real-vs-mocked.png
--rw-rw-rw-   0 root         (0) root         (0)   179107 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/mocking-tango-test-doubles.png
--rw-rw-rw-   0 root         (0) root         (0)    13299 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/motor.png
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/power_supply.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/project-config.jam
--rw-rw-rw-   0 root         (0) root         (0)     6201 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/pytango.css
--rw-rw-rw-   0 root         (0) root         (0)     6323 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/serial.png
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/slideshow.js
--rw-rw-rw-   0 root         (0) root         (0)    15763 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/starter.png
--rw-rw-rw-   0 root         (0) root         (0)   171117 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/testing-approaches-device-test-context-x2.png
--rw-rw-rw-   0 root         (0) root         (0)   211964 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/testing-approaches-device-test-context.png
--rw-rw-rw-   0 root         (0) root         (0)   206869 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/testing-approaches-hybrid.png
--rw-rw-rw-   0 root         (0) root         (0)   336790 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/testing-approaches-multi-device-test-context.png
--rw-rw-rw-   0 root         (0) root         (0)   108016 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_static/testing-approaches-real-facility.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.737637 pytango-9.4.1rc1/doc/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_templates/breadcrumbs.html
--rw-rw-rw-   0 root         (0) root         (0)    14238 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_templates/index.html
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/_templates/indexsidebar.html
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/api.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.737637 pytango-9.4.1rc1/doc/client_api/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/client_api/attribute_proxy.rst
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/client_api/device_proxy.rst
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/client_api/green.rst
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/client_api/group.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/client_api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/client_api/miscellaneous.rst
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/client_api/other.rst
--rw-rw-rw-   0 root         (0) root         (0)    18665 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/contents.rst
--rw-rw-rw-   0 root         (0) root         (0)    42078 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/data_types.rst
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/database.rst
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/encoded.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/environment.yml
--rw-rw-rw-   0 root         (0) root         (0)    12704 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/exception.rst
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/faq.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/doc/green_modes/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/green_modes/client_asyncio_mode.rst
--rw-rw-rw-   0 root         (0) root         (0)     3542 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/green_modes/client_futures_mode.rst
--rw-rw-rw-   0 root         (0) root         (0)     4036 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/green_modes/client_gevent_mode.rst
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/green_modes/green.rst
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/green_modes/green_modes_client.rst
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/green_modes/green_modes_server.rst
--rw-rw-rw-   0 root         (0) root         (0)     9713 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/how-to-contribute.rst
--rw-rw-rw-   0 root         (0) root         (0)    61818 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/howto.rst
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/indexes.rst
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/itango.rst
--rw-rw-rw-   0 root         (0) root         (0)   206038 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/logo-medium.bmp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/doc/man/
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/man/itango.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/doc/migration/
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/doc/migration/to-9.4/
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/attr-decorators.rst
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/deps-install.rst
--rw-rw-rw-   0 root         (0) root         (0)    16392 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/empty-attrs.rst
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/extract-as.rst
--rw-rw-rw-   0 root         (0) root         (0)     2075 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/hl-dev-enum.rst
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/hl-dynamic.rst
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/logging-percent-sym.rst
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/non-bound-user-funcs.rst
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/migration/to-9.4/optional-proxy-attrs.rst
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/mock_tango_extension.py
--rw-rw-rw-   0 root         (0) root         (0)     6793 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/news.rst
--rw-rw-rw-   0 root         (0) root         (0)     9178 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/quicktour.rst
--rw-rw-rw-   0 root         (0) root         (0)   163618 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/revision.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/doc/server_api/
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/server_api/attribute.rst
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/server_api/device.rst
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/server_api/device_class.rst
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/server_api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/server_api/logging.rst
--rw-rw-rw-   0 root         (0) root         (0)    10620 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/server_api/server.rst
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/server_api/util.rst
--rw-rw-rw-   0 root         (0) root         (0)     6447 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/start.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/doc/tep/
--rw-rw-rw-   0 root         (0) root         (0)    56811 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/tep/DataBase.xmi
--rw-rw-rw-   0 root         (0) root         (0)   100867 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/tep/database.py
--rw-rw-rw-   0 root         (0) root         (0)    19326 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/tep/tep-0001.rst
--rw-rw-rw-   0 root         (0) root         (0)    17205 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/tep/tep-0002.rst
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/tep.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/doc/testing/
--rw-rw-rw-   0 root         (0) root         (0)     8724 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/testing/mocks.rst
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/testing/test_context.rst
--rw-rw-rw-   0 root         (0) root         (0)    11017 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/testing/testing_approaches.rst
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/utilities.rst
--rw-rw-rw-   0 root         (0) root         (0)     6737 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/doc/windows_notes.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.725637 pytango-9.4.1rc1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/examples/Clock/
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/Clock/Clock.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/Clock/ClockDS.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/Clock/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/examples/TuringMachine/
--rw-rw-rw-   0 root         (0) root         (0)     2062 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/TuringMachine/TuringMachine.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/TuringMachine/turing_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/examples/asyncio_green_mode/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/asyncio_green_mode/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/asyncio_green_mode/asyncio_device_example.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/asyncio_green_mode/asyncio_simple_example.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/asyncio_green_mode/tcp_server_example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/examples/dynamic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/examples/dynamic/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/dynamic/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/dynamic/common/roi.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/dynamic/dynamic_client.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/dynamic/dynamic_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.741637 pytango-9.4.1rc1/examples/fwdAttr/
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/fwdAttr/FwdServer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/interfacechangeEvents/
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/ClassFactory.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeClient.py
--rw-rw-rw-   0 root         (0) root         (0)    11392 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5744 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.h
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.py
--rw-rw-rw-   0 root         (0) root         (0)     4643 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.xmi
--rw-rw-rw-   0 root         (0) root         (0)    21544 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerClass.cpp
--rw-rw-rw-   0 root         (0) root         (0)     7254 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerClass.h
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5037 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5095 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5095 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/Makefile.bck
--rw-rw-rw-   0 root         (0) root         (0)     2731 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/interfacechangeEvents/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/mandatory/
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/mandatory/MandatoryPropertyServer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/many/
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/many/many_client.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/many/many_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/multi/
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/multi/multi_client.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/multi/multi_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/multidevicetestcontext/
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/multidevicetestcontext/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2763 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/multidevicetestcontext/test_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/pipeEvents/
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/ClassFactory.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5047 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeEventClient.py
--rw-rw-rw-   0 root         (0) root         (0)    15129 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeServer.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeServer.h
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeServer.py
--rw-rw-rw-   0 root         (0) root         (0)     2512 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeServer.xmi
--rw-rw-rw-   0 root         (0) root         (0)    19277 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeServerClass.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5100 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeServerClass.h
--rw-rw-rw-   0 root         (0) root         (0)     3687 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/PipeServerStateMachine.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipeEvents/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/pipes/
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/ClassFactory.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5047 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeClient.py
--rw-rw-rw-   0 root         (0) root         (0)    11859 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeServer.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4416 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeServer.h
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeServer.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeServer.xmi
--rw-rw-rw-   0 root         (0) root         (0)    18280 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeServerClass.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4186 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeServerClass.h
--rw-rw-rw-   0 root         (0) root         (0)     3082 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/PipeServerStateMachine.cpp
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/pipes/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/simple/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/simple/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/simple/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/simple/common/roi.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/simple/simple_client.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/simple/simple_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.745637 pytango-9.4.1rc1/examples/training/
--rw-rw-rw-   0 root         (0) root         (0)     5106 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.749637 pytango-9.4.1rc1/examples/training/client/
--rwxrwxrwx   0 root         (0) root         (0)     1784 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/client/command01.py
--rwxrwxrwx   0 root         (0) root         (0)     1815 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/client/command02.py
--rwxrwxrwx   0 root         (0) root         (0)     1185 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/client/reading01.py
--rwxrwxrwx   0 root         (0) root         (0)     1636 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/client/reading02.py
--rwxrwxrwx   0 root         (0) root         (0)     5644 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/client/reading03.py
--rwxrwxrwx   0 root         (0) root         (0)     1251 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/client/writing01.py
--rwxrwxrwx   0 root         (0) root         (0)     1260 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/client/writing02.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.749637 pytango-9.4.1rc1/examples/training/server/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/high-level-api.py
--rwxrwxrwx   0 root         (0) root         (0)     1331 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/libps.py
--rwxrwxrwx   0 root         (0) root         (0)     1340 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/low-level-api.py
--rwxrwxrwx   0 root         (0) root         (0)     3831 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps-simulator.py
--rwxrwxrwx   0 root         (0) root         (0)      394 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps0a.py
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps0b-push-event.py
--rwxrwxrwx   0 root         (0) root         (0)      623 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps0b.py
--rwxrwxrwx   0 root         (0) root         (0)     1216 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps0c.py
--rwxrwxrwx   0 root         (0) root         (0)     1217 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps1-gevent.py
--rwxrwxrwx   0 root         (0) root         (0)     1154 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps1-use-lib-logging.py
--rwxrwxrwx   0 root         (0) root         (0)      943 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps1-use-lib.py
--rwxrwxrwx   0 root         (0) root         (0)     1119 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps1.py
--rwxrwxrwx   0 root         (0) root         (0)     1770 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps2-gevent-check.py
--rwxrwxrwx   0 root         (0) root         (0)     1462 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/ps2-gevent.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/test_ps0a.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/server/test_ps0b.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.749637 pytango-9.4.1rc1/examples/training/webinars/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/webinars/crash_example.py
--rw-rw-rw-   0 root         (0) root         (0)     3557 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/examples/training/webinars/test_webinar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.753637 pytango-9.4.1rc1/ext/
--rw-rw-rw-   0 root         (0) root         (0)     2498 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/api_util.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/archive_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/attr_conf_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/attribute_alarm_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/attribute_dimension.cpp
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/attribute_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/attribute_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1276 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/attribute_info_ex.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4095 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/attribute_proxy.cpp
--rw-rw-rw-   0 root         (0) root         (0)    16594 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/base_types.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/base_types_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)    15060 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/callback.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/callback.h
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/change_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/command_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5786 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/connection.cpp
--rw-rw-rw-   0 root         (0) root         (0)    18026 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/constants.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2842 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/data_ready_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)    19287 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/database.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4296 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/db.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/defs.h
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/dev_command_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/dev_error.cpp
--rw-rw-rw-   0 root         (0) root         (0)    30769 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     9721 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_attribute.h
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_attribute_config.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_attribute_history.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10170 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_attribute_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8504 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_data_history.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)    14245 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_pipe.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1743 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_pipe.h
--rw-rw-rw-   0 root         (0) root         (0)    42737 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/device_proxy.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2898 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/devintr_change_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12739 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/enums.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/exception.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3594 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/exception.h
--rw-rw-rw-   0 root         (0) root         (0)    18306 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/fast_from_py.h
--rw-rw-rw-   0 root         (0) root         (0)     9248 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/fast_from_py_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)    16064 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/from_py.cpp
--rw-rw-rw-   0 root         (0) root         (0)    26892 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/from_py.h
--rw-rw-rw-   0 root         (0) root         (0)    13470 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/group.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2717 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/group_reply.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1971 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/group_reply_list.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/locker_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/locking_thread.cpp
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/periodic_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/pipe_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1151 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/pipe_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/poll_device.cpp
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/precompiled_header.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/precompiled_header.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3343 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/pytango.cpp
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/pytgutils.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2021 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/pytgutils.h
--rw-rw-rw-   0 root         (0) root         (0)     6434 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/pyutils.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6325 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/pyutils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.757637 pytango-9.4.1rc1/ext/server/
--rw-rw-rw-   0 root         (0) root         (0)    10787 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/attr.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10786 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/attr.h
--rw-rw-rw-   0 root         (0) root         (0)    35043 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/attribute.h
--rw-rw-rw-   0 root         (0) root         (0)     3350 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/auto_monitor.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10637 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/command.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/command.h
--rw-rw-rw-   0 root         (0) root         (0)    15118 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/device_class.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6475 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/device_class.h
--rw-rw-rw-   0 root         (0) root         (0)    66602 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/device_impl.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12818 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/device_impl.h
--rw-rw-rw-   0 root         (0) root         (0)     7705 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/dserver.cpp
--rw-rw-rw-   0 root         (0) root         (0)    46331 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/encoded_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/fwdAttr.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6352 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/log4tango.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/multi_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1190 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/multi_class_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)    19095 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/pipe.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/pipe.h
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/subdev.cpp
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/tango_util.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4608 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/user_default_attr_prop.cpp
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/user_default_pipe_prop.cpp
--rw-rw-rw-   0 root         (0) root         (0)    23854 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/wattribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2575 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/server/wattribute_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3003 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/tango_numpy.h
--rw-rw-rw-   0 root         (0) root         (0)    24364 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/tgutils.h
--rw-rw-rw-   0 root         (0) root         (0)      885 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/time_val.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12585 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/to_py.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12370 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/to_py.h
--rw-rw-rw-   0 root         (0) root         (0)     5383 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/to_py_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/ext/version.cpp
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.757637 pytango-9.4.1rc1/pytango.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6386 2023-03-03 14:37:11.000000 pytango-9.4.1rc1/pytango.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13786 2023-03-03 14:37:11.000000 pytango-9.4.1rc1/pytango.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 14:37:11.000000 pytango-9.4.1rc1/pytango.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-03-03 14:37:11.000000 pytango-9.4.1rc1/pytango.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-03 14:37:11.000000 pytango-9.4.1rc1/pytango.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-03-03 14:37:11.765637 pytango-9.4.1rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    15681 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.761637 pytango-9.4.1rc1/tango/
--rw-rw-rw-   0 root         (0) root         (0)    10466 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5184 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/api_util.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/asyncio.py
--rw-rw-rw-   0 root         (0) root         (0)     2871 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/asyncio_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     4760 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/asyncio_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    15383 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/attr_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18234 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/attribute_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/auto_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)    29926 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/base_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2722 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/callback.py
--rw-rw-rw-   0 root         (0) root         (0)     8009 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/client.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/codec.py
--rw-rw-rw-   0 root         (0) root         (0)    23641 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.761637 pytango-9.4.1rc1/tango/databaseds/
--rw-rw-rw-   0 root         (0) root         (0)    56819 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/DataBase.xmi
--rwxrwxrwx   0 root         (0) root         (0)       88 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/DataBaseds
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9052 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/create_db.sql
--rw-rw-rw-   0 root         (0) root         (0)     6116 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/create_db_tables.sql
--rw-rw-rw-   0 root         (0) root         (0)    84031 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.761637 pytango-9.4.1rc1/tango/databaseds/db_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/db_access/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    69570 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/db_access/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/db_errors.py
--rwxrwxrwx   0 root         (0) root         (0)     3079 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/databaseds/mysql2sqlite.sh
--rw-rw-rw-   0 root         (0) root         (0)    99390 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/db.py
--rw-rw-rw-   0 root         (0) root         (0)     4349 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/device_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    35676 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/device_class.py
--rw-rw-rw-   0 root         (0) root         (0)     2528 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/device_data.py
--rw-rw-rw-   0 root         (0) root         (0)   112961 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/device_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)   102884 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/device_server.py
--rw-rw-rw-   0 root         (0) root         (0)    24876 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/encoded_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     6778 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     4377 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/futures.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/futures_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     4961 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     4908 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/gevent_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/globals.py
--rw-rw-rw-   0 root         (0) root         (0)     6465 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/green.py
--rw-rw-rw-   0 root         (0) root         (0)    30204 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/group.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/group_reply.py
--rw-rw-rw-   0 root         (0) root         (0)     3192 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/group_reply_list.py
--rw-rw-rw-   0 root         (0) root         (0)     9603 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/log4tango.py
--rw-rw-rw-   0 root         (0) root         (0)     5396 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/pipe_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/pytango_init.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/pytango_pprint.py
--rw-rw-rw-   0 root         (0) root         (0)    34284 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/pyutil.py
--rw-rw-rw-   0 root         (0) root         (0)     2789 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/release.py
--rw-rw-rw-   0 root         (0) root         (0)    67286 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/server.py
--rw-rw-rw-   0 root         (0) root         (0)     5680 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/tango_numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    19382 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/tango_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25662 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/test_context.py
--rw-rw-rw-   0 root         (0) root         (0)    10170 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5224 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/time_val.py
--rw-rw-rw-   0 root         (0) root         (0)    55988 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tango/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:37:11.761637 pytango-9.4.1rc1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tests/test_async.py
--rw-rw-rw-   0 root         (0) root         (0)    20231 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)    10853 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tests/test_event.py
--rw-rw-rw-   0 root         (0) root         (0)    89146 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tests/test_server.py
--rw-rw-rw-   0 root         (0) root         (0)    17460 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/tests/test_test_context.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-03-03 14:37:02.000000 pytango-9.4.1rc1/winsetup.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/
+-rw-r--r--   0 matveyev (30593) irc         (39)     6685 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/CMakeLists.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)     7883 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/LICENSE.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)      267 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/MANIFEST.in
+-rw-r--r--   0 matveyev (30593) irc         (39)     8584 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)     6385 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/PKG-INFO
+-rw-r--r--   0 matveyev (30593) irc         (39)     1560 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/PyTango.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5027 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/README.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.295756 pytango-9.4.2rc1/cmake/
+-rw-r--r--   0 matveyev (30593) irc         (39)      814 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/cmake/project_version.cc.in
+-rw-r--r--   0 matveyev (30593) irc         (39)     7407 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/cmake/project_version.cmake
+-rw-r--r--   0 matveyev (30593) irc         (39)     1672 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/cmake/project_version.h.in
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.299756 pytango-9.4.2rc1/doc/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.299756 pytango-9.4.2rc1/doc/.devcontainer/
+-rw-r--r--   0 matveyev (30593) irc         (39)      314 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/.devcontainer/Dockerfile
+-rw-r--r--   0 matveyev (30593) irc         (39)     1484 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/.devcontainer/README.md
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/_static/
+-rw-r--r--   0 matveyev (30593) irc         (39)     5669 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/arrow03.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   237697 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/banner1.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    73015 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/banner2.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    83303 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/banner3.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     7419 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_static/boost_python_install.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/_static/css/
+-rw-r--r--   0 matveyev (30593) irc         (39)   132306 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/css/tango_cs_theme.css
+-rw-r--r--   0 matveyev (30593) irc         (39)    13726 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/database.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    65909 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/device.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     1104 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/gallery.js
+-rw-r--r--   0 matveyev (30593) irc         (39)   603593 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/green_python.png
+-rw-r--r--   0 matveyev (30593) irc         (39)  1684994 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/green_python_original.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     2765 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_db.html
+-rw-r--r--   0 matveyev (30593) irc         (39)     3829 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_motor.html
+-rw-r--r--   0 matveyev (30593) irc         (39)     3909 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_serial.html
+-rw-r--r--   0 matveyev (30593) irc         (39)    20483 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_tango.html
+-rw-r--r--   0 matveyev (30593) irc         (39)    30674 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/itango00.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    14791 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jive_powersupply.png
+-rw-r--r--   0 matveyev (30593) irc         (39)      769 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jssor.css
+-rw-r--r--   0 matveyev (30593) irc         (39)    92207 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jssor.js
+-rw-r--r--   0 matveyev (30593) irc         (39)   170401 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jssor.slider.js
+-rw-r--r--   0 matveyev (30593) irc         (39)   172668 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/logo-medium.png
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     4030 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/logo.ico
+-rw-r--r--   0 matveyev (30593) irc         (39)    99573 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/logo.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   221457 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-db-access-crossed-out.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   145562 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-db-access.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    63184 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-not-mocked.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    54671 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-real-vs-mocked.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   179107 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-test-doubles.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    13299 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/motor.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     2455 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_static/power_supply.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      891 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/project-config.jam
+-rw-r--r--   0 matveyev (30593) irc         (39)     6201 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/pytango.css
+-rw-r--r--   0 matveyev (30593) irc         (39)     6323 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/serial.png
+-rw-r--r--   0 matveyev (30593) irc         (39)      720 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/slideshow.js
+-rw-r--r--   0 matveyev (30593) irc         (39)    15763 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/starter.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   171117 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context-x2.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   211964 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   206869 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-hybrid.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   336790 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-multi-device-test-context.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   108016 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-real-facility.png
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/_templates/
+-rw-r--r--   0 matveyev (30593) irc         (39)      695 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_templates/breadcrumbs.html
+-rw-r--r--   0 matveyev (30593) irc         (39)    14238 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_templates/index.html
+-rw-r--r--   0 matveyev (30593) irc         (39)      642 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_templates/indexsidebar.html
+-rw-r--r--   0 matveyev (30593) irc         (39)      246 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/api.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/client_api/
+-rw-r--r--   0 matveyev (30593) irc         (39)      111 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/attribute_proxy.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      187 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/client_api/device_proxy.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      474 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/client_api/green.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1157 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/group.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      139 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/index.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2410 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/miscellaneous.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1056 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/other.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    18665 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/conf.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      423 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/doc/contents.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    42078 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/data_types.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      493 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/database.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      171 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/encoded.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      120 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/environment.yml
+-rw-r--r--   0 matveyev (30593) irc         (39)    12704 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/exception.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1508 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/faq.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/green_modes/
+-rw-r--r--   0 matveyev (30593) irc         (39)      525 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/client_asyncio_mode.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     3542 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/client_futures_mode.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     4036 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/client_gevent_mode.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1220 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/green.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1204 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/green_modes_client.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2473 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/green_modes_server.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     9922 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/how-to-contribute.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    62310 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/howto.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)       61 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/indexes.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      524 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/itango.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)   206038 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/logo-medium.bmp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/man/
+-rw-r--r--   0 matveyev (30593) irc         (39)      451 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/man/itango.1
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/migration/
+-rw-r--r--   0 matveyev (30593) irc         (39)      212 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/index.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/migration/to-9.4/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1566 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/attr-decorators.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1156 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/deps-install.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    16392 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/empty-attrs.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2033 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/extract-as.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2075 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/hl-dev-enum.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      756 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/hl-dynamic.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      377 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/index.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1344 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/logging-percent-sym.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     3887 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/non-bound-user-funcs.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1997 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/optional-proxy-attrs.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     5186 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/mock_tango_extension.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     8020 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/doc/news.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     9178 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/quicktour.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)   170620 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/doc/revision.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/server_api/
+-rw-r--r--   0 matveyev (30593) irc         (39)      434 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/attribute.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      141 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/device.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)       98 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/device_class.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      158 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/index.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      419 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/logging.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    10620 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/server.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      101 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/util.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     6458 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/doc/start.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/doc/tep/
+-rw-r--r--   0 matveyev (30593) irc         (39)    56811 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep/DataBase.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)   100867 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/tep/database.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    19326 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep/tep-0001.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    17205 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep/tep-0002.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      222 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/doc/testing/
+-rw-r--r--   0 matveyev (30593) irc         (39)     3725 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/testing/coverage.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     8724 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/testing/mocks.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      643 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/testing/test_context.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    15469 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/testing/testing_approaches.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      276 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/testing.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1088 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/utilities.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2400 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/doc/version-policy.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     6737 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/windows_notes.txt
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.291756 pytango-9.4.2rc1/examples/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/Clock/
+-rw-r--r--   0 matveyev (30593) irc         (39)      315 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/Clock/Clock.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1867 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/Clock/ClockDS.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1490 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/Clock/client.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/TuringMachine/
+-rw-r--r--   0 matveyev (30593) irc         (39)     2062 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/TuringMachine/TuringMachine.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      447 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/TuringMachine/turing_client.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/asyncio_green_mode/
+-rw-r--r--   0 matveyev (30593) irc         (39)       38 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      969 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/asyncio_device_example.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      281 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/asyncio_simple_example.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1886 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/tcp_server_example.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/dynamic/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/dynamic/common/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/dynamic/common/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      285 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/dynamic/common/roi.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      638 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/dynamic/dynamic_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      958 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/dynamic/dynamic_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/fwdAttr/
+-rw-r--r--   0 matveyev (30593) irc         (39)      883 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/fwdAttr/FwdServer.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/interfacechangeEvents/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1954 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/ClassFactory.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1841 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeClient.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11392 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5744 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1926 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4643 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)    21544 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     7254 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     6341 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5037 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5095 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)     5095 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile.bck
+-rw-r--r--   0 matveyev (30593) irc         (39)     2731 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/main.cpp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/mandatory/
+-rw-r--r--   0 matveyev (30593) irc         (39)      576 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/mandatory/MandatoryPropertyServer.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/many/
+-rw-r--r--   0 matveyev (30593) irc         (39)      388 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/many/many_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      685 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/many/many_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/multi/
+-rw-r--r--   0 matveyev (30593) irc         (39)      700 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/multi/multi_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      955 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/multi/multi_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/multidevicetestcontext/
+-rw-r--r--   0 matveyev (30593) irc         (39)      960 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/examples/multidevicetestcontext/conftest.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2763 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/examples/multidevicetestcontext/test_integration.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/pipeEvents/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1926 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/ClassFactory.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5047 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)     1579 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeEventClient.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    15129 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4833 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     2977 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2512 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)    19277 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5100 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     3687 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServerStateMachine.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2719 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/main.cpp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/pipes/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1926 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/ClassFactory.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5047 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)      893 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipes/PipeClient.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11859 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4416 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1031 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2089 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)    18280 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServerClass.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4186 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServerClass.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     3082 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServerStateMachine.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2719 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/main.cpp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/simple/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/simple/common/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/simple/common/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      285 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/simple/common/roi.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      638 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/simple/simple_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      963 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/simple/simple_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/
+-rw-r--r--   0 matveyev (30593) irc         (39)     5106 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/README.md
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/client/
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1784 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/client/command01.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1815 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/client/command02.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1185 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/reading01.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1636 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/reading02.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     5644 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/reading03.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1251 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/client/writing01.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1260 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/writing02.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2444 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/docker-compose.yml
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/server/
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      412 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/high-level-api.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1331 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/libps.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1340 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/low-level-api.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     3831 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps-simulator.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      394 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0a.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1058 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0b-push-event.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      623 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0b.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1216 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0c.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1217 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1-gevent.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1154 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1-use-lib-logging.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      943 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1-use-lib.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1119 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1770 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps2-gevent-check.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1462 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps2-gevent.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      351 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/server/test_ps0a.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      929 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/test_ps0b.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/webinars/
+-rw-r--r--   0 matveyev (30593) irc         (39)      648 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/webinars/crash_example.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3557 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/webinars/test_webinar.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.323756 pytango-9.4.2rc1/ext/
+-rw-r--r--   0 matveyev (30593) irc         (39)     2498 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/api_util.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1102 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/archive_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2618 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attr_conf_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1299 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_alarm_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      872 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_dimension.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      989 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      921 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1276 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_info_ex.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4095 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_proxy.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    16584 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/base_types.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3388 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/base_types_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    15060 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/ext/callback.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4682 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/callback.h
+-rw-r--r--   0 matveyev (30593) irc         (39)      981 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/change_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      824 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/command_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5786 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/connection.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    18026 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/constants.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2842 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/data_ready_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    19287 2023-06-22 12:57:49.000000 pytango-9.4.2rc1/ext/database.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4296 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/db.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1228 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/ext/defs.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1321 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/dev_command_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2172 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/dev_error.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    33447 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/device_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     7614 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/device_attribute.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    13598 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute.h.gch
+-rw-r--r--   0 matveyev (30593) irc         (39)     2667 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_config.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1013 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_history.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    10170 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)  1831316 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_numpy.hpp.gch
+-rw-r--r--   0 matveyev (30593) irc         (39)     8332 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/device_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1185 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_data_history.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1120 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    14245 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_pipe.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1743 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_pipe.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    42737 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_proxy.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2898 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/devintr_change_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    12739 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/enums.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2951 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    18550 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/exception.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3594 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/exception.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    18306 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/fast_from_py.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     9248 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/fast_from_py_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    16044 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/from_py.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    26882 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/from_py.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    13470 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/group.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2717 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/group_reply.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1971 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/group_reply_list.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1204 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/locker_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      725 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/locking_thread.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      909 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/periodic_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2503 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pipe_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1151 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pipe_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1047 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/poll_device.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      577 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/precompiled_header.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1307 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/precompiled_header.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3343 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pytango.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      652 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pytgutils.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2021 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pytgutils.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     8373 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/pyutils.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     7427 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/pyutils.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    13598 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pyutils.h.gch
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.323756 pytango-9.4.2rc1/ext/server/
+-rw-r--r--   0 matveyev (30593) irc         (39)    10787 2023-07-05 13:49:12.000000 pytango-9.4.2rc1/ext/server/attr.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    10786 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/attr.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    34005 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/server/attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2860 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/attribute.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     3350 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/auto_monitor.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    10091 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/server/command.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1665 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/command.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    15118 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/device_class.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     6475 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/device_class.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    67588 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/ext/server/device_impl.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    13502 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/ext/server/device_impl.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     7705 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/dserver.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    46343 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/ext/server/encoded_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1084 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/fwdAttr.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     6352 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/log4tango.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2367 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/multi_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1190 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/multi_class_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    19095 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/pipe.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2568 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/pipe.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1904 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/subdev.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    11368 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/tango_util.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4608 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/user_default_attr_prop.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      911 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/user_default_pipe_prop.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    23854 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/ext/server/wattribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2575 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/wattribute_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3003 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/tango_numpy.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    24364 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/tgutils.h
+-rw-r--r--   0 matveyev (30593) irc         (39)      885 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/time_val.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    12585 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/to_py.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    12370 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/to_py.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     5383 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/to_py_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      723 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/version.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      554 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/pyproject.toml
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.327756 pytango-9.4.2rc1/pytango.egg-info/
+-rw-r--r--   0 matveyev (30593) irc         (39)     6385 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/PKG-INFO
+-rw-r--r--   0 matveyev (30593) irc         (39)    13372 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/SOURCES.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)        1 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/dependency_links.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       95 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/requires.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       21 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/top_level.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)      241 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/setup.cfg
+-rw-r--r--   0 matveyev (30593) irc         (39)    15707 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/setup.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.327756 pytango-9.4.2rc1/tango/
+-rw-r--r--   0 matveyev (30593) irc         (39)    10466 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5184 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/api_util.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4464 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/asyncio.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4016 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/tango/asyncio_executor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    15383 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/attr_data.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    18234 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/attribute_proxy.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2092 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/auto_monitor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    29926 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/base_types.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2722 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/callback.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     8009 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      621 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/codec.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    23142 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/connection.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/tango/databaseds/
+-rw-r--r--   0 matveyev (30593) irc         (39)    56819 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/DataBase.xmi
+-rwxr-xr-x   0 matveyev (30593) irc         (39)       88 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/databaseds/DataBaseds
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     9052 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/create_db.sql
+-rw-r--r--   0 matveyev (30593) irc         (39)     6116 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/create_db_tables.sql
+-rw-r--r--   0 matveyev (30593) irc         (39)    84031 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/databaseds/database.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/tango/databaseds/db_access/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/db_access/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    69570 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/databaseds/db_access/sqlite3.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      370 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/db_errors.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     3079 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/mysql2sqlite.sh
+-rw-r--r--   0 matveyev (30593) irc         (39)    99390 2023-06-22 12:57:49.000000 pytango-9.4.2rc1/tango/db.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4349 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/device_attribute.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    35676 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/device_class.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2528 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/device_data.py
+-rw-r--r--   0 matveyev (30593) irc         (39)   112961 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/device_proxy.py
+-rw-r--r--   0 matveyev (30593) irc         (39)   105543 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/device_server.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    24876 2023-07-11 13:23:50.000000 pytango-9.4.2rc1/tango/encoded_attribute.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     6778 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/exception.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4377 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/futures.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1950 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/futures_executor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4961 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/gevent.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4908 2023-06-19 08:20:41.000000 pytango-9.4.2rc1/tango/gevent_executor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3186 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/globals.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     6364 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/tango/green.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    30204 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/group.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3468 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/group_reply.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3192 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/group_reply_list.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     9633 2023-07-05 13:49:23.000000 pytango-9.4.2rc1/tango/log4tango.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5396 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pipe.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     7405 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pipe_data.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3883 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pytango_init.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     6463 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pytango_pprint.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    34307 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/pyutil.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2789 2023-07-13 09:20:11.000000 pytango-9.4.2rc1/tango/release.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    71542 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/server.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5680 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/tango_numpy.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    19382 2023-06-19 08:20:41.000000 pytango-9.4.2rc1/tango/tango_object.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    26277 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/test_context.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11603 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/test_utils.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5224 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/time_val.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    55988 2023-07-11 13:23:50.000000 pytango-9.4.2rc1/tango/utils.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/tests/
+-rw-r--r--   0 matveyev (30593) irc         (39)     3001 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/tests/conftest.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      209 2023-07-05 14:13:23.000000 pytango-9.4.2rc1/tests/report.xml
+-rw-r--r--   0 matveyev (30593) irc         (39)     1890 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tests/test_async.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    20138 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tests/test_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    10853 2023-06-19 08:03:31.000000 pytango-9.4.2rc1/tests/test_event.py
+-rw-r--r--   0 matveyev (30593) irc         (39)   111640 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/tests/test_server.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    18428 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tests/test_test_context.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2423 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/winsetup.py
```

### Comparing `pytango-9.4.1rc1/CMakeLists.txt` & `pytango-9.4.2rc1/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,16 @@
         ext/server/pipe.h
         ext/pytgutils.h
         ext/pyutils.h
         ext/tango_numpy.h
         ext/tgutils.h
         ext/to_py.h)
 
-set(BOOST_VCSTR "140")
-set(BOOST_VERSION_ "1_73")
+set(BOOST_VCSTR "142")
+set(BOOST_VERSION_ "1_82")
 set(ZMQ_VCSTR "141")
 set(ZMQ_VERSION_ "4_0_5")
 
 set(RELEASE "Release_$ENV{PYTHON_VER}_${PY_TARGET}")
 include_directories("${CMAKE_CURRENT_SOURCE_DIR}/ext")
 include_directories("$ENV{TANGO_ROOT}/include")
 include_directories("$ENV{PYTHON_ROOT}/include")
```

### Comparing `pytango-9.4.1rc1/LICENSE.txt` & `pytango-9.4.2rc1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -163,8 +163,8 @@
 apply, that proxy's public statement of acceptance of any version is
 permanent authorization for you to choose that version for the
 Library.
 
 
 Portions of the code are licensed under different licences, listed below:
 
-tango/asyncio_tools.py coroutine function:  CPython, Python Software Foundation License Version 2, https://github.com/python/cpython/blob/3.10/LICENSE
+tango/asyncio_executor.py _coroutine function:  CPython, Python Software Foundation License Version 2, https://github.com/python/cpython/blob/3.10/LICENSE
```

### Comparing `pytango-9.4.1rc1/Makefile` & `pytango-9.4.2rc1/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/PKG-INFO` & `pytango-9.4.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytango
-Version: 9.4.1rc1
+Version: 9.4.2rc1
 Summary: A python binding for the Tango control system
 Home-page: http://gitlab.com/tango-controls/pytango
+Download-URL: http://pypi.python.org/pypi/pytango
 Author: Tiago Coutinho
 Author-email: coutinho@esrf.fr
 License: LGPL
-Download-URL: http://pypi.python.org/pypi/pytango
 Keywords: Tango,CORBA,binding
 Platform: Linux
 Platform: Windows XP/Vista/7/8/10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides: tango
 Provides: PyTango
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: gevent
 License-File: LICENSE.txt
 
 PyTango
 =======
@@ -185,8 +185,7 @@
 .. _IPython: http://ipython.org
 
 .. _documentation: http://pytango.readthedocs.io/en/latest
 .. _Tango forums: http://tango-controls.org/community/forum
 .. _PR and bug reports: PyTango_
 .. _sources: PyTango_
 .. _How to Contribute: http://pytango.readthedocs.io/en/latest/how-to-contribute.html#how-to-contribute
-
```

### Comparing `pytango-9.4.1rc1/PyTango.py` & `pytango-9.4.2rc1/PyTango.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/README.rst` & `pytango-9.4.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/cmake/project_version.cc.in` & `pytango-9.4.2rc1/cmake/project_version.cc.in`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/cmake/project_version.cmake` & `pytango-9.4.2rc1/cmake/project_version.cmake`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/cmake/project_version.h.in` & `pytango-9.4.2rc1/cmake/project_version.h.in`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/.devcontainer/README.md` & `pytango-9.4.2rc1/doc/.devcontainer/README.md`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/arrow03.png` & `pytango-9.4.2rc1/doc/_static/arrow03.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/banner1.png` & `pytango-9.4.2rc1/doc/_static/banner1.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/banner2.png` & `pytango-9.4.2rc1/doc/_static/banner2.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/banner3.png` & `pytango-9.4.2rc1/doc/_static/banner3.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/boost_python_install.py` & `pytango-9.4.2rc1/doc/_static/boost_python_install.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/css/tango_cs_theme.css` & `pytango-9.4.2rc1/doc/_static/css/tango_cs_theme.css`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/database.png` & `pytango-9.4.2rc1/doc/_static/database.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/device.png` & `pytango-9.4.2rc1/doc/_static/device.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/gallery.js` & `pytango-9.4.2rc1/doc/_static/gallery.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/green_python.png` & `pytango-9.4.2rc1/doc/_static/green_python.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/green_python_original.png` & `pytango-9.4.2rc1/doc/_static/green_python_original.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/ipython_db.html` & `pytango-9.4.2rc1/doc/_static/ipython_db.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/ipython_motor.html` & `pytango-9.4.2rc1/doc/_static/ipython_motor.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/ipython_serial.html` & `pytango-9.4.2rc1/doc/_static/ipython_serial.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/ipython_tango.html` & `pytango-9.4.2rc1/doc/_static/ipython_tango.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/itango00.png` & `pytango-9.4.2rc1/doc/_static/itango00.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/jive_powersupply.png` & `pytango-9.4.2rc1/doc/_static/jive_powersupply.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/jssor.css` & `pytango-9.4.2rc1/doc/_static/jssor.css`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/jssor.js` & `pytango-9.4.2rc1/doc/_static/jssor.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/jssor.slider.js` & `pytango-9.4.2rc1/doc/_static/jssor.slider.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/logo-medium.png` & `pytango-9.4.2rc1/doc/_static/logo-medium.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/logo.ico` & `pytango-9.4.2rc1/doc/_static/logo.ico`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/logo.png` & `pytango-9.4.2rc1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/mocking-tango-db-access-crossed-out.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-db-access-crossed-out.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/mocking-tango-db-access.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-db-access.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/mocking-tango-test-case-not-mocked.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-not-mocked.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/mocking-tango-test-case-real-vs-mocked.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-real-vs-mocked.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/mocking-tango-test-doubles.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-test-doubles.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/motor.png` & `pytango-9.4.2rc1/doc/_static/motor.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/power_supply.py` & `pytango-9.4.2rc1/doc/_static/power_supply.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/project-config.jam` & `pytango-9.4.2rc1/doc/_static/project-config.jam`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/pytango.css` & `pytango-9.4.2rc1/doc/_static/pytango.css`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/serial.png` & `pytango-9.4.2rc1/doc/_static/serial.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/slideshow.js` & `pytango-9.4.2rc1/doc/_static/slideshow.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/starter.png` & `pytango-9.4.2rc1/doc/_static/starter.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/testing-approaches-device-test-context-x2.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context-x2.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/testing-approaches-device-test-context.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/testing-approaches-hybrid.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-hybrid.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/testing-approaches-multi-device-test-context.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-multi-device-test-context.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_static/testing-approaches-real-facility.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-real-facility.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_templates/breadcrumbs.html` & `pytango-9.4.2rc1/doc/_templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_templates/index.html` & `pytango-9.4.2rc1/doc/_templates/index.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/_templates/indexsidebar.html` & `pytango-9.4.2rc1/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/client_api/group.rst` & `pytango-9.4.2rc1/doc/client_api/group.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/client_api/miscellaneous.rst` & `pytango-9.4.2rc1/doc/client_api/miscellaneous.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/client_api/other.rst` & `pytango-9.4.2rc1/doc/client_api/other.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/conf.py` & `pytango-9.4.2rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/data_types.rst` & `pytango-9.4.2rc1/doc/data_types.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/exception.rst` & `pytango-9.4.2rc1/doc/exception.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/faq.rst` & `pytango-9.4.2rc1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/green_modes/client_asyncio_mode.rst` & `pytango-9.4.2rc1/doc/green_modes/client_asyncio_mode.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/green_modes/client_futures_mode.rst` & `pytango-9.4.2rc1/doc/green_modes/client_futures_mode.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/green_modes/client_gevent_mode.rst` & `pytango-9.4.2rc1/doc/green_modes/client_gevent_mode.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/green_modes/green.rst` & `pytango-9.4.2rc1/doc/green_modes/green.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/green_modes/green_modes_client.rst` & `pytango-9.4.2rc1/doc/green_modes/green_modes_client.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/green_modes/green_modes_server.rst` & `pytango-9.4.2rc1/doc/green_modes/green_modes_server.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/how-to-contribute.rst` & `pytango-9.4.2rc1/doc/how-to-contribute.rst`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 ---------------------------
 
 Documentation is written in reStructuredText_ and built with Sphinx_ - it's easy to contribute.
 It also uses autodoc_ importing docstrings from tango package.
 Theme is not important, a theme prepared for Tango Community can be also used.
 
 To test the docs locally requires Python >= 3.6:
-      - ``$ python -m pip install numpy sphinx sphinx_rtd_theme``
+      - ``$ python -m pip install gevent numpy packaging pillow psutil sphinx sphinx_rtd_theme``
       - ``$ python -m sphinx doc build/sphinx``
 
 To test the docs locally in a Sphinx Docker container:
       - ``(host) $ cd /path/to/pytango``
       - ``(host) $ docker run --rm -ti -v $PWD:/docs sphinxdoc/sphinx bash``
-      - ``(container) $ python -m pip install numpy sphinx_rtd_theme``
+      - ``(container) $ python -m pip install gevent numpy psutil sphinx_rtd_theme``
       - ``(container) $ python -m sphinx doc build/sphinx``
 
 After building, open the ``build/doc/index.html`` page in your browser.
 
 Source code standard
 --------------------
 
@@ -101,17 +101,16 @@
 For example:
  - ``docker run --rm -ti artefact.skao.int/ska-tango-images-tango-pytango:9.3.12``
 
 
 Releasing a new version
 -----------------------
 
-From time to time a new version should be released.  Anyone who wishes to see some
-features of the development branch released is free to make a new release.  The basic
-steps required are as follows:
+Starting from 9.4.2 pytango tries to follow cpptango releases with the delay up to ~1 month.
+The basic steps to make a new release are as follows:
 
 Pick a version number
   * A 3-part version numbering scheme is used:  <major>.<minor>.<patch>
   * Note that PyTango **does not** follow `Semantic Versioning <https://semver.org>`_.
     API changes can occur at minor releases (but avoid them if at all possible).
   * The major and minor version fields (e.g., 9.4) track the TANGO C++ core version.
   * Small changes are done as patch releases.  For these the version
@@ -122,14 +121,17 @@
       - changes to ``9.4.4`` (the actual release)
       - changes to ``9.4.5.dev0`` (bump the patch version at the end of the release process)
   * Minor release example:
       - ``9.4.4.devN`` or ``9.4.4rcN`` (current development branch)
       - changes to ``9.5.0`` (the actual release)
       - changes to ``9.5.1.dev0`` (bump the patch version at the end of the release process)
 
+Check which versions of Python should this release support
+ * Follow the :ref:`version policy <pytango-version-policy>` and modify correspondingly python_requires and minimum runtime dependency for NumPy in setup.py
+
 Create an issue in GitLab
   * This is to inform the community that a release is planned.
   * Use a checklist similar to the one below:
 
     | Task list:
     | - [ ] Read steps in the how-to-contribute docs for making a release
     | - [ ] Merge request to update changelog and bump version
```

### Comparing `pytango-9.4.1rc1/doc/howto.rst` & `pytango-9.4.2rc1/doc/howto.rst`

 * *Files 1% similar despite different names*

```diff
@@ -405,35 +405,42 @@
 	runworkers()
 
 After `cleanup()` all references to :class:`~tango.DeviceProxy`,
 :class:`~tango.AttributeProxy` or :class:`~tango.Database` objects
 in the current process become invalid
 and these objects need to be reconstructed.
 
-Using clients with multithreading
----------------------------------
+Multithreading - clients and servers
+------------------------------------
 
 When performing Tango I/O from user-created threads, there can be problems.
-This is often more noticeable with event subscription and unsubscription,
-but it could affect any Tango I/O.  As PyTango wraps the cppTango library,
-we needs to consider how cppTango's threads work.
+This is often more noticeable with event subscription/unsubscription, and
+when pushing events, but it could affect any Tango I/O.
 
+A client subscribing and unsubscribing to events via a user thread may see
+a crash, a deadlock, or ``Event channel is not responding anymore`` errors.
+
+A device server pushing events from a user-created thread (including asyncio
+callbacks) might see ``Not able to acquire serialization (dev, class or process) monitor``
+errors.
+
+As PyTango wraps the cppTango library, we need to consider how cppTango's threads work.
 cppTango was originally developed at a time where C++ didn't have standard
-threads. All the threads currently created in cppTango are omni threads,
+threads. All the threads currently created in cppTango are "omni threads",
 since this is what the omniORB library is using to create threads and since
 this implementation is available for free with omniORB.
 
 In C++, users used to create omni threads in the past so there was no issue.
 Since C++11, C++ comes with an implementation of standard threads.
-cppTango is currently (version 9.3.3) not directly thread safe when
+cppTango is currently (version 9.4.1) not directly thread safe when
 a user is using C++11 standard threads or threads different than omni threads.
 This lack of thread safety includes threads created from Python's
 :mod:`threading` module.
 
-In an ideal future cppTango should should protect itself, regardless
+In an ideal future cppTango should protect itself, regardless
 of what type of threads are used.  In the meantime, we need a work-around.
 
 The work-around when using threads which are not omni threads is to create an
 object of the C++ class ``omni_thread::ensure_self`` in the user thread, just
 after the thread creation, and to delete this object only when the thread
 has finished its job. This ``omni_thread::ensure_self`` object provides a
 dummy omniORB ID for the thread. This ID is used when accessing thread
@@ -868,23 +875,23 @@
 
 If you are still using the low-level API with a <Device>Class instead of just a <Device>,
 then you can use the generic device_factory's call to the
 :meth:`~tango.DeviceClass.dyn_attr` method.
 It is simply necessary to re-define this method within your <Device>Class and to create
 the dynamic attributes within this method.
 
-Internally, the high-level API re-defines dyn_attr() to call initialize_dynamic_attributes()
-for each device.
+Internally, the high-level API re-defines :meth:`~tango.DeviceClass.dyn_attr` to call
+:meth:`~tango.server.Device.initialize_dynamic_attributes` for each device.
 
-.. note:: The dyn_attr() (and initialize_dynamic_attributes() for high-level API) methods
-          are only called once when the device server starts, since the Python device_factory
-          method is only called once. Within the device_factory method, init_device() is
-          called for all devices and only after that is dyn_attr() called for all devices.
-          If the Init command is executed on a device it will not call the dyn_attr() method
-          again.
+.. note:: The ``dyn_attr()`` (and ``initialize_dynamic_attributes()`` for high-level API) methods
+          are only called **once** when the device server starts, since the Python device_factory
+          method is only called once. Within the device_factory method, ``init_device()`` is
+          called for all devices and only after that is ``dyn_attr()`` called for all devices.
+          If the ``Init`` command is executed on a device it will not call the ``dyn_attr()`` method
+          again (and will not call ``initialize_dynamic_attributes()`` either).
 
 There is another point to be noted regarding dynamic attributes within a Python
 device server. The Tango Python device server core checks that for each
 static attribute there exists methods named <attribute_name>_read and/or
 <attribute_name>_write and/or is_<attribute_name>_allowed. Using dynamic
 attributes, it is not possible to define these methods because attribute names
 and number are known only at run-time.
```

### Comparing `pytango-9.4.1rc1/doc/itango.rst` & `pytango-9.4.2rc1/doc/itango.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/logo-medium.bmp` & `pytango-9.4.2rc1/doc/logo-medium.bmp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/attr-decorators.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/attr-decorators.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/deps-install.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/deps-install.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/empty-attrs.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/empty-attrs.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/extract-as.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/extract-as.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/hl-dev-enum.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/hl-dev-enum.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/hl-dynamic.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/hl-dynamic.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/logging-percent-sym.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/logging-percent-sym.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/non-bound-user-funcs.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/non-bound-user-funcs.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/migration/to-9.4/optional-proxy-attrs.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/optional-proxy-attrs.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/mock_tango_extension.py` & `pytango-9.4.2rc1/doc/mock_tango_extension.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/news.rst` & `pytango-9.4.2rc1/doc/news.rst`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,68 @@
     :maxdepth: 1
 
     migration/index
     History of changes <revision>
 
 
 ****************************
+What's new in PyTango 9.4.2?
+****************************
+
+Date: 2023-07-??
+
+Type: minor release
+
+Changed
+=======
+
+- New python and NumPy :ref:`version policy <pytango-version-policy>` is implemented.
+
+Added
+=====
+
+- Correct code coverage of server's methods can be obtained
+- server_init_hook was added to high-level and low-level API
+- macOS wheels now are provided
+
+Fixed
+=====
+
+- DevEncoded attributes and commands read methods are now segfault safe
+- DevEncoded attributes and commands now decoded with utf-8
+- DevEncoded attributes and commands can be extracted and written as str, bytes and bytesarray
+- If string encoding with Latin-1 fails, UnicodeError will be raised instead of segfaulting
+- When user gives empty spectrum properties to the DeviceTestContext,
+  they will be patched with one space symbol " " for each element
+- In case patching failed or any other problems with FileDatabase, instead of crash PyTango will raise an exception
+  and print out generated file
+- Regression when applying additional decorators on attribute accessor functions.  Method calls
+  would have the wrong signature and fail.
+
+Removed
+=======
+
+- Support for Python < 3.9. See :ref:`version policy <pytango-version-policy>`
+
+****************************
 What's new in PyTango 9.4.1?
 ****************************
 
-Date: unreleased  (9.4.1rc1 on 2023-03-03)
+Date: 2023-03-15
 
 Type: major release (breaking changes compared to 9.4.0)
 
 Changed
 =======
 
 - Removed additional function signatures for high-level attribute read/write/is_allowed
   methods that were added in 9.4.0 resulting in a regression.  For example, the high-level
   write method API for dynamic attributes of the form ``write_method(self, attr, value)``
   has been removed, leaving only ``write_method(self, attr)``.  Similarly, unbound functions
-  that could used without a reference to the device object, like ``read_function()``, are no
+  that could be used without a reference to the device object, like ``read_function()``, are no
   longer supported - only ``read_function(device)``.
   See the :ref:`migration guide <to9.4_non_bound_user_funcs>`.
 - The dependencies packaged with the binary PyPI wheels are as follows:
     - Linux:
         - cpptango: 9.4.1
         - omniorb: 4.2.5  (changed since PyTango 9.4.0)
         - libzmq: v4.3.4
```

### Comparing `pytango-9.4.1rc1/doc/quicktour.rst` & `pytango-9.4.2rc1/doc/quicktour.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/revision.rst` & `pytango-9.4.2rc1/doc/revision.rst`

 * *Files 2% similar despite different names*

```diff
@@ -115,51 +115,87 @@
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 | 07/09/22 | `9.3.5 <http://pytango.readthedocs.io/en/v9.3.5>`_                               | 9.3.5 Release                                       | Y\. Matveev                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 | 28/09/22 | `9.3.6 <http://pytango.readthedocs.io/en/v9.3.6>`_                               | 9.3.6 Release                                       | Y\. Matveev                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 | 15/02/23 | `9.4.0 <http://pytango.readthedocs.io/en/v9.4.0>`_                               | 9.4.0 Release                                       | A\. Joubert                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
-| ??/??/?? | `9.4.1 <http://pytango.readthedocs.io/en/v9.4.1>`_                               | 9.4.1 Release                                       | A\. Joubert                       |
+| 15/03/23 | `9.4.1 <http://pytango.readthedocs.io/en/v9.4.1>`_                               | 9.4.1 Release                                       | A\. Joubert                       |
++----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
+| ??/07/23 | `9.4.2 <http://pytango.readthedocs.io/en/v9.4.2>`_                               | 9.4.2 Release                                       | Y\. Matveev                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 
 .. _pytango-version-history:
 
 Version history
 ---------------
 
 +----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Version  | Changes                                                                                                                                                                             |
 +==========+=====================================================================================================================================================================================+
-| 9.4.1rc1 | *Release candidate 1 for 9.4.1*.                                                                                                                                                    |
+| 9.4.2rc1 | Release candidate 1 for 9.4.2.                                                                                                                                                      |
+|          |                                                                                                                                                                                     |
+|          | Features:                                                                                                                                                                           |
+|          |     - `!578: Add server init hook to high-level and low-level devices <https://gitlab.com/tango-controls/pytango/-/merge_requests/578>`_                                            |
+|          |     - `!562: Check code coverage <https://gitlab.com/tango-controls/pytango/-/merge_requests/562>`_                                                                                 |
+|          |     - `!577: Implement new python and NumPy version policy <https://gitlab.com/tango-controls/pytango/-/merge_requests/577>`_                                                       |
+|          |                                                                                                                                                                                     |
+|          | Bug fixes and changes:                                                                                                                                                              |
+|          |     - `!551: Handle unsupported DeviceTestContext properties gracefully <https://gitlab.com/tango-controls/pytango/-/merge_requests/551>`_                                          |
+|          |     - `!556: Fix source location recorded by logging decorators <https://gitlab.com/tango-controls/pytango/-/merge_requests/556>`_                                                  |
+|          |     - `!564: Asyncio server doesn't change state to ALARM with AttrQuality <https://gitlab.com/tango-controls/pytango/-/merge_requests/564>`                                        |
+|          |     - `!557: Fix DevEncoded attributes and commands <https://gitlab.com/tango-controls/pytango/-/merge_requests/557>`_                                                              |
+|          |     - `!565: Raise UnicodeError instead of segfaulting when Latin-1 encoding fails <https://gitlab.com/tango-controls/pytango/-/merge_requests/565>`_                               |
+|          |     - `!570: Fix linter problem in winsetup.py <https://gitlab.com/tango-controls/pytango/-/merge_requests/570>`_                                                                   |
+|          |     - `!579: Extend "empty string workaround" to sequences for DeviceTestContext properties <https://gitlab.com/tango-controls/pytango/-/merge_requests/579>`_                      |
+|          |                                                                                                                                                                                     |
+|          | Doc fixes:                                                                                                                                                                          |
+|          |     - `!571: Update new build system doc <https://gitlab.com/tango-controls/pytango/-/merge_requests/571>`_                                                                         |
+|          |     - `!572: Improve docs for push_data_ready_event and EnsureOmniThread <https://gitlab.com/tango-controls/pytango/-/merge_requests/572>`_                                         |
+|          |     - `!587: Update docs and bump version for 9.4.2rc1 <https://gitlab.com/tango-controls/pytango/-/merge_requests/587>`_                                                           |
+|          |                                                                                                                                                                                     |
+|          |                                                                                                                                                                                     |
+|          | DevOps changes:                                                                                                                                                                     |
+|          |     - `!563: Skip log location tests in AppVeyor CI <https://gitlab.com/tango-controls/pytango/-/merge_requests/563>`_                                                              |
+|          |     - `!566: Add AppVeyor Windows builds for Python 3.9 to 3.11, Boost 1.82.0 <https://gitlab.com/tango-controls/pytango/-/merge_requests/566>`_                                    |
+|          |     - `!575: Add job to test main cpptango branch <https://gitlab.com/tango-controls/pytango/-/merge_requests/575>`_                                                                |
+|          |     - `!574: Added test for checking default and non-default units <https://gitlab.com/tango-controls/pytango/-/merge_requests/574>`_                                               |
+|          |     - `!576: Add macOS wheels + gitlab-ci cleaning <https://gitlab.com/tango-controls/pytango/-/merge_requests/576>`_                                                               |
+|          |     - `!585: Move to cppTango 9.4.2, drop Python<3.9 on Win, update wheel deps <https://gitlab.com/tango-controls/pytango/-/merge_requests/585>`_                                   |
+|          |                                                                                                                                                                                     |
+|          | More details in the `full changelog 9.4.1...9.4.2 <https://gitlab.com/tango-controls/pytango/-/compare/v9.4.1...v9.4.2>`_                                                           |
+|          |                                                                                                                                                                                     |
++==========+=====================================================================================================================================================================================+
+| 9.4.1    | 9.4.1 release.                                                                                                                                                                      |
 |          |                                                                                                                                                                                     |
 |          | Bug fixes and changes:                                                                                                                                                              |
 |          |     - `!547: Fix attributes with device inheritance and repeated method wrapping regression in 9.4.0 <https://gitlab.com/tango-controls/pytango/-/merge_requests/547>`_             |
 |          |     - `!548: Fix decorated attribute methods regression in 9.4.0 <https://gitlab.com/tango-controls/pytango/-/merge_requests/548>`_                                                 |
 |          |                                                                                                                                                                                     |
 |          | Doc fixes:                                                                                                                                                                          |
 |          |     - `!546: Add note about pip version for binary packages <https://gitlab.com/tango-controls/pytango/-/merge_requests/546>`_                                                      |
 |          |     - `!544: Bump version to 9.4.1dev0 <https://gitlab.com/tango-controls/pytango/-/merge_requests/544>`_                                                                           |
 |          |     - `!555: Update docs and bump version for 9.4.0rc1 <https://gitlab.com/tango-controls/pytango/-/merge_requests/555>`_                                                           |
-|          |     - `!xyz: Bump for 9.4.1 <https://gitlab.com/tango-controls/pytango/-/merge_requests/xyz>`_                                                                                      |
+|          |     - `!559: Groom docstrings <https://gitlab.com/tango-controls/pytango/-/merge_requests/559>`_                                                                                    |
+|          |     - `!560: Bump for 9.4.1 <https://gitlab.com/tango-controls/pytango/-/merge_requests/560>`_                                                                                      |
 |          |                                                                                                                                                                                     |
 |          | Deprecation fixes:                                                                                                                                                                  |
 |          |     - `!553: Remove compiler version check from setup.py <https://gitlab.com/tango-controls/pytango/-/merge_requests/553>`_                                                         |
 |          |                                                                                                                                                                                     |
 |          | DevOps changes:                                                                                                                                                                     |
 |          |     - `!545: Run black on repo and add to pre-commit-config <https://gitlab.com/tango-controls/pytango/-/merge_requests/545>`_                                                      |
 |          |     - `!554: Update to omniorb 4.2.5 for Linux wheels <https://gitlab.com/tango-controls/pytango/-/merge_requests/554>`_                                                            |
 |          |     - `!549: Use new tango-controls group runners <https://gitlab.com/tango-controls/pytango/-/merge_requests/549>`_                                                                |
 |          |     - `!550: Update mambaforge image and use conda instead of apt packages in CI <https://gitlab.com/tango-controls/pytango/-/merge_requests/550>`_                                 |
 |          |     - `!552: Run gitlab-triage to update old issues/MRs <https://gitlab.com/tango-controls/pytango/-/merge_requests/552>`_                                                          |
 |          |                                                                                                                                                                                     |
-|          | More details in the `full changelog 9.4.0...9.4.1rc1 <https://gitlab.com/tango-controls/pytango/-/compare/v9.4.0...v9.4.1rc1>`_                                                     |
+|          | More details in the `full changelog 9.4.0...9.4.1 <https://gitlab.com/tango-controls/pytango/-/compare/v9.4.0...v9.4.1>`_                                                           |
 |          |                                                                                                                                                                                     |
 +----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| 9.4.0    | 9.4.0 release.                                                                                                                                                                      |
+| 9.4.0    | 9.4.0 release (not recommended due to significant regressions).                                                                                                                     |
 |          |                                                                                                                                                                                     |
 |          | Features:                                                                                                                                                                           |
 |          |     - `!522: Support of non-bound methods for attributes <https://gitlab.com/tango-controls/pytango/-/merge_requests/522>`_                                                         |
 |          |     - `!535: Allow developer to optionally add attributes to a DeviceProxy instance <https://gitlab.com/tango-controls/pytango/-/merge_requests/535>`_                              |
 |          |     - `!515: DevEnum spectrum and image attributes support added <https://gitlab.com/tango-controls/pytango/-/merge_requests/515>`_                                                 |
 |          |     - `!502: Provide binary wheels on PyPI using pytango-builder images <https://gitlab.com/tango-controls/pytango/-/merge_requests/502>`_                                          |
 |          |     - `!510: Added high level API for dynamic attributes <https://gitlab.com/tango-controls/pytango/-/merge_requests/510>`_                                                         |
```

### Comparing `pytango-9.4.1rc1/doc/server_api/server.rst` & `pytango-9.4.2rc1/doc/server_api/server.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/start.rst` & `pytango-9.4.2rc1/doc/start.rst`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 Conda
 ~~~~~
 
 The basic steps are shown below (specify your Python version).
 
 .. sourcecode:: console
 
-   $ conda create -n pytangodev -c conda-forge boost cpptango tango-test cppzmq cxx-compiler gevent numpy packaging pkg-config psutil pytest pytest-forked python=3.11
+   $ conda create -n pytangodev -c conda-forge boost cpptango tango-test cppzmq cxx-compiler gevent numpy packaging pkg-config psutil pytest pytest-forked pytest-cov python=3.11
    $ conda activate pytangodev
    $ git clone https://gitlab.com/tango-controls/pytango.git
    $ cd pytango
    $ export BOOST_ROOT=$CONDA_PREFIX TANGO_ROOT=$CONDA_PREFIX ZMQ_ROOT=$CONDA_PREFIX OMNI_ROOT=$CONDA_PREFIX
    $ export BOOST_PYTHON_LIB=boost_python$(python -c "import sys; print(f'{sys.version_info.major}{sys.version_info.minor}')")
    $ pip install -v -e ".[tests]"
    $ pytest
```

### Comparing `pytango-9.4.1rc1/doc/tep/DataBase.xmi` & `pytango-9.4.2rc1/doc/tep/DataBase.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/tep/database.py` & `pytango-9.4.2rc1/doc/tep/database.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/tep/tep-0001.rst` & `pytango-9.4.2rc1/doc/tep/tep-0001.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/tep/tep-0002.rst` & `pytango-9.4.2rc1/doc/tep/tep-0002.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/testing/mocks.rst` & `pytango-9.4.2rc1/doc/testing/mocks.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/testing/test_context.rst` & `pytango-9.4.2rc1/doc/testing/test_context.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/utilities.rst` & `pytango-9.4.2rc1/doc/utilities.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/doc/windows_notes.txt` & `pytango-9.4.2rc1/doc/windows_notes.txt`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/Clock/ClockDS.py` & `pytango-9.4.2rc1/examples/Clock/ClockDS.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/Clock/client.py` & `pytango-9.4.2rc1/examples/Clock/client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/TuringMachine/TuringMachine.py` & `pytango-9.4.2rc1/examples/TuringMachine/TuringMachine.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/asyncio_green_mode/asyncio_device_example.py` & `pytango-9.4.2rc1/examples/asyncio_green_mode/asyncio_device_example.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/asyncio_green_mode/tcp_server_example.py` & `pytango-9.4.2rc1/examples/asyncio_green_mode/tcp_server_example.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/dynamic/dynamic_client.py` & `pytango-9.4.2rc1/examples/dynamic/dynamic_client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/dynamic/dynamic_server.py` & `pytango-9.4.2rc1/examples/dynamic/dynamic_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/fwdAttr/FwdServer.py` & `pytango-9.4.2rc1/examples/fwdAttr/FwdServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/ClassFactory.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/ClassFactory.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeClient.py` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeClient.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.h` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.py` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServer.xmi` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerClass.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerClass.h` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/Makefile` & `pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/Makefile.bck` & `pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile.bck`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/interfacechangeEvents/main.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/main.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/mandatory/MandatoryPropertyServer.py` & `pytango-9.4.2rc1/examples/mandatory/MandatoryPropertyServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/many/many_server.py` & `pytango-9.4.2rc1/examples/many/many_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/multi/multi_client.py` & `pytango-9.4.2rc1/examples/multi/multi_client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/multi/multi_server.py` & `pytango-9.4.2rc1/examples/multi/multi_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/multidevicetestcontext/conftest.py` & `pytango-9.4.2rc1/examples/multidevicetestcontext/conftest.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/multidevicetestcontext/test_integration.py` & `pytango-9.4.2rc1/examples/multidevicetestcontext/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/ClassFactory.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/ClassFactory.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/Makefile` & `pytango-9.4.2rc1/examples/pipeEvents/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeEventClient.py` & `pytango-9.4.2rc1/examples/pipeEvents/PipeEventClient.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeServer.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeServer.h` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeServer.py` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeServer.xmi` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeServerClass.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeServerClass.h` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/PipeServerStateMachine.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServerStateMachine.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipeEvents/main.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/main.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/ClassFactory.cpp` & `pytango-9.4.2rc1/examples/pipes/ClassFactory.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/Makefile` & `pytango-9.4.2rc1/examples/pipes/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeClient.py` & `pytango-9.4.2rc1/examples/pipes/PipeClient.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeServer.cpp` & `pytango-9.4.2rc1/examples/pipes/PipeServer.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeServer.h` & `pytango-9.4.2rc1/examples/pipes/PipeServer.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeServer.py` & `pytango-9.4.2rc1/examples/pipes/PipeServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeServer.xmi` & `pytango-9.4.2rc1/examples/pipes/PipeServer.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeServerClass.cpp` & `pytango-9.4.2rc1/examples/pipes/PipeServerClass.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeServerClass.h` & `pytango-9.4.2rc1/examples/pipes/PipeServerClass.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/PipeServerStateMachine.cpp` & `pytango-9.4.2rc1/examples/pipes/PipeServerStateMachine.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/pipes/main.cpp` & `pytango-9.4.2rc1/examples/pipes/main.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/simple/simple_client.py` & `pytango-9.4.2rc1/examples/simple/simple_client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/simple/simple_server.py` & `pytango-9.4.2rc1/examples/simple/simple_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/README.md` & `pytango-9.4.2rc1/examples/training/README.md`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/client/command01.py` & `pytango-9.4.2rc1/examples/training/client/command01.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/client/command02.py` & `pytango-9.4.2rc1/examples/training/client/command02.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/client/reading01.py` & `pytango-9.4.2rc1/examples/training/client/reading01.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/client/reading02.py` & `pytango-9.4.2rc1/examples/training/client/reading02.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/client/reading03.py` & `pytango-9.4.2rc1/examples/training/client/reading03.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/client/writing01.py` & `pytango-9.4.2rc1/examples/training/client/writing01.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/client/writing02.py` & `pytango-9.4.2rc1/examples/training/client/writing02.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/docker-compose.yml` & `pytango-9.4.2rc1/examples/training/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/libps.py` & `pytango-9.4.2rc1/examples/training/server/libps.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/low-level-api.py` & `pytango-9.4.2rc1/examples/training/server/low-level-api.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps-simulator.py` & `pytango-9.4.2rc1/examples/training/server/ps-simulator.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps0b-push-event.py` & `pytango-9.4.2rc1/examples/training/server/ps0b-push-event.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps0b.py` & `pytango-9.4.2rc1/examples/training/server/ps0b.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps0c.py` & `pytango-9.4.2rc1/examples/training/server/ps0c.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps1-gevent.py` & `pytango-9.4.2rc1/examples/training/server/ps1-gevent.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps1-use-lib-logging.py` & `pytango-9.4.2rc1/examples/training/server/ps1-use-lib-logging.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps1-use-lib.py` & `pytango-9.4.2rc1/examples/training/server/ps1-use-lib.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps1.py` & `pytango-9.4.2rc1/examples/training/server/ps1.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps2-gevent-check.py` & `pytango-9.4.2rc1/examples/training/server/ps2-gevent-check.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/ps2-gevent.py` & `pytango-9.4.2rc1/examples/training/server/ps2-gevent.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/server/test_ps0b.py` & `pytango-9.4.2rc1/examples/training/server/test_ps0b.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/webinars/crash_example.py` & `pytango-9.4.2rc1/examples/training/webinars/crash_example.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/examples/training/webinars/test_webinar.py` & `pytango-9.4.2rc1/examples/training/webinars/test_webinar.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/api_util.cpp` & `pytango-9.4.2rc1/ext/api_util.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/archive_event_info.cpp` & `pytango-9.4.2rc1/ext/archive_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/attr_conf_event_data.cpp` & `pytango-9.4.2rc1/ext/attr_conf_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/attribute_alarm_info.cpp` & `pytango-9.4.2rc1/ext/attribute_alarm_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/attribute_dimension.cpp` & `pytango-9.4.2rc1/ext/attribute_dimension.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/attribute_event_info.cpp` & `pytango-9.4.2rc1/ext/attribute_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/attribute_info.cpp` & `pytango-9.4.2rc1/ext/attribute_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/attribute_info_ex.cpp` & `pytango-9.4.2rc1/ext/attribute_info_ex.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/attribute_proxy.cpp` & `pytango-9.4.2rc1/ext/attribute_proxy.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/base_types.cpp` & `pytango-9.4.2rc1/ext/base_types.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                           boost::python::converter::rvalue_from_python_stage1_data* data)
     {
       bool decref = false;
 
       if (PyUnicode_Check(obj))
       {
           decref = true;
-          obj = PyUnicode_AsLatin1String(obj);
+          obj = EncodeAsLatin1(obj);
       }
 
       const char* value = PyBytes_AsString(obj);
       Py_ssize_t size = PyBytes_Size(obj);
 
       // Grab pointer to memory into which to construct the new std::string
       void* storage = (
```

### Comparing `pytango-9.4.1rc1/ext/base_types_numpy.hpp` & `pytango-9.4.2rc1/ext/base_types_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/callback.cpp` & `pytango-9.4.2rc1/ext/callback.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/callback.h` & `pytango-9.4.2rc1/ext/callback.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/change_event_info.cpp` & `pytango-9.4.2rc1/ext/change_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/command_info.cpp` & `pytango-9.4.2rc1/ext/command_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/connection.cpp` & `pytango-9.4.2rc1/ext/connection.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/constants.cpp` & `pytango-9.4.2rc1/ext/constants.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/data_ready_event_data.cpp` & `pytango-9.4.2rc1/ext/data_ready_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/database.cpp` & `pytango-9.4.2rc1/ext/database.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/db.cpp` & `pytango-9.4.2rc1/ext/db.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/defs.h` & `pytango-9.4.2rc1/ext/defs.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/dev_command_info.cpp` & `pytango-9.4.2rc1/ext/dev_command_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/dev_error.cpp` & `pytango-9.4.2rc1/ext/dev_error.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 namespace PyDevError
 {
     static void from_str_to_char(PyObject* in, CORBA::String_member& out)
     {
         if (PyUnicode_Check(in))
         {
-            PyObject *bytes_in = PyUnicode_AsLatin1String(in);
+            PyObject *bytes_in = EncodeAsLatin1(in);
             out = CORBA::string_dup(PyBytes_AsString(bytes_in));
             Py_DECREF(bytes_in);
         }
         else 
         {
             out = CORBA::string_dup(PyBytes_AsString(in));
         }
```

### Comparing `pytango-9.4.1rc1/ext/device_attribute.cpp` & `pytango-9.4.2rc1/ext/device_attribute.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -143,27 +143,26 @@
             {
                 Tango::DevEncoded& w_buffer = buffer[1];
                 bopy::str w_encoded_format(w_buffer.encoded_format);
 
                 Tango::DevVarCharArray& w_encoded_data_array = w_buffer.encoded_data;
                 char* w_ch_ptr = (char*) w_encoded_data_array.get_buffer();
                 PyObject* w_encoded_data_ptr = NULL;
-                    PyByteArray_FromStringAndSize(w_ch_ptr, w_encoded_data_array.length());
                 Py_ssize_t w_size = w_encoded_data_array.length();
                 if (read_only)
                 {
                     w_encoded_data_ptr = PyBytes_FromStringAndSize(w_ch_ptr, w_size);
                 }
                 else
                 {
                     w_encoded_data_ptr = PyByteArray_FromStringAndSize(w_ch_ptr, w_size);
                 }
                 bopy::object w_encoded_data = bopy::object(bopy::handle<>(w_encoded_data_ptr));
 
-                py_value.attr(value_attr_name) =
+                py_value.attr(w_value_attr_name) =
                     bopy::make_tuple(w_encoded_format, w_encoded_data);
             }
         }
         else
         {
             py_value.attr(w_value_attr_name) = bopy::object();
         }
@@ -224,18 +223,15 @@
         Tango::DevEncoded* buffer = value_ptr->get_buffer();
 
         Tango::DevEncoded& r_buffer = buffer[0];
         bopy::str r_encoded_format(r_buffer.encoded_format);
 
         Tango::DevVarCharArray& r_encoded_data_array = r_buffer.encoded_data;
         char* r_ch_ptr = (char*)r_encoded_data_array.get_buffer();
-
-        bopy::object r_encoded_data(
-            bopy::handle<>(PyBytes_FromStringAndSize(
-                r_ch_ptr, r_encoded_data_array.length())));
+        bopy::str r_encoded_data(r_ch_ptr, r_encoded_data_array.length());
 
         py_value.attr(value_attr_name) =
             bopy::make_tuple(r_encoded_format, r_encoded_data);
 
         if (self.get_written_dim_x() > 0)
         {
             bool is_write_type = self.get_written_dim_x() && (value_ptr->length() < 2);
@@ -249,18 +245,15 @@
             else
             {
                 Tango::DevEncoded& w_buffer = buffer[1];
                 bopy::str w_encoded_format(w_buffer.encoded_format);
 
                 Tango::DevVarCharArray& w_encoded_data_array = w_buffer.encoded_data;
                 char* w_ch_ptr = (char*)w_encoded_data_array.get_buffer();
-
-                bopy::object w_encoded_data(
-                    bopy::handle<>(PyBytes_FromStringAndSize(
-                        w_ch_ptr, w_encoded_data_array.length())));
+                bopy::str w_encoded_data(w_ch_ptr, w_encoded_data_array.length());
 
                 py_value.attr(w_value_attr_name) =
                     bopy::make_tuple(w_encoded_format, w_encoded_data);
             }
         }
         else
         {
@@ -300,15 +293,15 @@
         }
     }
 
     template<> inline void
     _update_scalar_values<Tango::DEV_ENCODED>(Tango::DeviceAttribute &self,
                                               bopy::object py_value)
     {
-        _update_value_as_string<Tango::DEV_ENCODED>(self, py_value);
+        _update_value_as_bin<Tango::DEV_ENCODED>(self, py_value, true);
     }
 
     template<> inline void
     _update_scalar_values<Tango::DEV_STRING>(Tango::DeviceAttribute &self,
                                              bopy::object py_value)
     {
         if (self.get_written_dim_x() > 0)
@@ -667,14 +660,80 @@
                                              const bopy::object & py_value)
     {
         /// @todo really? This is really not gonna happen?
         // Unsupported
         assert(false);
     }
 
+    template<long tangoTypeConst>
+    static inline void _fill_scalar_attribute(Tango::DeviceAttribute & dev_attr,
+                                              const boost::python::object & py_value)
+    {
+        typedef typename TANGO_const2type(tangoTypeConst) TangoScalarType;
+
+        TangoScalarType value;
+        from_py<tangoTypeConst>::convert(py_value.ptr(), value);
+        dev_attr << const_cast<TangoScalarType&>(value);
+    }
+
+    template<>
+    inline void _fill_scalar_attribute<Tango::DEV_STRING>(Tango::DeviceAttribute & dev_attr,
+                                                          const boost::python::object & py_value)
+    {
+        std::string value = from_str_to_char(py_value.ptr());
+        dev_attr << value;
+    }
+
+    template<>
+    inline void _fill_scalar_attribute<Tango::DEV_ENCODED>(Tango::DeviceAttribute & dev_attr,
+                                                           const boost::python::object & py_value)
+    {
+        if (boost::python::len(py_value) != 2) {
+            raise_(PyExc_TypeError, "Expecting a tuple of strings: encoded_format, encoded_data");
+        }
+
+        boost::python::object encoded_format_str = py_value[0];
+        boost::python::object encoded_data_str = py_value[1];
+
+        // todo second parameter of insert is a reference, and it does not take ownership of the pointer
+        // so to be 100% sure, we have to copy data. However, in this case we have to have an option to control release parameter.
+        // At the moment (cppTango 9.4.1) it is not realized, so we pass pointer to data and Python's gb destroys object
+        // this is a source of bugs. Somehow it works, but no idea why.
+
+        char* encoded_format = const_cast<char*>((boost::python::extract<const char*>(encoded_format_str)()));
+
+        Py_ssize_t encoded_data_len = boost::python::len(encoded_data_str);
+        PyObject* encoded_data_obj = encoded_data_str.ptr();
+        unsigned char* encoded_data;
+
+        if (PyUnicode_Check(encoded_data_obj))
+        {
+            Py_ssize_t size;
+            encoded_data = reinterpret_cast<unsigned char*>((char*)PyUnicode_AsUTF8AndSize(encoded_data_obj, &size));
+            dev_attr.insert(encoded_format, encoded_data, static_cast<unsigned int>(size));
+        }
+        else if (PyBytes_Check(encoded_data_obj) || PyByteArray_Check(encoded_data_obj))
+        {
+            Py_buffer view;
+
+            if (PyObject_GetBuffer(encoded_data_obj, &view, PyBUF_FULL_RO) < 0)
+            {
+                raise_(PyExc_TypeError, "Cannot convert encoded data");
+            }
+
+            encoded_data = reinterpret_cast<unsigned char*>((char*)view.buf);
+            dev_attr.insert(encoded_format, encoded_data, static_cast<unsigned int>(encoded_data_len));
+            PyBuffer_Release(&view);
+        }
+        else
+        {
+            raise_(PyExc_TypeError, "Encoded_data can be str, bytes or bytearray");
+        }
+    }
+
     static inline bopy::object
     undefined_attribute(Tango::DeviceAttribute* self)
     {
         return object(); // None
     }
 
     void
@@ -730,15 +789,14 @@
                 attr_info = dev_proxy.get_attribute_config(attr_name);
             }
             catch(...)
             {}
         }
         reset_values(self, attr_info.data_type, attr_info.data_format, py_value);
     }
-
 };
 
 void export_device_attribute()
 {
     class_<Tango::DeviceAttribute> DeviceAttribute("DeviceAttribute",
         init<>())
     ;
```

### Comparing `pytango-9.4.1rc1/ext/device_attribute.h` & `pytango-9.4.2rc1/ext/device_attribute.h`

 * *Files 18% similar despite different names*

```diff
@@ -182,56 +182,8 @@
     /// @param extract_as See ExtractAs enum.
     template<typename TDeviceAttribute>
     boost::python::object convert_to_python(TDeviceAttribute* dev_attr, Tango::DeviceProxy & dev_proxy, PyTango::ExtractAs extract_as)
     {
         update_data_format(dev_proxy, dev_attr, 1);
         return convert_to_python(dev_attr, extract_as);
     }
-    
-
-    template<long tangoTypeConst>
-    static inline void _fill_scalar_attribute(Tango::DeviceAttribute & dev_attr, const boost::python::object & py_value)
-    {
-        typedef typename TANGO_const2type(tangoTypeConst) TangoScalarType;
-
-        TangoScalarType value;
-        from_py<tangoTypeConst>::convert(py_value.ptr(), value);
-        dev_attr << const_cast<TangoScalarType&>(value);
-    }
-
-    template<>
-    inline void _fill_scalar_attribute<Tango::DEV_STRING>(Tango::DeviceAttribute & dev_attr, const boost::python::object & py_value)
-    {
-        std::string value;
-	from_str_to_char(py_value.ptr(), value);
-        dev_attr << value;
-    }
-
-    template<>
-    inline void _fill_scalar_attribute<Tango::DEV_ENCODED>(Tango::DeviceAttribute & dev_attr, const boost::python::object & py_value)
-    {
-        /// @todo test it!!
-
-        /// @todo Now I am accepting 2 strings: encoded_format, encoded_data. This
-        /// is far from a good solution, but its something...
-
-        if (boost::python::len(py_value) != 2) {
-            raise_(PyExc_TypeError, "Expecting a tuple of strings: encoded_format, encoded_data");
-        }
-
-        boost::python::object encoded_format_str = py_value[0];
-        boost::python::object encoded_data_str = py_value[1];
-
-        /// @todo not sure... second parameter of insert is a reference, does it
-        /// mean anything? Does he pretend to take ownership of the pointer or
-        /// is he making another copy? what should I do?
-        char* encoded_format = const_cast<char*>((boost::python::extract<const char*>(encoded_format_str)()));
-        Py_ssize_t encoded_data_len = boost::python::len(encoded_data_str);
-        unsigned char* encoded_data = reinterpret_cast<unsigned char*>(const_cast<char*>((boost::python::extract<const char*>(encoded_data_str)())));
-        // void insert(char *&,unsigned char *&,unsigned int);
-        dev_attr.insert(encoded_format, encoded_data, static_cast<unsigned int>(encoded_data_len));
-
-        //std::string value = boost::python::extract<std::string>(py_value);
-        //dev_attr << value;
-    }
-
 }
```

### Comparing `pytango-9.4.1rc1/ext/device_attribute_config.cpp` & `pytango-9.4.2rc1/ext/device_attribute_config.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/device_attribute_history.cpp` & `pytango-9.4.2rc1/ext/device_attribute_history.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/device_attribute_numpy.hpp` & `pytango-9.4.2rc1/ext/device_attribute_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/device_data.cpp` & `pytango-9.4.2rc1/ext/device_data.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -38,39 +38,37 @@
 
         template <>
         void insert_scalar<Tango::DEV_STRING>(Tango::DeviceData &self, object py_value)
         {
 	    PyObject* py_value_ptr = py_value.ptr();
 	    if(PyUnicode_Check(py_value_ptr))
 	    {
-		PyObject* obj_bytes_ptr = PyUnicode_AsLatin1String(py_value_ptr);
+		PyObject* obj_bytes_ptr = EncodeAsLatin1(py_value_ptr);
 		Tango::DevString value = PyBytes_AsString(obj_bytes_ptr);
 		self << value;
 		Py_DECREF(obj_bytes_ptr);
 	    }
 	    else
 	    {
 		Tango::DevString value = PyBytes_AsString(py_value_ptr);
 		self << value;
 	    }
 	}
 
         template <>
         void insert_scalar<Tango::DEV_ENCODED>(Tango::DeviceData &self, object py_value)
         {
+            Tango::DevEncoded val;
             object p0 = py_value[0];
-            object p1 = py_value[1];
             const char* encoded_format = extract<const char*> (p0.ptr());
-            const char* encoded_data = extract<const char*> (p1.ptr());
-            
-            CORBA::ULong nb = static_cast<CORBA::ULong>(boost::python::len(p1));
-            Tango::DevVarCharArray arr(nb, nb, (CORBA::Octet*)encoded_data, false);
-            Tango::DevEncoded val;
             val.encoded_format = CORBA::string_dup(encoded_format);
-            val.encoded_data = arr;
+
+            view_pybytes_as_char_array(py_value[1], val.encoded_data);
+            // By giving a value (not a pointer) to << the data will be copied by CORBA
+
             self << val;
         }
 
         template <>
         void insert_scalar<Tango::DEV_VOID>(Tango::DeviceData &self, object py_value)
         {
             raise_(PyExc_TypeError, "Trying to insert a value in a DEV_VOID DeviceData!");
```

### Comparing `pytango-9.4.1rc1/ext/device_data_history.cpp` & `pytango-9.4.2rc1/ext/device_data_history.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/device_info.cpp` & `pytango-9.4.2rc1/ext/device_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/device_pipe.cpp` & `pytango-9.4.2rc1/ext/device_pipe.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/device_pipe.h` & `pytango-9.4.2rc1/ext/device_pipe.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/device_proxy.cpp` & `pytango-9.4.2rc1/ext/device_proxy.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/devintr_change_event_data.cpp` & `pytango-9.4.2rc1/ext/devintr_change_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/enums.cpp` & `pytango-9.4.2rc1/ext/enums.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/event_data.cpp` & `pytango-9.4.2rc1/ext/event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/exception.cpp` & `pytango-9.4.2rc1/ext/exception.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/exception.h` & `pytango-9.4.2rc1/ext/exception.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/fast_from_py.h` & `pytango-9.4.2rc1/ext/fast_from_py.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/fast_from_py_numpy.hpp` & `pytango-9.4.2rc1/ext/fast_from_py_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/from_py.cpp` & `pytango-9.4.2rc1/ext/from_py.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     
     if (PyBytes_Check(py_value_ptr))
     {
         result.push_back(PyBytes_AS_STRING(py_value_ptr));
     }
     else if(PyUnicode_Check(py_value_ptr))
     {
-        PyObject* py_bytes_value_ptr = PyUnicode_AsLatin1String(py_value_ptr);
+        PyObject* py_bytes_value_ptr = EncodeAsLatin1(py_value_ptr);
         result.push_back(PyBytes_AS_STRING(py_bytes_value_ptr));
         Py_DECREF(py_bytes_value_ptr);
     }
     else
     {
         size_t size = boost::python::len(py_value);
         result.reserve(size);
@@ -91,15 +91,15 @@
     if (PyBytes_Check(py_value_ptr))
     {
         result.length(1);
         result[0] = CORBA::string_dup(PyBytes_AS_STRING(py_value_ptr));
     }
     else if(PyUnicode_Check(py_value_ptr))
     {
-        PyObject* py_bytes_value_ptr = PyUnicode_AsLatin1String(py_value_ptr);
+        PyObject* py_bytes_value_ptr = EncodeAsLatin1(py_value_ptr);
         result.length(1);
         result[0] = CORBA::string_dup(PyBytes_AS_STRING(py_bytes_value_ptr));
         Py_DECREF(py_bytes_value_ptr);
     }
     else
     {
         CORBA::ULong size = static_cast<CORBA::ULong>(boost::python::len(py_value));
```

### Comparing `pytango-9.4.1rc1/ext/from_py.h` & `pytango-9.4.2rc1/ext/from_py.h`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             PyObject *o_ptr = PySequence_GetItem(seq_ptr, i);
             if (PyBytes_Check(o_ptr))
             {
                 a.push_back(Tango::DbDatum(PyBytes_AS_STRING(o_ptr)));
             }
             else if(PyUnicode_Check(o_ptr))
             {
-                PyObject* o_bytes_ptr = PyUnicode_AsLatin1String(o_ptr);
+                PyObject* o_bytes_ptr = EncodeAsLatin1(o_ptr);
                 a.push_back(Tango::DbDatum(PyBytes_AS_STRING(o_bytes_ptr)));
                 Py_DECREF(o_bytes_ptr);
             }
         }
     }
 
     /**
```

### Comparing `pytango-9.4.1rc1/ext/group.cpp` & `pytango-9.4.2rc1/ext/group.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/group_reply.cpp` & `pytango-9.4.2rc1/ext/group_reply.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/group_reply_list.cpp` & `pytango-9.4.2rc1/ext/group_reply_list.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/locker_info.cpp` & `pytango-9.4.2rc1/ext/locker_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/locking_thread.cpp` & `pytango-9.4.2rc1/ext/locking_thread.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/periodic_event_info.cpp` & `pytango-9.4.2rc1/ext/periodic_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/pipe_event_data.cpp` & `pytango-9.4.2rc1/ext/pipe_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/pipe_info.cpp` & `pytango-9.4.2rc1/ext/pipe_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/poll_device.cpp` & `pytango-9.4.2rc1/ext/poll_device.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/precompiled_header.cpp` & `pytango-9.4.2rc1/ext/precompiled_header.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/precompiled_header.hpp` & `pytango-9.4.2rc1/ext/precompiled_header.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/pytango.cpp` & `pytango-9.4.2rc1/ext/pytango.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/pytgutils.cpp` & `pytango-9.4.2rc1/ext/pytgutils.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/pytgutils.h` & `pytango-9.4.2rc1/ext/pytgutils.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/pyutils.cpp` & `pytango-9.4.2rc1/ext/pyutils.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -51,66 +51,126 @@
     else
     {
         return PyUnicode_Decode(in, size, encoding, errors);
     }
 
 }
 
-void from_str_to_char(const bopy::object& in, std::string& out)
+void throw_bad_type(const char *type, const char *source)
 {
-    from_str_to_char(in.ptr(), out);
+    TangoSys_OMemStream description;
+    description << "Incompatible argument type, expected type is : Tango::" << type << std::ends;
+
+    TangoSys_OMemStream origin;
+    origin << source << std::ends;
+
+    Tango::Except::throw_exception("API_IncompatibleCmdArgumentType", description.str(),origin.str());
 }
 
-void from_str_to_char(PyObject* in, std::string& out)
+char* __copy_bytes_to_char(PyObject* in, Py_ssize_t* size)
 {
-    if (PyUnicode_Check(in))
-    {
-        PyObject *bytes_in = PyUnicode_AsLatin1String(in);
-        out = std::string(PyBytes_AsString(bytes_in), PyBytes_Size(bytes_in));
-        Py_DECREF(bytes_in);
-    }
-    else
+    Py_buffer view;
+
+    if (PyObject_GetBuffer(in, &view, PyBUF_FULL_RO) < 0)
     {
-        out = std::string(PyBytes_AsString(in), PyBytes_Size(in));
+        raise_(PyExc_TypeError, "Can't translate python object to C char* - PyObject_GetBuffer failed");
     }
+
+    *size = view.len;
+    char* out = new char[*size+1];
+    out[*size] = '\0';
+    memcpy(out, (char*)view.buf, *size);
+
+    PyBuffer_Release(&view);
+
+    return out;
 }
 
 char* from_str_to_char(const bopy::object& in)
 {
-    return from_str_to_char(in.ptr());
+    Py_ssize_t size;
+    return from_str_to_char(in.ptr(), &size);
+}
+
+char* from_str_to_char(PyObject* in)
+{
+    Py_ssize_t size;
+    return from_str_to_char(in, &size);
+}
+
+char* from_str_to_char(const bopy::object& in, Py_ssize_t* size_out, const bool utf_encoding)
+{
+    return from_str_to_char(in.ptr(), size_out, utf_encoding);
 }
 
 // The result is a newly allocated buffer. It is the responsibility
 // of the caller to manage the memory returned by this function
-char* from_str_to_char(PyObject* in)
+char* from_str_to_char(PyObject* in, Py_ssize_t* size_out, const bool utf_encoding)
 {
     char* out = NULL;
     if (PyUnicode_Check(in))
     {
-        PyObject *bytes_in = PyUnicode_AsLatin1String(in);
-	Py_ssize_t size = PyBytes_Size(bytes_in);
-	out = new char[size+1];
-	out[size] = '\0';
-	out = strncpy(out, PyBytes_AsString(bytes_in), size);
+        PyObject *bytes_in;
+        if (utf_encoding)
+        {
+            bytes_in = PyUnicode_AsUTF8String(in);
+        }
+        else
+        {
+            bytes_in = EncodeAsLatin1(in);
+        }
+        out = __copy_bytes_to_char(bytes_in, size_out);
         Py_DECREF(bytes_in);
+
     }
-    else if (PyBytes_Check(in))
+    else if (PyBytes_Check(in) || PyByteArray_Check(in))
     {
-	Py_ssize_t size = PyBytes_Size(in);
-	out = new char[size+1];
-	out[size] = '\0';
-	out = strncpy(out, PyBytes_AsString(in), size);
+        out = __copy_bytes_to_char(in, size_out);
     }
     else
     {
         raise_(PyExc_TypeError, "can't translate python object to C char*");
     }
     return out;
 }
 
+// The out_array will be updated with a pointer to existing memory (e.g., Python's internal memory for
+// a byte array). The caller gets a "view" of the memory and must not modify the memory.
+void view_pybytes_as_char_array(const bopy::object& py_value, Tango::DevVarCharArray& out_array)
+{
+    CORBA::ULong nb;
+    PyObject* data_ptr = py_value.ptr();
+
+    if (PyUnicode_Check(data_ptr))
+    {
+        Py_ssize_t size;
+        CORBA::Octet* encoded_data = (CORBA::Octet*)PyUnicode_AsUTF8AndSize(data_ptr, &size);
+        nb = static_cast<CORBA::ULong>(size);
+        out_array.replace(nb, nb, encoded_data, false);
+    }
+
+    else if (PyBytes_Check(data_ptr))
+    {
+        nb = static_cast<CORBA::ULong>(boost::python::len(py_value));
+        CORBA::Octet* encoded_data = (CORBA::Octet*)PyBytes_AsString(data_ptr);
+        out_array.replace(nb, nb, encoded_data, false);
+    }
+    else if (PyByteArray_Check(data_ptr))
+    {
+        nb = static_cast<CORBA::ULong>(boost::python::len(py_value));
+        CORBA::Octet* encoded_data = (CORBA::Octet*)PyByteArray_AsString(data_ptr);
+        out_array.replace(nb, nb, encoded_data, false);
+    }
+    else
+    {
+        throw_bad_type(Tango::CmdArgTypeName[Tango::DEV_ENCODED], TANGO_EXCEPTION_ORIGIN);
+    }
+}
+
+
 bool is_method_defined(object &obj, const std::string &method_name)
 {
     return is_method_defined(obj.ptr(), method_name);
 }
 
 bool is_method_defined(PyObject *obj, const std::string &method_name)
 {
```

### Comparing `pytango-9.4.1rc1/ext/pyutils.h` & `pytango-9.4.2rc1/ext/pyutils.h`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,42 @@
 #include <tango/tango.h>
 #include <omnithread.h>
 
 namespace bopy = boost::python;
 
 #define arg_(a) boost::python::arg(a)
 
+inline void raise_(PyObject *type, const char *message)
+{
+    PyErr_SetString(type, message);
+    boost::python::throw_error_already_set();
+}
+
+inline PyObject* EncodeAsLatin1(PyObject *in)
+{
+    PyObject* bytes_out = PyUnicode_AsLatin1String(in);
+    if (!bytes_out)
+    {
+        PyObject* bytes_replaced = PyUnicode_AsEncodedString(in, "latin-1", "replace");
+        const char* string_replaced = PyBytes_AsString(bytes_replaced);
+        std::string err_msg = "Can't encode ";
+        if (!string_replaced) {
+            err_msg += "unknown Unicode string as Latin-1";
+        } else {
+            err_msg += "'";
+            err_msg += string_replaced;
+            err_msg += "' Unicode string as Latin-1 (bad chars replaced with ?)";
+        }
+        Py_XDECREF(bytes_replaced);
+        raise_(PyExc_UnicodeError, err_msg.c_str());
+    }
+
+    return bytes_out;
+}
+
 
 inline PyObject *PyObject_GetAttrString_(PyObject *o, const std::string &attr_name)
 {
     const char *attr = attr_name.c_str();
     return PyObject_GetAttrString(o, attr);
 }
 
@@ -49,24 +77,26 @@
                                     const char* errors="strict");
 
 bopy::object from_char_to_boost_str(const std::string& in,
                                     const char* encoding=NULL, /* defaults to latin-1 */
                                     const char* errors="strict");
 
 
-void from_str_to_char(const bopy::object& in, std::string& out);
-void from_str_to_char(PyObject* in, std::string& out);
+void throw_bad_type(const char *type, const char *source);
+
+char* from_str_to_char(PyObject* in,
+                       Py_ssize_t* size_out,
+                       const bool utf_encoding=false /* defaults to latin-1 */);
+char* from_str_to_char(const bopy::object& in,
+                       Py_ssize_t* size_out,
+                       const bool utf_encoding=false /* defaults to latin-1 */);
 char* from_str_to_char(PyObject* in);
 char* from_str_to_char(const bopy::object& in);
 
-inline void raise_(PyObject *type, const char *message)
-{
-    PyErr_SetString(type, message);
-    boost::python::throw_error_already_set();
-}
+void view_pybytes_as_char_array(const bopy::object& py_value, Tango::DevVarCharArray& out_array);
 
 /// You should run any I/O intensive operations (like requesting data through
 /// the network) in the context of an object like this.
 class AutoPythonAllowThreads
 {
     PyThreadState *m_save;
```

### Comparing `pytango-9.4.1rc1/ext/server/attr.cpp` & `pytango-9.4.2rc1/ext/server/attr.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/attr.h` & `pytango-9.4.2rc1/ext/server/attr.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/attribute.cpp` & `pytango-9.4.2rc1/ext/server/attribute.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -86,65 +86,44 @@
         att.set_value(cpp_val.release(), 1, 0, true);
     }
 
     /**
      * Tango Attribute set_value wrapper for DevEncoded attributes
      *
      * @param att attribute reference
-     * @param data_str new attribute data string
-     * @param data new attribute data
+     * @param encoding_str new attribute encoding info
+     * @param data_str new attribute data
      */
     inline void __set_value(Tango::Attribute &att,
-                            bopy::str &data_str,
-                            bopy::str &data)
+                            bopy::str &encoding_str,
+                            bopy::str &data_str)
     {
-        extract<Tango::DevString> val_str(data_str.ptr());
-        if (!val_str.check())
-        {
-            throw_wrong_python_data_type(att.get_name(), "set_value()");
-        }
-        extract<Tango::DevString> val(data.ptr());
-        if (!val.check())
-        {
-            throw_wrong_python_data_type(att.get_name(), "set_value()");
-        }
+        Tango::DevString encoding_char = from_str_to_char(encoding_str);
+        Py_ssize_t size;
+        Tango::DevString data_char = from_str_to_char(data_str, &size, true);
 
-        Tango::DevString val_str_real = val_str;
-        Tango::DevString val_real = val;
-        att.set_value(&val_str_real, (Tango::DevUChar*)val_real, (long)len(data));
+        att.set_value(&encoding_char, (Tango::DevUChar*)data_char, (long)size, true);
     }
 
     /**
      * Tango Attribute set_value wrapper for DevEncoded attributes
      *
      * @param att attribute reference
      * @param data_str new attribute data string
      * @param data new attribute data
      */
     inline void __set_value(Tango::Attribute &att,
-                            bopy::str &data_str,
-                            bopy::object &data)
+                            bopy::str &encoding_str,
+                            bopy::object &data_obj)
     {
-        extract<Tango::DevString> val_str(data_str.ptr());
-        if (!val_str.check())
-        {
-            throw_wrong_python_data_type(att.get_name(), "set_value()");
-        }
-
-        PyObject* data_ptr = data.ptr();
-        Py_buffer view;
+        Tango::DevString encoding_char = from_str_to_char(encoding_str);
+        Py_ssize_t size;
+        Tango::DevString data_char = from_str_to_char(data_obj, &size, true);
 
-        if (PyObject_GetBuffer(data_ptr, &view, PyBUF_FULL_RO) < 0)
-        {
-            throw_wrong_python_data_type(att.get_name(), "set_value()");
-        }
-
-        Tango::DevString val_str_real = val_str;
-            att.set_value(&val_str_real, (Tango::DevUChar*)view.buf, (long)view.len);
-        PyBuffer_Release(&view);
+        att.set_value(&encoding_char, (Tango::DevUChar*)data_char, (long)size, true);
     }
 
     /**
      * Tango Attribute set_value_date_quality wrapper for scalar attributes
      *
      * @param att attribute reference
      * @param value new attribute value
@@ -174,76 +153,57 @@
         att.set_value_date_quality(cpp_val.release(), tv, quality, 1, 0, true);
     }
 
     /**
      * Tango Attribute set_value_date_quality wrapper for DevEncoded attributes
      *
      * @param att attribute reference
-     * @param data_str new attribute data string
-     * @param data new attribute data
+     * @param encoding_str new attribute data string
+     * @param data_str new attribute data
      * @param t timestamp
      * @param quality attribute quality
      */
     inline void __set_value_date_quality(Tango::Attribute &att,
+                                         bopy::str &encoding_str,
                                          bopy::str &data_str,
-                                         bopy::str &data,
                                          double t, Tango::AttrQuality quality)
     {
-        extract<Tango::DevString> val_str(data_str.ptr());
-        if (!val_str.check())
-        {
-            throw_wrong_python_data_type(att.get_name(), "set_value1()");
-        }
-        extract<Tango::DevString> val(data.ptr());
-        if (!val.check())
-        {
-            throw_wrong_python_data_type(att.get_name(), "set_value2()");
-        }
+        Tango::DevString encoding_char = from_str_to_char(encoding_str);
+        Py_ssize_t size;
+        Tango::DevString data_char = from_str_to_char(data_str, &size, true);
 
         PYTG_NEW_TIME_FROM_DOUBLE(t, tv);
-        Tango::DevString val_str_real = val_str;
-        Tango::DevString val_real = val;
-        att.set_value_date_quality(&val_str_real, (Tango::DevUChar*)val_real,
-                                   (long)len(data), tv, quality);
+
+        att.set_value_date_quality(&encoding_char, (Tango::DevUChar*)data_char,
+                                   (long)size, tv, quality, true);
     }
 
     /**
      * Tango Attribute set_value_date_quality wrapper for DevEncoded attributes
      *
      * @param att attribute reference
-     * @param data_str new attribute data string
-     * @param data new attribute data
+     * @param encoding_str new attribute data string
+     * @param data_obj new attribute data
      * @param t timestamp
      * @param quality attribute quality
      */
     inline void __set_value_date_quality(Tango::Attribute &att,
-                                         bopy::str &data_str,
-                                         bopy::object &data,
+                                         bopy::str &encoding_str,
+                                         bopy::object &data_obj,
                                          double t, Tango::AttrQuality quality)
     {
-        extract<Tango::DevString> val_str(data_str.ptr());
-        if (!val_str.check())
-        {
-            throw_wrong_python_data_type(att.get_name(), "set_value1()");
-        }
-
-	PyObject* data_ptr = data.ptr();
-	Py_buffer view;
-	
-	if (PyObject_GetBuffer(data_ptr, &view, PyBUF_FULL_RO) < 0)
-	{
-	    throw_wrong_python_data_type(att.get_name(), "set_value()");
-	}
+        Tango::DevString encoding_char = from_str_to_char(encoding_str);
+        Py_ssize_t size;
+        Tango::DevString data_char = from_str_to_char(data_obj, &size, true);
 
         PYTG_NEW_TIME_FROM_DOUBLE(t, tv);
-	Tango::DevString val_str_real = val_str;
-        att.set_value_date_quality(&val_str_real, (Tango::DevUChar*)view.buf,
-                                   (long)view.len, tv, quality);
-	PyBuffer_Release(&view);
-    }
+
+        att.set_value_date_quality(&encoding_char, (Tango::DevUChar*)data_char,
+                                   (long)size, tv, quality, true);
+        }
 
     template<long tangoTypeConst>
     void __set_value_date_quality_array(
             Tango::Attribute& att,
             bopy::object &value,
             double time,
             Tango::AttrQuality* quality,
```

### Comparing `pytango-9.4.1rc1/ext/server/attribute.h` & `pytango-9.4.2rc1/ext/server/attribute.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/auto_monitor.cpp` & `pytango-9.4.2rc1/ext/server/auto_monitor.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/command.cpp` & `pytango-9.4.2rc1/ext/server/command.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -72,42 +72,30 @@
         Tango::Except::throw_exception(
             "API_MemoryAllocation",
             "Can't allocate memory in server",
             "PyCmd::allocate_any()");
     }
 }
 
-void throw_bad_type(const char *type)
-{
-    TangoSys_OMemStream o;
-
-    o << "Incompatible command argument type, expected type is : Tango::" 
-      << type << std::ends;
-    Tango::Except::throw_exception(
-            "API_IncompatibleCmdArgumentType",
-            o.str(),
-            "PyCmd::extract()");
-}
-
 template<long tangoTypeConst>
 void insert_scalar(boost::python::object &o, CORBA::Any &any)
 {
     typedef typename TANGO_const2type(tangoTypeConst) TangoScalarType;
     
     any <<= extract<TangoScalarType>(o);
 }
 
 template<>
 void insert_scalar<Tango::DEV_STRING>(boost::python::object &o, CORBA::Any &any)
 {
     PyObject *o_ptr = o.ptr();
     if (PyUnicode_Check(o_ptr))
     {
-        PyObject *bytes_o_ptr = PyUnicode_AsLatin1String(o_ptr);
-	any <<= PyBytes_AsString(bytes_o_ptr);
+        PyObject *bytes_o_ptr = EncodeAsLatin1(o_ptr);
+        any <<= PyBytes_AsString(bytes_o_ptr);
         Py_DECREF(bytes_o_ptr);
     }
     else if (PyBytes_Check(o_ptr))
     {
         any <<= PyBytes_AsString(o_ptr);
     }
     else
@@ -128,36 +116,23 @@
 
     any <<= any_value;
 }
 
 template<>
 void insert_scalar<Tango::DEV_ENCODED>(boost::python::object &o, CORBA::Any &any)
 {
-    bopy::object p0 = o[0];
-    bopy::object p1 = o[1];
+    Tango::DevEncoded data;
 
+    bopy::object p0 = o[0];
     const char* encoded_format = bopy::extract<const char *> (p0.ptr());
-    
-    PyObject* data_ptr = p1.ptr();
-    Py_buffer view;
-    
-    if (PyObject_GetBuffer(data_ptr, &view, PyBUF_FULL_RO) < 0)
-    {
-        throw_bad_type(Tango::CmdArgTypeName[Tango::DEV_ENCODED]);
-    }
-    
-    CORBA::ULong nb = static_cast<CORBA::ULong>(view.len);
-    Tango::DevVarCharArray arr(nb, nb, (CORBA::Octet*)view.buf, false);
-    Tango::DevEncoded *data = new Tango::DevEncoded;
-    data->encoded_format = CORBA::string_dup(encoded_format);
-    data->encoded_data = arr;    
-    
-    any <<= data;
+    data.encoded_format = CORBA::string_dup(encoded_format);
+    view_pybytes_as_char_array(o[1], data.encoded_data);
 
-    PyBuffer_Release(&view);
+    // By giving a value (not a pointer) to <<= the data will be copied by CORBA
+    any <<= data;
 }
 
 template<>
 void insert_scalar<Tango::DEV_PIPE_BLOB>(boost::python::object &o, CORBA::Any &any)
 {
     assert(false);
 }
@@ -185,26 +160,26 @@
 void extract_scalar(const CORBA::Any &any, boost::python::object &o)
 {
     typedef typename TANGO_const2type(tangoTypeConst) TangoScalarType;
     
     TangoScalarType data;
     
     if ((any >>= data) == false)
-        throw_bad_type(Tango::CmdArgTypeName[tangoTypeConst]);
+        throw_bad_type(Tango::CmdArgTypeName[tangoTypeConst], TANGO_EXCEPTION_ORIGIN);
 
     o = object(data);
 }
 
 template<>
 void extract_scalar<Tango::DEV_STRING>(const CORBA::Any &any, boost::python::object &o)
 {
     Tango::ConstDevString data;
     
     if ((any >>= data) == false)
-        throw_bad_type(Tango::CmdArgTypeName[Tango::DEV_STRING]);
+        throw_bad_type(Tango::CmdArgTypeName[Tango::DEV_STRING], TANGO_EXCEPTION_ORIGIN);
 
     o = from_char_to_boost_str(data);
 }
 
 template<>
 void extract_scalar<Tango::DEV_VOID>(const CORBA::Any &any, boost::python::object &o)
 {}
@@ -217,15 +192,15 @@
 
 template<>
 void extract_scalar<Tango::DEV_ENCODED>(const CORBA::Any &any, boost::python::object &o)
 {
     Tango::DevEncoded* data;
 
     if ((any >>= data) == false)
-        throw_bad_type(Tango::CmdArgTypeName[Tango::DEV_ENCODED]);
+        throw_bad_type(Tango::CmdArgTypeName[Tango::DEV_ENCODED], TANGO_EXCEPTION_ORIGIN);
 
     boost::python::str encoded_format(data[0].encoded_format);
     boost::python::object encoded_data(
         boost::python::handle<>(
             PyBytes_FromStringAndSize(
                 (const char*)data[0].encoded_data.get_buffer(),
                 data[0].encoded_data.length()
@@ -266,15 +241,15 @@
 void extract_array(const CORBA::Any &any, boost::python::object &py_result)
 {
     typedef typename TANGO_const2type(tangoArrayTypeConst) TangoArrayType;
     
     TangoArrayType *tmp_ptr;
 
     if ((any >>= tmp_ptr) == false)
-        throw_bad_type(Tango::CmdArgTypeName[tangoArrayTypeConst]);
+        throw_bad_type(Tango::CmdArgTypeName[tangoArrayTypeConst], TANGO_EXCEPTION_ORIGIN);
 
       // For numpy we need a 'guard' object that handles the memory used
       // by the numpy object (releases it).
       // But I cannot manage memory inside our 'any' object, because it is
       // const and handles it's memory itself. So I need a copy before
       // creating the object.
       TangoArrayType* copy_ptr = new TangoArrayType(*tmp_ptr);
```

### Comparing `pytango-9.4.1rc1/ext/server/command.h` & `pytango-9.4.2rc1/ext/server/command.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/device_class.cpp` & `pytango-9.4.2rc1/ext/server/device_class.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/device_class.h` & `pytango-9.4.2rc1/ext/server/device_class.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/device_impl.cpp` & `pytango-9.4.2rc1/ext/server/device_impl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,15 @@
     }                                                                         \
     __AUX_CATCH_PY_EXCEPTION \
     __AUX_CATCH_EXCEPTION(name)
 
 // we don't use extract<> from boost bellow to get attribute name because it is
 // considerably slow
 #define SAFE_PUSH(dev, attr, attr_name) \
-    std::string __att_name; \
-    from_str_to_char(attr_name.ptr(), __att_name); \
+    std::string __att_name = from_str_to_char(attr_name.ptr()); \
     AutoPythonAllowThreads python_guard_ptr; \
     Tango::AutoTangoMonitor tango_guard(&dev); \
     Tango::Attribute & attr = dev.get_device_attr()->get_attr_by_name(__att_name.c_str()); \
     (void)attr; \
     python_guard_ptr.giveup();
 
 #define SAFE_PUSH_CHANGE_EVENT(dev, attr_name, data) \
@@ -532,16 +531,15 @@
     }
 
     /* **********************************
      * pipe event
      * **********************************/
     inline void push_pipe_event(Tango::DeviceImpl &self, str &pipe_name, object& pipe_data)
     {
-    	std::string __pipe_name;
-    	from_str_to_char(pipe_name.ptr(), __pipe_name);
+        std::string __pipe_name = from_str_to_char(pipe_name.ptr());
     	boost::python::extract<Tango::DevFailed> except_convert(pipe_data);
     	if (except_convert.check()) {
     		self.push_pipe_event(__pipe_name, const_cast<Tango::DevFailed*>(&except_convert()));
     		return;
     	}
     	Tango::DevicePipeBlob dpb;
     	bool reuse = false;
@@ -1009,14 +1007,24 @@
     }
     catch(boost::python::error_already_set &eas)
     {
         handle_python_exception(eas);
     }
 }
 
+void Device_3ImplWrap::server_init_hook()
+{
+    CALL_DEVICE_METHOD(Device_3Impl, server_init_hook)
+}
+
+void Device_3ImplWrap::default_server_init_hook()
+{
+    this->Tango::Device_3Impl::server_init_hook();
+}
+
 void Device_3ImplWrap::delete_device()
 {
     CALL_DEVICE_METHOD(Device_3Impl, delete_device)
 }
 
 void Device_3ImplWrap::default_delete_device()
 {
@@ -1184,14 +1192,24 @@
     }
     catch(boost::python::error_already_set &eas)
     {
         handle_python_exception(eas);
     }
 }
 
+void Device_4ImplWrap::server_init_hook()
+{
+    CALL_DEVICE_METHOD(Device_4Impl, server_init_hook)
+}
+
+void Device_4ImplWrap::default_server_init_hook()
+{
+    this->Tango::Device_4Impl::server_init_hook();
+}
+
 void Device_4ImplWrap::delete_device()
 {
     CALL_DEVICE_METHOD(Device_4Impl, delete_device)
 }
 
 void Device_4ImplWrap::default_delete_device()
 {
@@ -1352,14 +1370,24 @@
     }
     catch(boost::python::error_already_set &eas)
     {
         handle_python_exception(eas);
     }
 }
 
+void Device_5ImplWrap::server_init_hook()
+{
+    CALL_DEVICE_METHOD(Device_5Impl, server_init_hook)
+}
+
+void Device_5ImplWrap::default_server_init_hook()
+{
+    this->Tango::Device_5Impl::server_init_hook();
+}
+
 void Device_5ImplWrap::delete_device()
 {
     CALL_DEVICE_METHOD(Device_5Impl, delete_device)
 }
 
 void Device_5ImplWrap::default_delete_device()
 {
@@ -1761,14 +1789,16 @@
     class_<Tango::Device_3Impl, Device_3ImplWrap,
            bases<Tango::Device_2Impl>,
            boost::noncopyable>
            ("Device_3Impl",
             init<CppDeviceClass *, const char *,
                  boost::python::optional<const char *, Tango::DevState, const char *> >())
         .def("init_device", pure_virtual(&Tango::Device_3Impl::init_device))
+        .def("server_init_hook", &Tango::Device_3Impl::server_init_hook,
+             &Device_3ImplWrap::default_server_init_hook)
         .def("delete_device", &Tango::Device_3Impl::delete_device,
             &Device_3ImplWrap::default_delete_device)
         .def("always_executed_hook", &Tango::Device_3Impl::always_executed_hook,
             &Device_3ImplWrap::default_always_executed_hook)
         .def("read_attr_hardware", &Tango::Device_3Impl::read_attr_hardware,
             &Device_3ImplWrap::default_read_attr_hardware)
         .def("write_attr_hardware", &Tango::Device_3Impl::write_attr_hardware,
@@ -1786,14 +1816,16 @@
     class_<Tango::Device_4Impl, std::auto_ptr<Device_4ImplWrap>,
            bases<Tango::Device_3Impl>,
            boost::noncopyable>
            ("Device_4Impl",
             init<CppDeviceClass *, const char *,
                  boost::python::optional<const char *, Tango::DevState, const char *> >())
         .def("init_device", pure_virtual(&Tango::Device_4Impl::init_device))
+        .def("server_init_hook", &Tango::Device_4Impl::server_init_hook,
+             &Device_4ImplWrap::default_server_init_hook)
         .def("delete_device", &Tango::Device_4Impl::delete_device,
             &Device_4ImplWrap::default_delete_device)
         .def("always_executed_hook", &Tango::Device_4Impl::always_executed_hook,
             &Device_4ImplWrap::default_always_executed_hook)
         .def("read_attr_hardware", &Tango::Device_4Impl::read_attr_hardware,
             &Device_4ImplWrap::default_read_attr_hardware)
         .def("write_attr_hardware", &Tango::Device_4Impl::write_attr_hardware,
@@ -1810,14 +1842,16 @@
     class_<Tango::Device_5Impl, std::auto_ptr<Device_5ImplWrap>,
            bases<Tango::Device_4Impl>,
            boost::noncopyable>
            ("Device_5Impl",
             init<CppDeviceClass *, const char *,
                  boost::python::optional<const char *, Tango::DevState, const char *> >())
         .def("init_device", pure_virtual(&Tango::Device_5Impl::init_device))
+        .def("server_init_hook", &Tango::Device_5Impl::server_init_hook,
+             &Device_5ImplWrap::default_server_init_hook)
         .def("delete_device", &Tango::Device_5Impl::delete_device,
             &Device_5ImplWrap::default_delete_device)
         .def("always_executed_hook", &Tango::Device_5Impl::always_executed_hook,
             &Device_5ImplWrap::default_always_executed_hook)
         .def("read_attr_hardware", &Tango::Device_5Impl::read_attr_hardware,
             &Device_5ImplWrap::default_read_attr_hardware)
         .def("write_attr_hardware", &Tango::Device_5Impl::write_attr_hardware,
```

### Comparing `pytango-9.4.1rc1/ext/server/device_impl.h` & `pytango-9.4.2rc1/ext/server/device_impl.h`

 * *Files 9% similar despite different names*

```diff
@@ -172,14 +172,24 @@
     
     /**
      * Necessary init_device implementation to call python
      */
     virtual void init_device();
 
     /**
+     * Necessary server_init_hook implementation to call python
+     */
+    virtual void server_init_hook();
+
+    /**
+     * Executes default server_init_hook implementation
+     */
+    void default_server_init_hook();
+
+    /**
      * Necessary delete_device implementation to call python
      */
     virtual void delete_device();
 
     /**
      * Executes default delete_device implementation
      */
@@ -299,14 +309,24 @@
 
     /**
      * Necessary init_device implementation to call python
      */
     virtual void init_device();
 
     /**
+     * Necessary server_init_hook implementation to call python
+     */
+    virtual void server_init_hook();
+
+    /**
+     * Executes default server_init_hook implementation
+     */
+    void default_server_init_hook();
+
+    /**
      * Necessary delete_device implementation to call python
      */
     virtual void delete_device();
 
     /**
      * Executes default delete_device implementation
      */
@@ -426,14 +446,24 @@
 
     /**
      * Necessary init_device implementation to call python
      */
     virtual void init_device();
 
     /**
+     * Necessary server_init_hook implementation to call python
+     */
+    virtual void server_init_hook();
+
+    /**
+     * Executes default server_init_hook implementation
+     */
+    void default_server_init_hook();
+
+    /**
      * Necessary delete_device implementation to call python
      */
     virtual void delete_device();
 
     /**
      * Executes default delete_device implementation
      */
```

### Comparing `pytango-9.4.1rc1/ext/server/dserver.cpp` & `pytango-9.4.2rc1/ext/server/dserver.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/encoded_attribute.cpp` & `pytango-9.4.2rc1/ext/server/encoded_attribute.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             self.encode_gray8(buffer, w, h);
             return;
         }
         // It must be a py sequence
         // we are sure that w and h are given by python (see encoded_attribute.py)
         const int length = w*h;
         unsigned char *raw_b = new unsigned char[length];
-        unique_pointer<unsigned char> b(raw_b);
+        unique_pointer<unsigned char[]> b(raw_b);
         buffer = raw_b;
         unsigned char *p = raw_b;
         int w_bytes = w;
         for (long y=0; y<h; ++y)
         {
             PyObject *row = PySequence_GetItem(py_value_ptr, y);
             if (!row) boost::python::throw_error_already_set();
@@ -183,15 +183,15 @@
             self.encode_jpeg_gray8(buffer, w, h, quality);
             return;
         }
         // It must be a py sequence
         // we are sure that w and h are given by python (see encoded_attribute.py)
         const int length = w*h;
         unsigned char *raw_b = new unsigned char[length];
-        unique_pointer<unsigned char> b(raw_b);
+        unique_pointer<unsigned char[]> b(raw_b);
         buffer = raw_b;
         unsigned char *p = raw_b;
         int w_bytes = w;
         for (long y=0; y<h; ++y)
         {
             PyObject *row = PySequence_GetItem(py_value_ptr, y);
             if (!row) boost::python::throw_error_already_set();
@@ -295,15 +295,15 @@
             self.encode_gray16(buffer, w, h);
             return;
         }
         // It must be a py sequence
         // we are sure that w and h are given by python (see encoded_attribute.py)
         const int length = w*h;
         unsigned short *raw_b = new unsigned short[length];
-        unique_pointer<unsigned short> b(raw_b);
+        unique_pointer<unsigned short[]> b(raw_b);
         buffer = raw_b;
         unsigned short *p = raw_b;
         int w_bytes = 2*w;
         for (long y=0; y<h; ++y)
         {
             PyObject *row = PySequence_GetItem(py_value_ptr, y);
             if (!row) boost::python::throw_error_already_set();
@@ -403,15 +403,15 @@
             self.encode_rgb24(buffer, w, h);
             return;
         }
         // It must be a py sequence
         // we are sure that w and h are given by python (see encoded_attribute.py)
         const int length = w*h;
         unsigned char *raw_b = new unsigned char[length];
-        unique_pointer<unsigned char> b(raw_b);
+        unique_pointer<unsigned char[]> b(raw_b);
         buffer = raw_b;
         unsigned char *p = raw_b;
         int w_bytes = 3*w;
         for (long y=0; y<h; ++y)
         {
             PyObject *row = PySequence_GetItem(py_value_ptr, y);
             if (!row) boost::python::throw_error_already_set();
@@ -515,15 +515,15 @@
             self.encode_jpeg_rgb24(buffer, w, h, quality);
             return;
         }
         // It must be a py sequence
         // we are sure that w and h are given by python (see encoded_attribute.py)
 		const int length = w*h;
         unsigned char *raw_b = new unsigned char[length];
-        unique_pointer<unsigned char> b(raw_b);
+        unique_pointer<unsigned char[]> b(raw_b);
 		buffer = raw_b;
         unsigned char *p = raw_b;
         int w_bytes = 3*w;
         for (long y=0; y<h; ++y)
         {
             PyObject *row = PySequence_GetItem(py_value_ptr, y);
             if (!row) boost::python::throw_error_already_set();
@@ -627,15 +627,15 @@
             self.encode_jpeg_rgb32(buffer, w, h, quality);
             return;
         }
         // It must be a py sequence
         // we are sure that w and h are given by python (see encoded_attribute.py)
 		const int length = w*h;
         unsigned char *raw_b = new unsigned char[length];
-        unique_pointer<unsigned char> b(raw_b);
+        unique_pointer<unsigned char[]> b(raw_b);
 		buffer = raw_b;
         unsigned char *p = raw_b;
         int w_bytes = 4*w;
         for (long y=0; y<h; ++y)
         {
             PyObject *row = PySequence_GetItem(py_value_ptr, y);
             if (!row) boost::python::throw_error_already_set();
```

### Comparing `pytango-9.4.1rc1/ext/server/fwdAttr.cpp` & `pytango-9.4.2rc1/ext/server/fwdAttr.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/log4tango.cpp` & `pytango-9.4.2rc1/ext/server/log4tango.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/multi_attribute.cpp` & `pytango-9.4.2rc1/ext/server/multi_attribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/multi_class_attribute.cpp` & `pytango-9.4.2rc1/ext/server/multi_class_attribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/pipe.cpp` & `pytango-9.4.2rc1/ext/server/pipe.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/pipe.h` & `pytango-9.4.2rc1/ext/server/pipe.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/subdev.cpp` & `pytango-9.4.2rc1/ext/server/subdev.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/tango_util.cpp` & `pytango-9.4.2rc1/ext/server/tango_util.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/user_default_attr_prop.cpp` & `pytango-9.4.2rc1/ext/server/user_default_attr_prop.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/user_default_pipe_prop.cpp` & `pytango-9.4.2rc1/ext/server/user_default_pipe_prop.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/wattribute.cpp` & `pytango-9.4.2rc1/ext/server/wattribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/server/wattribute_numpy.hpp` & `pytango-9.4.2rc1/ext/server/wattribute_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/tango_numpy.h` & `pytango-9.4.2rc1/ext/tango_numpy.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/tgutils.h` & `pytango-9.4.2rc1/ext/tgutils.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/time_val.cpp` & `pytango-9.4.2rc1/ext/time_val.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/to_py.cpp` & `pytango-9.4.2rc1/ext/to_py.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/to_py.h` & `pytango-9.4.2rc1/ext/to_py.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/to_py_numpy.hpp` & `pytango-9.4.2rc1/ext/to_py_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/ext/version.cpp` & `pytango-9.4.2rc1/ext/version.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/pyproject.toml` & `pytango-9.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/pytango.egg-info/PKG-INFO` & `pytango-9.4.2rc1/pytango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytango
-Version: 9.4.1rc1
+Version: 9.4.2rc1
 Summary: A python binding for the Tango control system
 Home-page: http://gitlab.com/tango-controls/pytango
+Download-URL: http://pypi.python.org/pypi/pytango
 Author: Tiago Coutinho
 Author-email: coutinho@esrf.fr
 License: LGPL
-Download-URL: http://pypi.python.org/pypi/pytango
 Keywords: Tango,CORBA,binding
 Platform: Linux
 Platform: Windows XP/Vista/7/8/10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides: tango
 Provides: PyTango
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: gevent
 License-File: LICENSE.txt
 
 PyTango
 =======
@@ -185,8 +185,7 @@
 .. _IPython: http://ipython.org
 
 .. _documentation: http://pytango.readthedocs.io/en/latest
 .. _Tango forums: http://tango-controls.org/community/forum
 .. _PR and bug reports: PyTango_
 .. _sources: PyTango_
 .. _How to Contribute: http://pytango.readthedocs.io/en/latest/how-to-contribute.html#how-to-contribute
-
```

### Comparing `pytango-9.4.1rc1/pytango.egg-info/SOURCES.txt` & `pytango-9.4.2rc1/pytango.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,81 +4,81 @@
 Makefile
 PyTango.py
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 winsetup.py
-/builds/tango-controls/pytango/ext/api_util.cpp
-/builds/tango-controls/pytango/ext/archive_event_info.cpp
-/builds/tango-controls/pytango/ext/attr_conf_event_data.cpp
-/builds/tango-controls/pytango/ext/attribute_alarm_info.cpp
-/builds/tango-controls/pytango/ext/attribute_dimension.cpp
-/builds/tango-controls/pytango/ext/attribute_event_info.cpp
-/builds/tango-controls/pytango/ext/attribute_info.cpp
-/builds/tango-controls/pytango/ext/attribute_info_ex.cpp
-/builds/tango-controls/pytango/ext/attribute_proxy.cpp
-/builds/tango-controls/pytango/ext/base_types.cpp
-/builds/tango-controls/pytango/ext/callback.cpp
-/builds/tango-controls/pytango/ext/change_event_info.cpp
-/builds/tango-controls/pytango/ext/command_info.cpp
-/builds/tango-controls/pytango/ext/connection.cpp
-/builds/tango-controls/pytango/ext/constants.cpp
-/builds/tango-controls/pytango/ext/data_ready_event_data.cpp
-/builds/tango-controls/pytango/ext/database.cpp
-/builds/tango-controls/pytango/ext/db.cpp
-/builds/tango-controls/pytango/ext/dev_command_info.cpp
-/builds/tango-controls/pytango/ext/dev_error.cpp
-/builds/tango-controls/pytango/ext/device_attribute.cpp
-/builds/tango-controls/pytango/ext/device_attribute_config.cpp
-/builds/tango-controls/pytango/ext/device_attribute_history.cpp
-/builds/tango-controls/pytango/ext/device_data.cpp
-/builds/tango-controls/pytango/ext/device_data_history.cpp
-/builds/tango-controls/pytango/ext/device_info.cpp
-/builds/tango-controls/pytango/ext/device_pipe.cpp
-/builds/tango-controls/pytango/ext/device_proxy.cpp
-/builds/tango-controls/pytango/ext/devintr_change_event_data.cpp
-/builds/tango-controls/pytango/ext/enums.cpp
-/builds/tango-controls/pytango/ext/event_data.cpp
-/builds/tango-controls/pytango/ext/exception.cpp
-/builds/tango-controls/pytango/ext/from_py.cpp
-/builds/tango-controls/pytango/ext/group.cpp
-/builds/tango-controls/pytango/ext/group_reply.cpp
-/builds/tango-controls/pytango/ext/group_reply_list.cpp
-/builds/tango-controls/pytango/ext/locker_info.cpp
-/builds/tango-controls/pytango/ext/locking_thread.cpp
-/builds/tango-controls/pytango/ext/periodic_event_info.cpp
-/builds/tango-controls/pytango/ext/pipe_event_data.cpp
-/builds/tango-controls/pytango/ext/pipe_info.cpp
-/builds/tango-controls/pytango/ext/poll_device.cpp
-/builds/tango-controls/pytango/ext/precompiled_header.cpp
-/builds/tango-controls/pytango/ext/pytango.cpp
-/builds/tango-controls/pytango/ext/pytgutils.cpp
-/builds/tango-controls/pytango/ext/pyutils.cpp
-/builds/tango-controls/pytango/ext/time_val.cpp
-/builds/tango-controls/pytango/ext/to_py.cpp
-/builds/tango-controls/pytango/ext/version.cpp
-/builds/tango-controls/pytango/ext/server/attr.cpp
-/builds/tango-controls/pytango/ext/server/attribute.cpp
-/builds/tango-controls/pytango/ext/server/auto_monitor.cpp
-/builds/tango-controls/pytango/ext/server/command.cpp
-/builds/tango-controls/pytango/ext/server/device_class.cpp
-/builds/tango-controls/pytango/ext/server/device_impl.cpp
-/builds/tango-controls/pytango/ext/server/dserver.cpp
-/builds/tango-controls/pytango/ext/server/encoded_attribute.cpp
-/builds/tango-controls/pytango/ext/server/fwdAttr.cpp
-/builds/tango-controls/pytango/ext/server/log4tango.cpp
-/builds/tango-controls/pytango/ext/server/multi_attribute.cpp
-/builds/tango-controls/pytango/ext/server/multi_class_attribute.cpp
-/builds/tango-controls/pytango/ext/server/pipe.cpp
-/builds/tango-controls/pytango/ext/server/subdev.cpp
-/builds/tango-controls/pytango/ext/server/tango_util.cpp
-/builds/tango-controls/pytango/ext/server/user_default_attr_prop.cpp
-/builds/tango-controls/pytango/ext/server/user_default_pipe_prop.cpp
-/builds/tango-controls/pytango/ext/server/wattribute.cpp
+/home/matveyev/pytango/ext/api_util.cpp
+/home/matveyev/pytango/ext/archive_event_info.cpp
+/home/matveyev/pytango/ext/attr_conf_event_data.cpp
+/home/matveyev/pytango/ext/attribute_alarm_info.cpp
+/home/matveyev/pytango/ext/attribute_dimension.cpp
+/home/matveyev/pytango/ext/attribute_event_info.cpp
+/home/matveyev/pytango/ext/attribute_info.cpp
+/home/matveyev/pytango/ext/attribute_info_ex.cpp
+/home/matveyev/pytango/ext/attribute_proxy.cpp
+/home/matveyev/pytango/ext/base_types.cpp
+/home/matveyev/pytango/ext/callback.cpp
+/home/matveyev/pytango/ext/change_event_info.cpp
+/home/matveyev/pytango/ext/command_info.cpp
+/home/matveyev/pytango/ext/connection.cpp
+/home/matveyev/pytango/ext/constants.cpp
+/home/matveyev/pytango/ext/data_ready_event_data.cpp
+/home/matveyev/pytango/ext/database.cpp
+/home/matveyev/pytango/ext/db.cpp
+/home/matveyev/pytango/ext/dev_command_info.cpp
+/home/matveyev/pytango/ext/dev_error.cpp
+/home/matveyev/pytango/ext/device_attribute.cpp
+/home/matveyev/pytango/ext/device_attribute_config.cpp
+/home/matveyev/pytango/ext/device_attribute_history.cpp
+/home/matveyev/pytango/ext/device_data.cpp
+/home/matveyev/pytango/ext/device_data_history.cpp
+/home/matveyev/pytango/ext/device_info.cpp
+/home/matveyev/pytango/ext/device_pipe.cpp
+/home/matveyev/pytango/ext/device_proxy.cpp
+/home/matveyev/pytango/ext/devintr_change_event_data.cpp
+/home/matveyev/pytango/ext/enums.cpp
+/home/matveyev/pytango/ext/event_data.cpp
+/home/matveyev/pytango/ext/exception.cpp
+/home/matveyev/pytango/ext/from_py.cpp
+/home/matveyev/pytango/ext/group.cpp
+/home/matveyev/pytango/ext/group_reply.cpp
+/home/matveyev/pytango/ext/group_reply_list.cpp
+/home/matveyev/pytango/ext/locker_info.cpp
+/home/matveyev/pytango/ext/locking_thread.cpp
+/home/matveyev/pytango/ext/periodic_event_info.cpp
+/home/matveyev/pytango/ext/pipe_event_data.cpp
+/home/matveyev/pytango/ext/pipe_info.cpp
+/home/matveyev/pytango/ext/poll_device.cpp
+/home/matveyev/pytango/ext/precompiled_header.cpp
+/home/matveyev/pytango/ext/pytango.cpp
+/home/matveyev/pytango/ext/pytgutils.cpp
+/home/matveyev/pytango/ext/pyutils.cpp
+/home/matveyev/pytango/ext/time_val.cpp
+/home/matveyev/pytango/ext/to_py.cpp
+/home/matveyev/pytango/ext/version.cpp
+/home/matveyev/pytango/ext/server/attr.cpp
+/home/matveyev/pytango/ext/server/attribute.cpp
+/home/matveyev/pytango/ext/server/auto_monitor.cpp
+/home/matveyev/pytango/ext/server/command.cpp
+/home/matveyev/pytango/ext/server/device_class.cpp
+/home/matveyev/pytango/ext/server/device_impl.cpp
+/home/matveyev/pytango/ext/server/dserver.cpp
+/home/matveyev/pytango/ext/server/encoded_attribute.cpp
+/home/matveyev/pytango/ext/server/fwdAttr.cpp
+/home/matveyev/pytango/ext/server/log4tango.cpp
+/home/matveyev/pytango/ext/server/multi_attribute.cpp
+/home/matveyev/pytango/ext/server/multi_class_attribute.cpp
+/home/matveyev/pytango/ext/server/pipe.cpp
+/home/matveyev/pytango/ext/server/subdev.cpp
+/home/matveyev/pytango/ext/server/tango_util.cpp
+/home/matveyev/pytango/ext/server/user_default_attr_prop.cpp
+/home/matveyev/pytango/ext/server/user_default_pipe_prop.cpp
+/home/matveyev/pytango/ext/server/wattribute.cpp
 cmake/project_version.cc.in
 cmake/project_version.cmake
 cmake/project_version.h.in
 doc/api.rst
 doc/conf.py
 doc/contents.rst
 doc/data_types.rst
@@ -96,14 +96,15 @@
 doc/news.rst
 doc/quicktour.rst
 doc/revision.rst
 doc/start.rst
 doc/tep.rst
 doc/testing.rst
 doc/utilities.rst
+doc/version-policy.rst
 doc/windows_notes.txt
 doc/.devcontainer/Dockerfile
 doc/.devcontainer/README.md
 doc/_static/arrow03.png
 doc/_static/banner1.png
 doc/_static/banner2.png
 doc/_static/banner3.png
@@ -178,14 +179,15 @@
 doc/server_api/logging.rst
 doc/server_api/server.rst
 doc/server_api/util.rst
 doc/tep/DataBase.xmi
 doc/tep/database.py
 doc/tep/tep-0001.rst
 doc/tep/tep-0002.rst
+doc/testing/coverage.rst
 doc/testing/mocks.rst
 doc/testing/test_context.rst
 doc/testing/testing_approaches.rst
 examples/Clock/Clock.py
 examples/Clock/ClockDS.py
 examples/Clock/client.py
 examples/TuringMachine/TuringMachine.py
@@ -294,17 +296,19 @@
 ext/database.cpp
 ext/db.cpp
 ext/defs.h
 ext/dev_command_info.cpp
 ext/dev_error.cpp
 ext/device_attribute.cpp
 ext/device_attribute.h
+ext/device_attribute.h.gch
 ext/device_attribute_config.cpp
 ext/device_attribute_history.cpp
 ext/device_attribute_numpy.hpp
+ext/device_attribute_numpy.hpp.gch
 ext/device_data.cpp
 ext/device_data_history.cpp
 ext/device_info.cpp
 ext/device_pipe.cpp
 ext/device_pipe.h
 ext/device_proxy.cpp
 ext/devintr_change_event_data.cpp
@@ -328,14 +332,15 @@
 ext/precompiled_header.cpp
 ext/precompiled_header.hpp
 ext/pytango.cpp
 ext/pytgutils.cpp
 ext/pytgutils.h
 ext/pyutils.cpp
 ext/pyutils.h
+ext/pyutils.h.gch
 ext/tango_numpy.h
 ext/tgutils.h
 ext/time_val.cpp
 ext/to_py.cpp
 ext/to_py.h
 ext/to_py_numpy.hpp
 ext/version.cpp
@@ -369,15 +374,14 @@
 pytango.egg-info/dependency_links.txt
 pytango.egg-info/requires.txt
 pytango.egg-info/top_level.txt
 tango/__init__.py
 tango/api_util.py
 tango/asyncio.py
 tango/asyncio_executor.py
-tango/asyncio_tools.py
 tango/attr_data.py
 tango/attribute_proxy.py
 tango/auto_monitor.py
 tango/base_types.py
 tango/callback.py
 tango/client.py
 tango/codec.py
@@ -420,12 +424,13 @@
 tango/databaseds/create_db_tables.sql
 tango/databaseds/database.py
 tango/databaseds/db_errors.py
 tango/databaseds/mysql2sqlite.sh
 tango/databaseds/db_access/__init__.py
 tango/databaseds/db_access/sqlite3.py
 tests/conftest.py
+tests/report.xml
 tests/test_async.py
 tests/test_client.py
 tests/test_event.py
 tests/test_server.py
 tests/test_test_context.py
```

### Comparing `pytango-9.4.1rc1/setup.py` & `pytango-9.4.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,15 @@
     ]
 
     provides = [
         "tango",
         "PyTango",  # Backward compatibilty
     ]
 
-    python_requires = ">=3.6"
+    python_requires = ">=3.9"
 
     install_requires = [
         "numpy (>=1.13.3)",
         "packaging",
         "psutil",
     ]
 
@@ -379,14 +379,15 @@
     if PYTHON_VERSION < (3, 7):
         tests_require += [
             "pytest < 7.1",
             "pytest-forked",
             "tomli < 2.0",
             "typing-extensions < 4.0",
             "iniconfig < 2.0",
+            "attrs < 23",
         ]
     else:
         tests_require += ["pytest", "pytest-forked"]
 
     extras_require = {"tests": tests_require, "gevent": ["gevent >= 20.0"]}
 
     package_data = {
```

### Comparing `pytango-9.4.1rc1/tango/__init__.py` & `pytango-9.4.2rc1/tango/__init__.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/api_util.py` & `pytango-9.4.2rc1/tango/api_util.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/asyncio.py` & `pytango-9.4.2rc1/tango/asyncio.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/asyncio_executor.py` & `pytango-9.4.2rc1/tango/futures_executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,65 @@
-# -----------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # This file is part of PyTango (http://pytango.rtfd.io)
 #
 # Copyright 2006-2012 CELLS / ALBA Synchrotron, Bellaterra, Spain
 # Copyright 2013-2014 European Synchrotron Radiation Facility, Grenoble, France
 #
 # Distributed under the terms of the GNU Lesser General Public License,
 # either version 3 of the License, or (at your option) any later version.
 # See LICENSE.txt for more info.
-# -----------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 
-# Imports
-import functools
-
-# Asyncio imports
-try:
-    import asyncio
-except ImportError:
-    import trollius as asyncio
-try:
-    from asyncio import run_coroutine_threadsafe
-except ImportError:
-    from .asyncio_tools import run_coroutine_threadsafe
-try:
-    from asyncio import coroutine
-except ImportError:
-    from .asyncio_tools import coroutine
+# Concurrent imports
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 # Tango imports
 from .green import AbstractExecutor
 
-__all__ = ("AsyncioExecutor", "get_global_executor", "set_global_executor")
-
+__all__ = ("FuturesExecutor", "get_global_executor", "set_global_executor")
 
 # Global executor
 
 _EXECUTOR = None
 
 
 def get_global_executor():
     global _EXECUTOR
     if _EXECUTOR is None:
-        _EXECUTOR = AsyncioExecutor()
+        _EXECUTOR = FuturesExecutor()
     return _EXECUTOR
 
 
 def set_global_executor(executor):
     global _EXECUTOR
     _EXECUTOR = executor
 
 
-# Asyncio executor
+# Futures executor
 
 
-class AsyncioExecutor(AbstractExecutor):
-    """Asyncio tango executor"""
+class FuturesExecutor(AbstractExecutor):
+    """Futures tango executor"""
 
     asynchronous = True
-    default_wait = False
+    default_wait = True
 
-    def __init__(self, loop=None, subexecutor=None):
+    def __init__(self, process=False, max_workers=20):
         super().__init__()
-        if loop is None:
-            try:
-                loop = asyncio.get_event_loop()
-            except RuntimeError:
-                loop = asyncio.new_event_loop()
-                asyncio.set_event_loop(loop)
-        self.loop = loop
-        self.subexecutor = subexecutor
+        cls = ProcessPoolExecutor if process else ThreadPoolExecutor
+        self.subexecutor = cls(max_workers=max_workers)
 
     def delegate(self, fn, *args, **kwargs):
-        """Return the given operation as an asyncio future."""
-        callback = functools.partial(fn, *args, **kwargs)
-        coro = self.loop.run_in_executor(self.subexecutor, callback)
-        return asyncio.ensure_future(coro)
+        """Return the given operation as a concurrent future."""
+        return self.subexecutor.submit(fn, *args, **kwargs)
 
     def access(self, accessor, timeout=None):
-        """Return a result from an asyncio future."""
-        if self.loop.is_running():
-            raise RuntimeError("Loop is already running")
-        coro = asyncio.wait_for(accessor, timeout)
-        return self.loop.run_until_complete(coro)
+        """Return a result from a single callable."""
+        return accessor.result(timeout=timeout)
 
     def submit(self, fn, *args, **kwargs):
         """Submit an operation"""
-        corofn = coroutine(lambda: fn(*args, **kwargs))
-        return run_coroutine_threadsafe(corofn(), self.loop)
+        return fn(*args, **kwargs)
 
     def execute(self, fn, *args, **kwargs):
         """Execute an operation and return the result."""
-        if self.in_executor_context():
-            corofn = coroutine(lambda: fn(*args, **kwargs))
-            return corofn()
-        future = self.submit(fn, *args, **kwargs)
-        return future.result()
+        return fn(*args, **kwargs)
```

### Comparing `pytango-9.4.1rc1/tango/attr_data.py` & `pytango-9.4.2rc1/tango/attr_data.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/attribute_proxy.py` & `pytango-9.4.2rc1/tango/attribute_proxy.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/auto_monitor.py` & `pytango-9.4.2rc1/tango/auto_monitor.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/base_types.py` & `pytango-9.4.2rc1/tango/base_types.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/callback.py` & `pytango-9.4.2rc1/tango/callback.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/client.py` & `pytango-9.4.2rc1/tango/client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/codec.py` & `pytango-9.4.2rc1/tango/codec.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/connection.py` & `pytango-9.4.2rc1/tango/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,42 +237,30 @@
 
 
 __Connection__command_inout_asynch.__name__ = "command_inout_asynch"
 
 
 def __Connection__command_inout_reply(self, idx, timeout=None):
     """
-    command_inout_reply(self, id) -> DeviceData
+    command_inout_reply(self, idx, timeout=None) -> DeviceData
 
             Check if the answer of an asynchronous command_inout is arrived
             (polling model). If the reply is arrived and if it is a valid
             reply, it is returned to the caller in a DeviceData object. If
-            the reply is an exception, it is re-thrown by this call. An
-            exception is also thrown in case of the reply is not yet arrived.
-
-        Parameters :
-            - id      : (int) Asynchronous call identifier.
-        Return     : (DeviceData)
-        Throws     : AsynCall, AsynReplyNotArrived, CommunicationFailed, DevFailed from device
-
-    command_inout_reply(self, id, timeout) -> DeviceData
-
-            Check if the answer of an asynchronous command_inout is arrived
-            (polling model). id is the asynchronous call identifier. If the
-            reply is arrived and if it is a valid reply, it is returned to
-            the caller in a DeviceData object. If the reply is an exception,
-            it is re-thrown by this call. If the reply is not yet arrived,
-            the call will wait (blocking the process) for the time specified
+            the reply is an exception, it is re-thrown by this call. If optional
+            `timeout` parameter is not provided an exception is also thrown in case
+            of the reply is not yet arrived. If `timeout` is provided, the call will
+            wait (blocking the process) for the time specified
             in timeout. If after timeout milliseconds, the reply is still
             not there, an exception is thrown. If timeout is set to 0, the
             call waits until the reply arrived.
 
         Parameters :
-            - id      : (int) Asynchronous call identifier.
-            - timeout : (int)
+            - idx      : (int) Asynchronous call identifier.
+            - timeout  : (int) (optional) Milliseconds to wait for the reply.
         Return     : (DeviceData)
         Throws     : AsynCall, AsynReplyNotArrived, CommunicationFailed, DevFailed from device
     """
     if timeout is None:
         r = self.command_inout_reply_raw(idx)
     else:
         r = self.command_inout_reply_raw(idx, timeout)
```

### Comparing `pytango-9.4.1rc1/tango/databaseds/DataBase.xmi` & `pytango-9.4.2rc1/tango/databaseds/DataBase.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/databaseds/create_db.sql` & `pytango-9.4.2rc1/tango/databaseds/create_db.sql`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/databaseds/create_db_tables.sql` & `pytango-9.4.2rc1/tango/databaseds/create_db_tables.sql`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/databaseds/database.py` & `pytango-9.4.2rc1/tango/databaseds/database.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/databaseds/db_access/sqlite3.py` & `pytango-9.4.2rc1/tango/databaseds/db_access/sqlite3.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/databaseds/mysql2sqlite.sh` & `pytango-9.4.2rc1/tango/databaseds/mysql2sqlite.sh`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/db.py` & `pytango-9.4.2rc1/tango/db.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/device_attribute.py` & `pytango-9.4.2rc1/tango/device_attribute.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/device_class.py` & `pytango-9.4.2rc1/tango/device_class.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/device_data.py` & `pytango-9.4.2rc1/tango/device_data.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/device_proxy.py` & `pytango-9.4.2rc1/tango/device_proxy.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/device_server.py` & `pytango-9.4.2rc1/tango/device_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,25 +87,47 @@
         # to avoid double wrapping we add an empty field, and then use it to check, whether function is already wrapped
         wrapper.wrapped_with_executor = True
         return wrapper
     else:
         return fn
 
 
-def get_source_location():
-    """Helper function that provides source location for logging functions."""
-    # Search the call stack until we are out of the 'tango' module. We cannot
-    # have a fixed number here beause loggers/streams are used in many places
-    # inside pytango with varying call stack depth.
-    for frame, filename, lineno, _, _, _ in inspect.stack():
-        module = frame.f_globals["__name__"]
-        if module != "tango" and not module.startswith("tango."):
-            filename = os.path.basename(filename)
-            return filename, lineno
-    return "(unknown)", 0
+def get_source_location(source=None):
+    """Helper function that provides source location for logging functions.
+    :param source:
+        (optional) Method or function, which will be unwrapped of decorated wrappers
+        and inspected for location. If not provided - current stack will be used to deduce the location.
+    :type source: Callable
+
+    :return:
+        Tuple (filename, lineno)
+    :rtype :tuple:
+    """
+    try:
+        if source:
+            # If source is a wrapped function - unwrap it to inner function
+            source = inspect.unwrap(source)
+            # Find callable code location
+            code = getattr(source, "__code__", None)
+            if code:
+                filename = os.path.basename(code.co_filename)
+                lineno = code.co_firstlineno
+                return filename, lineno
+        else:
+            # Search the call stack until we are out of the 'tango' module. We cannot
+            # have a fixed number here beause loggers/streams are used in many places
+            # inside pytango with varying call stack depth.
+            for frame, filename, lineno, _, _, _ in inspect.stack():
+                module = frame.f_globals["__name__"]
+                if module != "tango" and not module.startswith("tango."):
+                    filename = os.path.basename(filename)
+                    return filename, lineno
+        return "(unknown)", 0
+    except Exception:
+        return "(unknown)", 0
 
 
 # Note: the inheritance below doesn't call get_latest_device_class(),
 #       because such dynamic inheritance breaks auto-completion in IDEs.
 #       Instead, we manually provide the correct class here, and verify
 #       that the inheritance is correct via a unit test, in test_server.py.
 class LatestDeviceImpl(Device_5Impl):
@@ -704,15 +726,15 @@
 
     bound_method = types.MethodType(is_allowed_cmd, device)
     setattr(device, name, bound_method)
 
 
 def __DeviceImpl__remove_command(self, cmd_name, free_it=False, clean_db=True):
     """
-    remove_command(self, attr_name)
+    remove_command(self, cmd_name, free_it=False, clean_db=True)
 
         Remove one command from the device command list.
 
         :param cmd_name: command name to be removed from the list
         :type cmd_name: str
         :param free_it: set to true if the command object must be freed.
         :type free_it: bool
@@ -720,104 +742,144 @@
                          if the command is polled) from database.
 
         :raises DevFailed:
     """
     self._remove_command(cmd_name, free_it, clean_db)
 
 
-def __DeviceImpl__debug_stream(self, msg, *args):
+def __DeviceImpl__debug_stream(self, msg, *args, source=None):
     """
-    debug_stream(self, msg, *args)
+    debug_stream(self, msg, *args, source=None)
 
         Sends the given message to the tango debug stream.
 
         Since PyTango 7.1.3, the same can be achieved with::
 
             print(msg, file=self.log_debug)
 
         :param msg: the message to be sent to the debug stream
         :type msg: str
+
+        :param *args: Arguments to format a message string.
+
+        :param source: Function that will be inspected for filename and lineno in the log message.
+        :type source: Callable
+
+        .. versionadded:: 9.4.2
+            added *source* parameter
     """
-    filename, line = get_source_location()
+    filename, line = get_source_location(source)
     if args:
         msg = msg % args
     self.__debug_stream(filename, line, msg)
 
 
-def __DeviceImpl__info_stream(self, msg, *args):
+def __DeviceImpl__info_stream(self, msg, *args, source=None):
     """
-    info_stream(self, msg, *args)
+    info_stream(self, msg, *args, source=None)
 
         Sends the given message to the tango info stream.
 
         Since PyTango 7.1.3, the same can be achieved with::
 
             print(msg, file=self.log_info)
 
         :param msg: the message to be sent to the info stream
         :type msg: str
+
+        :param *args: Arguments to format a message string.
+
+        :param source: Function that will be inspected for filename and lineno in the log message.
+        :type source: Callable
+
+        .. versionadded:: 9.4.2
+            added *source* parameter
     """
-    filename, line = get_source_location()
+    filename, line = get_source_location(source)
     if args:
         msg = msg % args
     self.__info_stream(filename, line, msg)
 
 
-def __DeviceImpl__warn_stream(self, msg, *args):
+def __DeviceImpl__warn_stream(self, msg, *args, source=None):
     """
-    warn_stream(self, msg, *args)
+    warn_stream(self, msg, *args, source=None)
 
         Sends the given message to the tango warn stream.
 
         Since PyTango 7.1.3, the same can be achieved with::
 
             print(msg, file=self.log_warn)
 
         :param msg: the message to be sent to the warn stream
         :type msg: str
+
+        :param *args: Arguments to format a message string.
+
+        :param source: Function that will be inspected for filename and lineno in the log message.
+        :type source: Callable
+
+        .. versionadded:: 9.4.2
+            added *source* parameter
     """
-    filename, line = get_source_location()
+    filename, line = get_source_location(source)
     if args:
         msg = msg % args
     self.__warn_stream(filename, line, msg)
 
 
-def __DeviceImpl__error_stream(self, msg, *args):
+def __DeviceImpl__error_stream(self, msg, *args, source=None):
     """
-    error_stream(self, msg, *args)
+    error_stream(self, msg, *args, source=None)
 
         Sends the given message to the tango error stream.
 
         Since PyTango 7.1.3, the same can be achieved with::
 
             print(msg, file=self.log_error)
 
         :param msg: the message to be sent to the error stream
         :type msg: str
+
+        :param *args: Arguments to format a message string.
+
+        :param source: Function that will be inspected for filename and lineno in the log message.
+        :type source: Callable
+
+        .. versionadded:: 9.4.2
+            added *source* parameter
     """
-    filename, line = get_source_location()
+    filename, line = get_source_location(source)
     if args:
         msg = msg % args
     self.__error_stream(filename, line, msg)
 
 
-def __DeviceImpl__fatal_stream(self, msg, *args):
+def __DeviceImpl__fatal_stream(self, msg, *args, source=None):
     """
-    fatal_stream(self, msg, *args)
+    fatal_stream(self, msg, *args, source=None)
 
         Sends the given message to the tango fatal stream.
 
         Since PyTango 7.1.3, the same can be achieved with::
 
             print(msg, file=self.log_fatal)
 
         :param msg: the message to be sent to the fatal stream
         :type msg: str
+
+        :param *args: Arguments to format a message string.
+
+        :param source: Function that will be inspected for filename and lineno in the log message.
+        :type source: Callable
+
+        .. versionadded:: 9.4.2
+            added *source* parameter
     """
-    filename, line = get_source_location()
+    filename, line = get_source_location(source)
     if args:
         msg = msg % args
     self.__fatal_stream(filename, line, msg)
 
 
 @property
 def __DeviceImpl__debug(self):
@@ -1286,16 +1348,14 @@
                       push_change_event(self, attr_name, str_data, data)
                       push_change_event(self, attr_name, data, time_stamp, quality, dim_x = 1, dim_y = 0)
                       push_change_event(self, attr_name, str_data, data, time_stamp, quality)
             :noindex:
 
         Push a change event for the given attribute name.
 
-        The event is pushed to the notification daemon.
-
         :param attr_name: attribute name
         :type attr_name: str
         :param data: the data to be sent as attribute event data. Data must be compatible with the
                      attribute type and format.
                      for SPECTRUM and IMAGE attributes, data can be any type of sequence of elements
                      compatible with the attribute type
         :param str_data: special variation for DevEncoded data type. In this case 'data' must
@@ -1326,16 +1386,14 @@
                       push_archive_event(self, attr_name, str_data, data)
                       push_archive_event(self, attr_name, data, time_stamp, quality, dim_x = 1, dim_y = 0)
                       push_archive_event(self, attr_name, str_data, data, time_stamp, quality)
             :noindex:
 
         Push an archive event for the given attribute name.
 
-        The event is pushed to the notification daemon.
-
         :param attr_name: attribute name
         :type attr_name: str
         :param data: the data to be sent as attribute event data. Data must be compatible with the
                      attribute type and format.
                      for SPECTRUM and IMAGE attributes, data can be any type of sequence of elements
                      compatible with the attribute type
         :param str_data: special variation for DevEncoded data type. In this case 'data' must
@@ -1365,16 +1423,14 @@
                       push_event(self, attr_name, filt_names, filt_vals, str_data, data)
                       push_event(self, attr_name, filt_names, filt_vals, data, time_stamp, quality, dim_x = 1, dim_y = 0)
                       push_event(self, attr_name, filt_names, filt_vals, str_data, data, time_stamp, quality)
             :noindex:
 
         Push a user event for the given attribute name.
 
-        The event is pushed to the notification daemon.
-
         :param attr_name: attribute name
         :type attr_name: str
         :param filt_names: the filterable fields name
         :type filt_names: Sequence[str]
         :param filt_vals: the filterable fields value
         :type filt_vals: Sequence[double]
         :param data: the data to be sent as attribute event data. Data must be compatible with the
@@ -1411,22 +1467,20 @@
         :type implemented: bool
     """,
     )
 
     document_method(
         "push_data_ready_event",
         """
-    push_data_ready_event(self, attr_name, counter = 0)
+    push_data_ready_event(self, attr_name, counter)
 
         Push a data ready event for the given attribute name.
 
-        The event is pushed to the notification daemon.
-
-        The method needs only the attribue name and an optional
-        "counter" which will be passed unchanged within the event
+        The method needs the attribute name and a
+        "counter" which will be passed within the event
 
         :param attr_name: attribute name
         :type attr_name: str
         :param counter: the user counter
         :type counter: int
 
         :raises DevFailed: If the attribute name is unknown.
@@ -1968,14 +2022,31 @@
         in case of the default behaviour does not fullfill the needs
 
         :raises DevFailed: This method does not throw exception but a redefined method can.
     """,
     )
 
     document_method(
+        "server_init_hook",
+        """
+    server_init_hook(self)
+
+        Hook method.
+
+        This method is called once the device server admin device is exported.
+        This allows for instance for the different devices to subscribe 
+        to events at server startup on attributes from other devices 
+        of the same device server with stateless parameter set to false.
+        
+        This method can be redefined in sub-classes in case of the default 
+        behaviour does not fullfill the needs
+    """,
+    )
+
+    document_method(
         "read_attr_hardware",
         """
     read_attr_hardware(self, attr_list)
 
         Read the hardware to return attribute value(s).
 
         Default method to implement an action necessary on a device to read
```

### Comparing `pytango-9.4.1rc1/tango/encoded_attribute.py` & `pytango-9.4.2rc1/tango/encoded_attribute.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/exception.py` & `pytango-9.4.2rc1/tango/exception.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/futures.py` & `pytango-9.4.2rc1/tango/futures.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/gevent.py` & `pytango-9.4.2rc1/tango/gevent.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/gevent_executor.py` & `pytango-9.4.2rc1/tango/gevent_executor.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/globals.py` & `pytango-9.4.2rc1/tango/globals.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/green.py` & `pytango-9.4.2rc1/tango/green.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 # -----------------------------------------------------------------------------
 
 
 # Imports
 import os
 from functools import wraps
 
-# Compatibility imports
-try:
-    from threading import get_ident
-except Exception:
-    from threading import _get_ident as get_ident
+from threading import get_ident
 
 # Tango imports
 from ._tango import GreenMode
 
 __all__ = (
     "get_green_mode",
     "set_green_mode",
```

### Comparing `pytango-9.4.1rc1/tango/group.py` & `pytango-9.4.2rc1/tango/group.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/group_reply.py` & `pytango-9.4.2rc1/tango/group_reply.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/group_reply_list.py` & `pytango-9.4.2rc1/tango/group_reply_list.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/log4tango.py` & `pytango-9.4.2rc1/tango/log4tango.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,28 +130,28 @@
             log = self.get_log_func(dev)
             f_name = dev.__class__.__name__ + "." + f.__name__
             sargs = ""
             if self._show_args:
                 sargs = self.__compact_elems_str(args[1:])
             if self._show_kwargs:
                 sargs += self.__compact_dict_str(kwargs)
-            log(f"-> {f_name}({sargs})")
+            log(f"-> {f_name}({sargs})", source=f)
             with_exc = True
             try:
                 ret = f(*args, **kwargs)
                 with_exc = False
                 return ret
             finally:
                 if with_exc:
-                    log(f"<- {f_name}() raised exception!")
+                    log(f"<- {f_name}() raised exception!", source=f)
                 else:
                     sret = ""
                     if self._show_ret:
                         sret = self.__compact_elem(ret) + " "
-                    log(f"{sret}<- {f_name}()")
+                    log(f"{sret}<- {f_name}()", source=f)
 
         log_stream._wrapped = f
         return log_stream
 
 
 class DebugIt(LogIt):
     """A class designed to be a decorator of any method of a
```

### Comparing `pytango-9.4.1rc1/tango/pipe.py` & `pytango-9.4.2rc1/tango/pipe.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/pipe_data.py` & `pytango-9.4.2rc1/tango/pipe_data.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/pytango_init.py` & `pytango-9.4.2rc1/tango/pytango_init.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/pytango_pprint.py` & `pytango-9.4.2rc1/tango/pytango_pprint.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/pyutil.py` & `pytango-9.4.2rc1/tango/pyutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1168,15 +1168,15 @@
 
 def __doc_EnsureOmniThread():
     EnsureOmniThread.__doc__ = """\
 
     Tango servers and clients that start their own additional threads
     that will interact with Tango must guard these threads within this
     Python context.  This is especially important when working with
-    event subscriptions.
+    event subscriptions, and pushing events.
     
     This context handler class ensures a non-omniORB thread will still
     get a dummy omniORB thread ID - cppTango requires threads to
     be identifiable in this way.  It should only be acquired once for
     the lifetime of the thread, and must be released before the thread
     is cleaned up.
         
@@ -1203,15 +1203,15 @@
         thread = Thread(target=my_thread_run)
         running = True
         thread.start()
         sleep(5)
         running = False
         thread.join()
         
-    New in PyTango 9.3.2
+    .. versionadded:: 9.3.2
     """
 
 
 def __doc_is_omni_thread():
     is_omni_thread.__doc__ = """\
 
     Determines if the calling thread is (or looks like) an omniORB thread.
```

### Comparing `pytango-9.4.1rc1/tango/release.py` & `pytango-9.4.2rc1/tango/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         - download_url: (str) package download url
         - platform: (seq<str>) list of available platforms
         - keywords: (seq<str>) list of keywords
         - license: (str) the license
     """
 
     name = "pytango"
-    version_info = (9, 4, 1, "rc", 1)
+    version_info = (9, 4, 2, "rc", 1)
     version = ".".join(map(str, version_info[:3]))
     release = "".join(map(str, version_info[3:]))
     separator = "." if "dev" in release or "post" in release else ""
     version_long = version + separator + release
 
     version_description = "This version implements the C++ Tango 9.4 API."
     version_number = int(version.replace(".", ""))
```

### Comparing `pytango-9.4.1rc1/tango/server.py` & `pytango-9.4.2rc1/tango/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 import sys
 import copy
 from inspect import getfullargspec
 import inspect
 import logging
 import functools
 import traceback
+import asyncio
+import warnings
+import threading
 
 from ._tango import AttrDataFormat, AttrWriteType, CmdArgType, PipeWriteType
-from ._tango import DevFailed, GreenMode, SerialModel
+from ._tango import DevFailed, GreenMode, SerialModel, ApiUtil
 
 from .attr_data import AttrData
 from .pipe_data import PipeData
 from .device_class import DeviceClass
 from .device_server import LatestDeviceImpl, get_worker, set_worker, run_in_executor
 from .utils import get_enum_labels
 from .utils import (
@@ -34,14 +37,15 @@
     is_pure_str,
     is_enum_seq,
     is_enum,
     set_complex_value,
 )
 from .utils import is_devstate, is_devstate_seq, scalar_to_array_type, TO_TANGO_TYPE
 from .green import get_green_mode, get_executor
+from .asyncio_executor import AsyncioExecutor
 from .pyutil import Util
 
 __all__ = (
     "DeviceMeta",
     "Device",
     "LatestDeviceImpl",
     "attribute",
@@ -54,14 +58,58 @@
     "Server",
 )
 
 API_VERSION = 2
 
 # Helpers
 
+_coverage_run_active = False
+
+try:
+    import coverage
+
+    if coverage.Coverage.current():
+        if ApiUtil.get_env_var("PYTANGO_DISABLE_COVERAGE_TRACE_PATCHING"):
+            warnings.warn(
+                "Coverage run detected, but PYTANGO_DISABLE_COVERAGE_TRACE_PATCHING "
+                "environment variable is set. Reported coverage may be inaccurate."
+            )
+        else:
+            if getattr(threading, "_trace_hook", None):
+                _coverage_run_active = True
+                warnings.warn(
+                    "Coverage run detected: tango.server.Device methods "
+                    "will be patched for tracing."
+                )
+            else:
+                warnings.warn(
+                    "Coverage run detected, but unable to get threading._trace_hook. "
+                    "Reported coverage may be inaccurate."
+                )
+
+except Exception:
+    pass
+
+
+def _force_threading_trace_hook(fn):
+    @functools.wraps(fn)
+    def trace_wrapper(*args, **kwargs):
+        original_tracer = sys.gettrace()
+
+        threading_trace_hook = getattr(threading, "_trace_hook", None)
+        if threading_trace_hook:
+            sys.settrace(threading_trace_hook)
+        try:
+            ret = fn(*args, **kwargs)
+        finally:
+            sys.settrace(original_tracer)
+        return ret
+
+    return trace_wrapper
+
 
 def _get_tango_type_format(dtype=None, dformat=None, caller=None):
     if dformat is None:
         dformat = AttrDataFormat.SCALAR
         if is_non_str_seq(dtype):
             if len(dtype):
                 dtype = dtype[0]
@@ -99,14 +147,17 @@
     :type read_method: callable
     """
 
     already_wrapped = hasattr(read_method, "__access_wrapped__")
     if already_wrapped:
         return read_method
 
+    if _coverage_run_active:
+        read_method = _force_threading_trace_hook(read_method)
+
     if attribute.read_green_mode:
 
         @functools.wraps(read_method)
         def read_attr(self, attr):
             worker = get_worker()
             ret = worker.execute(read_method, self)
             if not attr.get_value_flag() and ret is not None:
@@ -152,14 +203,17 @@
     """
     Wraps write method with executor, if needed.
     """
     already_wrapped = hasattr(write_method, "__access_wrapped__")
     if already_wrapped:
         return write_method
 
+    if _coverage_run_active:
+        write_method = _force_threading_trace_hook(write_method)
+
     if attribute.write_green_mode:
 
         @functools.wraps(write_method)
         def write_attr(self, attr):
             value = attr.get_write_value()
             return get_worker().execute(write_method, self, value)
 
@@ -205,14 +259,17 @@
     :param isallowed_method: is allowed method
     :type isallowed_method: callable
     """
     already_wrapped = hasattr(isallowed_method, "__access_wrapped__")
     if already_wrapped:
         return isallowed_method
 
+    if _coverage_run_active:
+        isallowed_method = _force_threading_trace_hook(isallowed_method)
+
     if attribute.isallowed_green_mode:
 
         @functools.wraps(isallowed_method)
         def isallowed_attr(self, request_type):
             worker = get_worker()
             return worker.execute(isallowed_method, self, request_type)
 
@@ -270,14 +327,17 @@
 
 
 def __get_wrapped_pipe_read_method(pipe, read_method):
     already_wrapped = hasattr(read_method, "__access_wrapped__")
     if already_wrapped:
         return read_method
 
+    if _coverage_run_active:
+        read_method = _force_threading_trace_hook(read_method)
+
     if pipe.read_green_mode:
 
         @functools.wraps(read_method)
         def read_pipe(self, pipe):
             worker = get_worker()
             ret = worker.execute(read_method, self)
             if ret is not None:
@@ -321,14 +381,17 @@
 
 
 def __get_wrapped_pipe_write_method(pipe, write_method):
     already_wrapped = hasattr(write_method, "__access_wrapped__")
     if already_wrapped:
         return write_method
 
+    if _coverage_run_active:
+        write_method = _force_threading_trace_hook(write_method)
+
     if pipe.write_green_mode:
 
         @functools.wraps(write_method)
         def write_pipe(self, pipe):
             value = pipe.get_value()
             return get_worker().execute(write_method, self, value)
 
@@ -374,14 +437,17 @@
     :param isallowed_method: is allowed method
     :type isallowed_method: callable
     """
     already_wrapped = hasattr(isallowed_method, "__access_wrapped__")
     if already_wrapped:
         return isallowed_method
 
+    if _coverage_run_active:
+        isallowed_method = _force_threading_trace_hook(isallowed_method)
+
     if pipe.isallowed_green_mode:
 
         @functools.wraps(isallowed_method)
         def isallowed_pipe(self, request_type):
             worker = get_worker()
             return worker.execute(isallowed_method, self, request_type)
 
@@ -445,14 +511,17 @@
     :param cmd_name: command name
     :type cmd_name: str
     """
     already_wrapped = hasattr(is_allowed_method, "__access_wrapped__")
     if already_wrapped:
         return is_allowed_method.__wrapped_method_name__
 
+    if _coverage_run_active:
+        is_allowed_method = _force_threading_trace_hook(is_allowed_method)
+
     method_name = getattr(is_allowed_method, "__name__", f"is_{cmd_name}_allowed")
     method_name = f"__wrapped_{method_name}__"
 
     wrapped_method = run_in_executor(is_allowed_method)
     wrapped_method.__access_wrapped__ = True
     wrapped_method.__wrapped_method_name__ = method_name
     setattr(tango_device_klass, method_name, wrapped_method)
@@ -462,83 +531,120 @@
 
 def __patch_standard_device_methods(klass):
     # TODO allow to force non green mode
 
     init_device_orig = klass.init_device
     already_wrapped = hasattr(init_device_orig, "__access_wrapped__")
     if not already_wrapped:
+        if _coverage_run_active:
+            init_device_orig = _force_threading_trace_hook(init_device_orig)
 
         @functools.wraps(init_device_orig)
         def init_device(self):
             return get_worker().execute(init_device_orig, self)
 
         init_device.__access_wrapped__ = True
         setattr(klass, "init_device", init_device)
 
     delete_device_orig = klass.delete_device
     already_wrapped = hasattr(delete_device_orig, "__access_wrapped__")
     if not already_wrapped:
+        if _coverage_run_active:
+            delete_device_orig = _force_threading_trace_hook(delete_device_orig)
 
         @functools.wraps(delete_device_orig)
         def delete_device(self):
             return get_worker().execute(delete_device_orig, self)
 
         delete_device.__access_wrapped__ = True
         setattr(klass, "delete_device", delete_device)
 
     dev_state_orig = klass.dev_state
     already_wrapped = hasattr(dev_state_orig, "__access_wrapped__")
     if not already_wrapped:
+        dev_state_async = klass._BaseDevice__asyncio_dev_state
+        is_base_klass_state = dev_state_orig == BaseDevice.dev_state
+        if _coverage_run_active:
+            dev_state_orig = _force_threading_trace_hook(dev_state_orig)
+            dev_state_async = _force_threading_trace_hook(dev_state_async)
 
         @functools.wraps(dev_state_orig)
         def dev_state(self):
-            return get_worker().execute(dev_state_orig, self)
+            if isinstance(get_worker(), AsyncioExecutor) and is_base_klass_state:
+                return get_worker().execute(dev_state_async, self)
+            else:
+                return get_worker().execute(dev_state_orig, self)
 
         dev_state.__access_wrapped__ = True
         setattr(klass, "dev_state", dev_state)
 
     dev_status_orig = klass.dev_status
     already_wrapped = hasattr(dev_status_orig, "__access_wrapped__")
     if not already_wrapped:
+        if _coverage_run_active:
+            dev_status_orig = _force_threading_trace_hook(dev_status_orig)
 
         @functools.wraps(dev_status_orig)
         def dev_status(self):
             return get_worker().execute(dev_status_orig, self)
 
         dev_status.__access_wrapped__ = True
         setattr(klass, "dev_status", dev_status)
 
     read_attr_hardware_orig = klass.read_attr_hardware
     already_wrapped = hasattr(read_attr_hardware_orig, "__access_wrapped__")
     if not already_wrapped:
+        if _coverage_run_active:
+            read_attr_hardware_orig = _force_threading_trace_hook(
+                read_attr_hardware_orig
+            )
 
         @functools.wraps(read_attr_hardware_orig)
         def read_attr_hardware(self, attr_list):
             return get_worker().execute(read_attr_hardware_orig, self, attr_list)
 
         read_attr_hardware.__access_wrapped__ = True
         setattr(klass, "read_attr_hardware", read_attr_hardware)
 
     always_executed_hook_orig = klass.always_executed_hook
     already_wrapped = hasattr(always_executed_hook_orig, "__access_wrapped__")
     if not already_wrapped:
+        if _coverage_run_active:
+            always_executed_hook_orig = _force_threading_trace_hook(
+                always_executed_hook_orig
+            )
 
         @functools.wraps(always_executed_hook_orig)
         def always_executed_hook(self):
             return get_worker().execute(always_executed_hook_orig, self)
 
         always_executed_hook.__access_wrapped__ = True
         setattr(klass, "always_executed_hook", always_executed_hook)
 
+    server_init_hook_orig = klass.server_init_hook
+    already_wrapped = hasattr(server_init_hook_orig, "__access_wrapped__")
+    if not already_wrapped:
+
+        @functools.wraps(server_init_hook_orig)
+        def server_init_hook(self):
+            return get_worker().execute(server_init_hook_orig, self)
+
+        server_init_hook.__access_wrapped__ = True
+        setattr(klass, "server_init_hook", server_init_hook)
+
 
 class _DeviceClass(DeviceClass):
     def __init__(self, name):
         DeviceClass.__init__(self, name)
         self.set_type(name)
 
+        if _coverage_run_active:
+            orig_dyn_attr = getattr(self, "dyn_attr")
+            setattr(self, "dyn_attr", _force_threading_trace_hook(orig_dyn_attr))
+
     def dyn_attr(self, dev_list):
         """Invoked to create dynamic attributes for the given devices.
         Default implementation calls
         :meth:`TT.initialize_dynamic_attributes` for each device
 
         :param dev_list: list of devices
         :type dev_list: :class:`tango.DeviceImpl`"""
@@ -727,14 +833,24 @@
         pass
 
     delete_device.__doc__ = LatestDeviceImpl.delete_device.__doc__
 
     def read_attr_hardware(self, attr_list):
         return LatestDeviceImpl.read_attr_hardware(self, attr_list)
 
+    async def __asyncio_dev_state(self):
+        if sys.version_info >= (3, 9):
+            return await asyncio.to_thread(LatestDeviceImpl.dev_state, self)
+        else:
+            warnings.warn(
+                "DevState.ALARM cannot be correctly reported with GreenMode.Asyncio prior to Python 3.9"
+            )
+            # See https://gitlab.com/tango-controls/pytango/-/merge_requests/564 for details
+            return LatestDeviceImpl.dev_state(self)
+
     def dev_state(self):
         return LatestDeviceImpl.dev_state(self)
 
     def dev_status(self):
         return LatestDeviceImpl.dev_status(self)
 
     def get_device_properties(self, ds_class=None):
@@ -771,14 +887,22 @@
     def always_executed_hook(self):
         """
         Tango always_executed_hook. Default implementation does
         nothing
         """
         pass
 
+    def server_init_hook(self):
+        """
+        Tango server_init_hook.  Called once the device server admin device
+        (DServer) is exported.
+        Default implementation does nothing.
+        """
+        pass
+
     def initialize_dynamic_attributes(self):
         """
         Method executed at initializion phase to create dynamic
         attributes. Default implementation does nothing. Overwrite
         when necessary.
         """
         pass
@@ -1379,14 +1503,17 @@
         cmd = f
     else:
 
         @functools.wraps(f)
         def cmd(self, *args, **kwargs):
             return get_worker().execute(f, self, *args, **kwargs)
 
+    if _coverage_run_active:
+        cmd = _force_threading_trace_hook(cmd)
+
     cmd.__tango_command__ = name, [din, dout, config_dict]
 
     # try to create a minimalistic __doc__
     if cmd.__doc__ is None:
         try:
             cmd.__doc__ = __build_command_doc(
                 f, name, dtype_in, doc_in, dtype_out, doc_out
@@ -1650,95 +1777,74 @@
     green_mode=None,
     raises=False,
 ):
     """
     Provides a simple way to run a tango server. It handles exceptions
     by writting a message to the msg_stream.
 
-    The `classes` parameter can be either a sequence of:
+    :Examples:
 
-    * :class:`~tango.server.Device` or
-    * a sequence of two elements
-      :class:`~tango.DeviceClass`, :class:`~tango.DeviceImpl` or
-    * a sequence of three elements
-      :class:`~tango.DeviceClass`, :class:`~tango.DeviceImpl`,
-      tango class name (str)
-
-    or a dictionary where:
-
-    * key is the tango class name
-    * value is either:
-        * a :class:`~tango.server.Device` class or
-        * a sequence of two elements
-          :class:`~tango.DeviceClass`, :class:`~tango.DeviceImpl`
-          or
-        * a sequence of three elements
-          :class:`~tango.DeviceClass`, :class:`~tango.DeviceImpl`,
-          tango class name (str)
-
-    The optional `post_init_callback` can be a callable (without
-    arguments) or a tuple where the first element is the callable,
-    the second is a list of arguments (optional) and the third is a
-    dictionary of keyword arguments (also optional).
-
-    .. note::
-       the order of registration of tango classes defines the order
-       tango uses to initialize the corresponding devices.
-       if using a dictionary as argument for classes be aware that the
-       order of registration becomes arbitrary. If you need a
-       predefined order use a sequence or an OrderedDict.
+        Example 1: registering and running a PowerSupply inheriting from
+        :class:`~tango.server.Device`::
 
-    Example 1: registering and running a PowerSupply inheriting from
-    :class:`~tango.server.Device`::
+            from tango.server import Device, run
 
-        from tango.server import Device, run
+            class PowerSupply(Device):
+                pass
 
-        class PowerSupply(Device):
-            pass
+            run((PowerSupply,))
 
-        run((PowerSupply,))
+        Example 2: registering and running a MyServer defined by tango
+        classes `MyServerClass` and `MyServer`::
 
-    Example 2: registering and running a MyServer defined by tango
-    classes `MyServerClass` and `MyServer`::
+            from tango import Device_4Impl, DeviceClass
+            from tango.server import run
 
-        from tango import Device_4Impl, DeviceClass
-        from tango.server import run
+            class MyServer(Device_4Impl):
+                pass
 
-        class MyServer(Device_4Impl):
-            pass
+            class MyServerClass(DeviceClass):
+                pass
 
-        class MyServerClass(DeviceClass):
-            pass
+            run({'MyServer': (MyServerClass, MyServer)})
 
-        run({'MyServer': (MyServerClass, MyServer)})
+        Example 3: registering and running a MyServer defined by tango
+        classes `MyServerClass` and `MyServer`::
 
-    Example 3: registering and running a MyServer defined by tango
-    classes `MyServerClass` and `MyServer`::
+            from tango import Device_4Impl, DeviceClass
+            from tango.server import Device, run
 
-        from tango import Device_4Impl, DeviceClass
-        from tango.server import Device, run
+            class PowerSupply(Device):
+                pass
 
-        class PowerSupply(Device):
-            pass
+            class MyServer(Device_4Impl):
+                pass
 
-        class MyServer(Device_4Impl):
-            pass
+            class MyServerClass(DeviceClass):
+                pass
 
-        class MyServerClass(DeviceClass):
-            pass
+            run([PowerSupply, [MyServerClass, MyServer]])
+            # or: run({'MyServer': (MyServerClass, MyServer)})
 
-        run([PowerSupply, [MyServerClass, MyServer]])
-        # or: run({'MyServer': (MyServerClass, MyServer)})
+    .. note::
+       the order of registration of tango classes defines the order
+       tango uses to initialize the corresponding devices.
+       if using a dictionary as argument for classes be aware that the
+       order of registration becomes arbitrary. If you need a
+       predefined order use a sequence or an OrderedDict.
 
     :param classes:
-        a sequence of :class:`~tango.server.Device` classes or
-        a dictionary where keyword is the tango class name and value
-        is a sequence of Tango Device Class python class, and Tango
-        Device python class
-    :type classes: sequence or dict
+        Defines for which Tango Device Classes the server will run.
+        If :class:`~dict` is provided, it's key is the tango class name
+        and value is either:
+
+            | :class:`~tango.server.Device`
+            | two element sequence: :class:`~tango.DeviceClass`, :class:`~tango.DeviceImpl`
+            | three element sequence: :class:`~tango.DeviceClass`, :class:`~tango.DeviceImpl`, tango class name :class:`~str`
+    :type classes: Sequence[tango.server.Device] | dict
 
     :param args:
         list of command line arguments [default: None, meaning use
         sys.argv]
     :type args: list
 
     :param msg_stream:
@@ -1751,16 +1857,20 @@
 
     :param event_loop: event_loop callable
     :type event_loop: callable
 
     :param post_init_callback:
         an optional callback that is executed between the calls
         Util.server_init and Util.server_run
+        The optional `post_init_callback` can be a callable (without
+        arguments) or a tuple where the first element is the callable,
+        the second is a list of arguments (optional) and the third is a
+        dictionary of keyword arguments (also optional).
     :type post_init_callback:
-        callable or tuple (see description above)
+        callable or tuple
 
     :param raises:
         Disable error handling and propagate exceptions from the server
     :type raises: bool
 
     :return: The Util singleton object
     :rtype: :class:`~tango.Util`
```

### Comparing `pytango-9.4.1rc1/tango/tango_numpy.py` & `pytango-9.4.2rc1/tango/tango_numpy.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/tango_object.py` & `pytango-9.4.2rc1/tango/tango_object.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/test_context.py` & `pytango-9.4.2rc1/tango/test_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,27 @@
 from ast import literal_eval
 from importlib import import_module
 from argparse import ArgumentParser, ArgumentTypeError
 
 # Local imports
 from .server import run
 from .utils import is_non_str_seq
-from . import DeviceProxy, Database, Util
+from . import Database, DeviceProxy, DevFailed, Util
 
 __all__ = (
     "MultiDeviceTestContext",
     "DeviceTestContext",
     "run_device_test_context",
     "get_server_port_via_pid",
 )
 
 # Helpers
 
-_WINDOWS = "nt" in os.name
-if not _WINDOWS:
-    _DEFAULT_THREAD_TIMEOUT = 3.0
-    _DEFAULT_PROCESS_TIMEOUT = 5.0
-else:
-    _DEFAULT_THREAD_TIMEOUT = 5.0
-    _DEFAULT_PROCESS_TIMEOUT = 7.0
-
+_DEFAULT_THREAD_TIMEOUT = 5.0
+_DEFAULT_PROCESS_TIMEOUT = 7.0
 
 IOR = collections.namedtuple(
     "IOR",
     "first dtype_length dtype nb_profile tag "
     "length major minor wtf host_length host port body",
 )
 
@@ -336,14 +330,16 @@
       Optional. Default is warn.
     :type debug:
       :py:obj:`int`
     :param process:
       True if the device server should be launched in a new process, otherwise
       use a new thread.  Note:  if the context will be used mutiple times, it
       may seg fault if the thread mode is chosen.
+      See the :ref:`issues <testing_approaches_issues>` and
+      :ref:`process kwarg <testing_approaches_process_kwarg>` discussion in the docs.
       Optional.  Default is thread.
     :type process:
       :py:obj:`bool`
     :param daemon:
       True if the new thread/process must be created in daemon mode.
       Optional.  Default is not daemon.
     :type daemon:
@@ -495,28 +491,41 @@
             f.write(", ".join(device_names))
             f.write("\n")
         # Create database
         db = Database(self.db)
         # Write properties
         for info in device_prop_info:
             device_name = info["name"]
-            properties = info.get("properties", {})
+            properties = dict(info.get("properties", {}))
             # Patch the property dict to avoid a PyTango bug
-            patched = {
-                key: value if value != "" else " " for key, value in properties.items()
-            }
-            db.put_device_property(device_name, patched)
+            for key, value in properties.items():
+                if is_non_str_seq(value):
+                    properties[key] = [v if v != "" else " " for v in value]
+                else:
+                    properties[key] = value if value != "" else " "
+            db.put_device_property(device_name, properties)
 
             memorized = info.get("memorized", {})
             munged = {
                 attribute_name: {"__value": memorized_value}
                 for (attribute_name, memorized_value) in memorized.items()
             }
             db.put_device_attribute_property(device_name, munged)
-        return db
+        try:
+            validated_db = Database(self.db)
+        except DevFailed:
+            with open(self.db, "r") as f:
+                content = f.read()
+            raise RuntimeError(
+                f"Invalid FileDatabase file was created.\n"
+                f"Check device properties (empty list or str?): "
+                f"{device_prop_info}.\n"
+                f"Problematic file has content:\n{content}"
+            )
+        return validated_db
 
     def delete_db(self):
         """delete temporary database file only if it was created by this class"""
         if self.handle is not None:
             os.close(self.handle)
             os.unlink(self.db)
```

### Comparing `pytango-9.4.1rc1/tango/test_utils.py` & `pytango-9.4.2rc1/tango/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,19 +27,27 @@
     "DeviceTestContext",
     "SimpleDevice",
     "ClassicAPISimpleDeviceImpl",
     "ClassicAPISimpleDeviceClass",
     "state",
     "command_typed_values",
     "attribute_typed_values",
+    "dev_encoded_values",
     "server_green_mode",
     "attr_data_format",
     "get_server_port_via_pid",
 )
 
+UTF8_STRING = (
+    r"""ăѣ𝔠ծềſģȟᎥ𝒋ǩľḿꞑȯ𝘱𝑞𝗋𝘴ȶ𝞄𝜈ψ𝒙𝘆𝚣1234567890!@#$%^&*()-_=+[{]};:'",<.>/?~𝘈Ḇ𝖢𝕯٤ḞԍНǏ𝙅ƘԸⲘ𝙉০Ρ𝗤Ɍ𝓢ȚЦ𝒱Ѡ𝓧ƳȤ"""
+    r"""ả𝘢ѧᖯć𝗱ễ𝑓𝙜Ⴙ𝞲𝑗𝒌ļṃŉо𝞎𝒒ᵲꜱ𝙩ừ𝗏ŵ𝒙𝒚ź1234567890!@#$%^&*()-_=+[{]};:'",<.>/?~АḂⲤ𝗗𝖤𝗙ꞠꓧȊ𝐉𝜥ꓡ𝑀𝑵Ǭ𝙿𝑄Ŗ𝑆𝒯𝖴𝘝𝘞ꓫŸ𝜡"""
+    r"""𝜶ƀ𝖼ḋếᵮℊ𝙝Ꭵ𝕛кιṃդⱺ𝓅𝘲𝕣𝖘ŧ𝑢ṽẉ𝘅ყž1234567890!@#$%^&*()-_=+[{]};:'",<.>/?~Ѧ𝙱ƇᗞΣℱԍҤ١𝔍К𝓛𝓜ƝȎ𝚸𝑄Ṛ𝓢ṮṺƲᏔꓫ𝚈𝚭"""
+    r"""Ꮟçძ𝑒𝖿𝗀ḧ𝗂𝐣ҝɭḿ𝕟𝐨𝝔𝕢ṛ𝓼тú𝔳ẃ⤬𝝲𝗓1234567890!@#$%^&*()-_=+[{]};:'",<.>/?~𝖠Β𝒞𝘋𝙴𝓕ĢȞỈ𝕵ꓗʟ𝙼ℕ০𝚸𝗤ՀꓢṰǓⅤ𝔚Ⲭ𝑌𝙕𝘢𝕤"""
+)
+
 # char \x00 cannot be sent in a DevString. All other 1-255 chars can
 ints = tuple(range(1, 256))
 bytes_devstring = bytes(ints)
 str_devstring = bytes_devstring.decode("latin-1")
 
 # Test devices
 
@@ -169,14 +177,24 @@
     (ExtractAs.Bytes, bytes),
     (ExtractAs.ByteArray, bytearray),
     (ExtractAs.String, str),
 ]
 
 BASE_TYPES = [float, int, str, bool]
 
+# we also test a large dataset to force memory allocation from heap,
+# to insure immediate segfault if we try to access data after dereferencing
+LARGE_DATA_SIZE = 1 * 1024**2  # 1 Mb seems to be enough
+
+DEV_ENCODED_DATA = {
+    "str": UTF8_STRING,
+    "bytes": UTF8_STRING.encode(),
+    "bytearray": bytearray(UTF8_STRING.encode()),
+}
+
 # these sets to test Device Server input arguments
 
 OS_SYSTEMS = ["linux", "win"]
 
 #    os_system, in string, out arguments list, raised exception
 DEVICE_SERVER_ARGUMENTS = (
     (
@@ -346,14 +364,21 @@
     )
     def attribute_typed_values(request):
         dtype, values = request.param
         expected = lambda v: create_result(dtype, v)
         return dtype, values, expected
 
     @pytest.fixture(
+        params=list(DEV_ENCODED_DATA.items()),
+        ids=list(DEV_ENCODED_DATA.keys()),
+    )
+    def dev_encoded_values(request):
+        return request.param
+
+    @pytest.fixture(
         params=EXTRACT_AS, ids=[f"extract_as.{req_type}" for req_type, _ in EXTRACT_AS]
     )
     def extract_as(request):
         requested_type, expected_type = request.param
         return requested_type, expected_type
 
     @pytest.fixture(params=BASE_TYPES)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytango-9.4.1rc1/tango/time_val.py` & `pytango-9.4.2rc1/tango/time_val.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tango/utils.py` & `pytango-9.4.2rc1/tango/utils.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tests/conftest.py` & `pytango-9.4.2rc1/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """Load tango-specific pytest fixtures."""
 
-from tango.test_utils import state, command_typed_values, attribute_typed_values
+from tango.test_utils import (
+    state,
+    command_typed_values,
+    attribute_typed_values,
+    dev_encoded_values,
+)
 from tango.test_utils import server_green_mode, attr_data_format
 from tango.test_utils import extract_as, base_type
 import pytest
 
 import sys
 import os
 import json
 
 __all__ = (
     "state",
     "command_typed_values",
     "attribute_typed_values",
+    "dev_encoded_values",
     "server_green_mode",
     "attr_data_format",
     "extract_as",
     "base_type",
 )
```

### Comparing `pytango-9.4.1rc1/tests/test_async.py` & `pytango-9.4.2rc1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tests/test_client.py` & `pytango-9.4.2rc1/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 So don't even try to test anything of the above as it will not work
 and is even likely to crash the device (!)
 
 """
 
 import gc
 import weakref
+import asyncio
 
 from distutils.spawn import find_executable
 from subprocess import Popen
 from time import sleep
 
 import pytest
 from functools import partial
@@ -34,20 +35,14 @@
     get_server_port_via_pid,
     str_devstring,
 )
 from tango.gevent import DeviceProxy as gevent_DeviceProxy
 from tango.futures import DeviceProxy as futures_DeviceProxy
 from tango.asyncio import DeviceProxy as asyncio_DeviceProxy
 
-# Asyncio imports
-try:
-    import asyncio
-except ImportError:
-    import trollius as asyncio  # noqa: F401
-
 
 ATTRIBUTES = [
     "State",
     "Status",
     "ampli",
     "boolean_image",
     "boolean_image_ro",
@@ -138,15 +133,15 @@
 
 
 def get_proxy(host, port, device, green_mode):
     access = f"tango://{host}:{port}/{device}#dbase=no"
     return device_proxy_map[green_mode](access)
 
 
-def wait_for_proxy(host, proc, device, green_mode, retries=400, delay=0.01):
+def wait_for_proxy(host, proc, device, green_mode, retries=400, delay=0.03):
     last_error = None
     count = 0
     port = None
     while port is None and count < retries:
         try:
             port = get_server_port_via_pid(proc.pid, host)
         except RuntimeError as exc:
```

### Comparing `pytango-9.4.1rc1/tests/test_event.py` & `pytango-9.4.2rc1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.1rc1/tests/test_server.py` & `pytango-9.4.2rc1/tests/test_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+import multiprocessing
 import os
 import sys
 import textwrap
 import threading
 import time
 import enum
+import inspect
+import asyncio
+
+import psutil
 
 import numpy as np
 import pytest
 
+import tango.asyncio
+import tango.constants
 from tango import (
     AttrData,
     Attr,
     AttrDataFormat,
     AttrQuality,
     AttReqType,
     AttrWriteType,
@@ -22,15 +29,18 @@
     DevEncoded,
     DevEnum,
     DevState,
     DevVoid,
     Device_4Impl,
     Device_5Impl,
     DeviceClass,
+    DeviceProxy,
+    EventType,
     GreenMode,
+    InfoIt,
     LatestDeviceImpl,
     ExtractAs,
     READ_WRITE,
     SCALAR,
     SPECTRUM,
     CmdArgType,
 )
@@ -41,26 +51,32 @@
 from tango.test_utils import DeviceTestContext, MultiDeviceTestContext
 from tango.test_utils import (
     GoodEnum,
     BadEnumNonZero,
     BadEnumSkipValues,
     BadEnumDuplicates,
 )
-from tango.test_utils import assert_close, general_decorator, DEVICE_SERVER_ARGUMENTS
+from tango.test_utils import (
+    assert_close,
+    general_decorator,
+    DEVICE_SERVER_ARGUMENTS,
+    UTF8_STRING,
+)
 from tango.utils import (
     EnumTypeError,
     FROM_TANGO_TO_NUMPY_TYPE,
     TO_TANGO_TYPE,
     get_enum_labels,
     get_latest_device_class,
     is_pure_str,
 )
 
 # Constants
 WINDOWS = "nt" in os.name
+TIMEOUT = 10.0
 
 # Test implementation classes
 
 
 def test_device_classes_use_latest_implementation():
     assert issubclass(LatestDeviceImpl, get_latest_device_class())
     assert issubclass(BaseDevice, LatestDeviceImpl)
@@ -89,14 +105,45 @@
             self.set_state(state)
 
     with DeviceTestContext(TestDevice) as proxy:
         assert proxy.state() == state
         assert proxy.status() == status
 
 
+def test_user_dev_state_status(server_green_mode):
+    state = DevState.MOVING
+    status = "Device is MOVING"
+
+    if server_green_mode == GreenMode.Asyncio:
+
+        class TestDevice(Device):
+            green_mode = server_green_mode
+
+            async def dev_state(self):
+                return state
+
+            async def dev_status(self):
+                return status
+
+    else:
+
+        class TestDevice(Device):
+            green_mode = server_green_mode
+
+            def dev_state(self):
+                return state
+
+            def dev_status(self):
+                return status
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == state
+        assert proxy.status() == status
+
+
 def test_set_status(server_green_mode):
     status = "\n".join(
         (
             "This is a multiline status",
             "with special characters such as",
             "Café à la crème",
         )
@@ -110,14 +157,62 @@
             self.set_status(status)
 
     with DeviceTestContext(TestDevice) as proxy:
         assert proxy.state() == DevState.ON
         assert proxy.status() == status
 
 
+def test_attr_quality_checked_with_state(server_green_mode):
+    if sys.version_info < (3, 9) and server_green_mode == GreenMode.Asyncio:
+        pytest.xfail("In PY<3.9 dev_state with alarm does not work for Asyncio mode")
+
+    class TestDevice(Device):
+        green_mode = server_green_mode
+
+        read_attr_hardware_was_called = False
+        always_executed_hook_was_called = False
+
+        @command(dtype_out=bool)
+        def check_sub_function_was_called(self):
+            return (
+                self.read_attr_hardware_was_called
+                and self.always_executed_hook_was_called
+            )
+
+        sync_code = textwrap.dedent(
+            """
+            def init_device(self):
+                Device.init_device(self)
+                self.set_state(DevState.ON)
+            
+            def read_attr_hardware(self, attr_list):
+                self.read_attr_hardware_was_called = True
+                return Device.read_attr_hardware(self, attr_list)
+
+            def always_executed_hook(self):
+                self.always_executed_hook_was_called = True
+            
+            @attribute(max_alarm=0)
+            def test_attribute(self):
+                return 42
+                """
+        )
+
+        if server_green_mode == GreenMode.Asyncio:
+            exec(
+                sync_code.replace("def", "async def").replace("Device", "await Device")
+            )
+        else:
+            exec(sync_code)
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == DevState.ALARM
+        assert proxy.check_sub_function_was_called()
+
+
 # Test commands
 
 
 def test_identity_command(command_typed_values, server_green_mode):
     dtype, values, expected = command_typed_values
 
     if dtype == (bool,):
@@ -505,14 +600,25 @@
         proxy.make_allowed(False)
         with pytest.raises(DevFailed):
             proxy.attr = value
         with pytest.raises(DevFailed):
             _ = proxy.attr
 
 
+def test_wrong_encoding_string():
+    class TestDevice(Device):
+        @attribute(dtype=str)
+        def wrong_string(self):
+            return "�"
+
+    with DeviceTestContext(TestDevice) as proxy:
+        with pytest.raises(DevFailed, match="UnicodeError"):
+            _ = proxy.wrong_string
+
+
 def test_read_write_attribute_with_unbound_functions(server_green_mode):
     v = {"attr": None}
     is_allowed = None
 
     if server_green_mode == GreenMode.Asyncio:
 
         async def read_attr(device):
@@ -2090,14 +2196,115 @@
             ac3 = self.get_attribute_config(["attr_config_ok"])
             return repr(ac1) == repr(ac2) == repr(ac3)
 
     with DeviceTestContext(TestDevice) as proxy:
         assert proxy.attr_config_ok
 
 
+def test_get_attr_config_ex(server_green_mode):
+    class TestDevice(Device):
+        green_mode = server_green_mode
+
+        @attribute(dtype=int, unit="mA")
+        def attr_config_int(self):
+            return 1
+
+        @attribute(dtype=bool)
+        def attr_config_bool(self):
+            return True
+
+    def assert_attr_config_ok(dev_proxy):
+        # testing that call to get_attribute_config_ex for all types of
+        # input arguments gives same result and doesn't raise an exception
+        ac1 = dev_proxy.get_attribute_config_ex("attr_config_int")
+        ac2 = dev_proxy.get_attribute_config_ex(["attr_config_int"])
+        assert repr(ac1) == repr(ac2)
+
+    def assert_multiple_attrs_config_ok(dev_proxy):
+        # testing that querying multiple attributes gives same result and
+        # doesn't raise an exception
+        ac1 = dev_proxy.get_attribute_config_ex("attr_config_int")
+        ac2 = dev_proxy.get_attribute_config_ex("attr_config_bool")
+        acs = dev_proxy.get_attribute_config_ex(("attr_config_int", "attr_config_bool"))
+        acs_2 = dev_proxy.get_attribute_config_ex(
+            ["attr_config_int", "attr_config_bool"]
+        )
+
+        acs_all = dev_proxy.get_attribute_config_ex(tango.constants.AllAttr)
+
+        assert repr(ac1[0]) == repr(acs[0]) == repr(acs_2[0]) == repr(
+            acs_all[0]
+        ) and repr(ac2[0]) == repr(acs[1]) == repr(acs_2[1]) == repr(acs_all[1])
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert_attr_config_ok(proxy)
+        assert_multiple_attrs_config_ok(proxy)
+
+
+def test_default_units(server_green_mode):
+    # testing that, by default tango.constants.UnitNotSpec is set
+    # when no unit is specified. For bool, int, float and str dtypes
+    class TestDevice(Device):
+        green_mode = server_green_mode
+
+        @attribute(dtype=bool)
+        def attr_bool_ok(self):
+            return True
+
+        @attribute(dtype=int)
+        def attr_int_ok(self):
+            return 1
+
+        @attribute(dtype=float)
+        def attr_float_ok(self):
+            return 1.0
+
+        @attribute(dtype=str)
+        def attr_str_ok(self):
+            return "True"
+
+    def assert_attr_bool_ok(dev_proxy):
+        config = dev_proxy.get_attribute_config("attr_bool_ok")
+        assert config.unit == tango.constants.UnitNotSpec
+
+    def assert_attr_int_ok(dev_proxy):
+        config = dev_proxy.get_attribute_config("attr_int_ok")
+        assert config.unit == tango.constants.UnitNotSpec
+
+    def assert_attr_float_ok(dev_proxy):
+        config = dev_proxy.get_attribute_config("attr_float_ok")
+        assert config.unit == tango.constants.UnitNotSpec
+
+    def assert_attr_str_ok(dev_proxy):
+        config = dev_proxy.get_attribute_config("attr_str_ok")
+        assert config.unit == tango.constants.UnitNotSpec
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert_attr_bool_ok(proxy)
+        assert_attr_int_ok(proxy)
+        assert_attr_float_ok(proxy)
+        assert_attr_str_ok(proxy)
+
+
+def test_custom_units(server_green_mode):
+    class TestDevice(Device):
+        green_mode = server_green_mode
+
+        @attribute(dtype=bool, unit="mA")
+        def custom_unit_ok(self):
+            return True
+
+    def assert_custom_unit_ok(dev_proxy):
+        config = dev_proxy.get_attribute_config("custom_unit_ok")
+        assert config.unit == "mA"
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert_custom_unit_ok(proxy)
+
+
 # Test inheritance
 
 
 def test_inheritance_override_a_property(server_green_mode):
     class A(Device):
         green_mode = server_green_mode
 
@@ -2719,14 +2926,98 @@
             if len(msg) > 1:
                 check_log_msg = log_msg[0] % log_msg[1]
             else:
                 check_log_msg = log_msg[0]
             assert_log_details_correct(level, check_log_msg)
 
 
+@pytest.mark.skipif(
+    not os.environ.get("PYTHONUNBUFFERED"),
+    reason="This test requires PYTHONUNBUFFERED=1 to capture the outputs.",
+)
+def test_decorator_logging_source_location(server_green_mode, capfd):
+    """Run decorated commands and attributes and verify that @InfoIt decorator
+    always logs the correct location."""
+
+    class InfoItDevice(Device):
+        green_mode = server_green_mode
+
+        @InfoIt()
+        @command(dtype_out=int)
+        def decorated_command(self):
+            return inspect.currentframe().f_lineno
+
+        @command(dtype_out=int)
+        def run_decorated_method(self):
+            return self.decorated_method()
+
+        @InfoIt()
+        @general_decorator
+        def decorated_method(self):
+            return inspect.currentframe().f_lineno
+
+        @attribute(dtype=int)
+        @InfoIt()
+        def decorated_attribute(self):
+            return inspect.currentframe().f_lineno
+
+    with DeviceTestContext(InfoItDevice, debug=3) as device:
+        filename = os.path.basename(__file__)
+        for cmd, method in [
+            ("decorated_command", "decorated_command"),
+            ("run_decorated_method", "decorated_method"),
+        ]:
+            lineno = device.command_inout(cmd) - 3
+            out, err = capfd.readouterr()  # calling this function clears the buffer
+            assert (
+                f"({filename}:{lineno}) test/nodb/infoitdevice -> InfoItDevice.{method}()"
+                in out
+            )
+
+        lineno = device.decorated_attribute - 3
+        out, err = capfd.readouterr()
+        assert (
+            f"({filename}:{lineno}) test/nodb/infoitdevice -> InfoItDevice.decorated_attribute()"
+            in out
+        )
+
+
+@pytest.mark.skipif(
+    not os.environ.get("PYTHONUNBUFFERED"),
+    reason="This test requires PYTHONUNBUFFERED=1 to capture the outputs.",
+)
+def test_stream_logging_source_location(server_green_mode, capfd):
+    class StreamLogsDevice(Device):
+        green_mode = server_green_mode
+
+        @command(dtype_out=int)
+        def log_streams(self):
+            self.info_stream("info")
+            self.debug_stream("debug")
+            self.warn_stream("warn")
+            self.error_stream("error")
+            self.fatal_stream("fatal")
+            return inspect.currentframe().f_lineno
+
+    with DeviceTestContext(StreamLogsDevice, debug=3) as device:
+        lineno = device.command_inout("log_streams") - 5
+        filename = os.path.basename(__file__)
+        out, err = capfd.readouterr()
+        for i, level in [
+            (0, "INFO"),
+            (1, "DEBUG"),
+            (2, "WARN"),
+            (3, "ERROR"),
+            (4, "FATAL"),
+        ]:
+            assert (
+                f"{level} ({filename}:{lineno + i}) test/nodb/streamlogsdevice" in out
+            )
+
+
 # fixtures
 
 
 @pytest.fixture(params=[GoodEnum])
 def good_enum(request):
     return request.param
 
@@ -2748,51 +3039,213 @@
     with pytest.raises(EnumTypeError):
         get_enum_labels(bad_enum)
 
 
 # DevEncoded
 
 
-def test_read_write_dev_encoded(server_green_mode):
+def test_read_write_dev_encoded(dev_encoded_values, server_green_mode):
+    def check_ans(raw_ans, expected_type):
+        assert len(raw_ans) == 2
+        assert is_pure_str(raw_ans[0])
+        if expected_type == bytes:
+            assert isinstance(raw_ans[1], bytes)
+            assert raw_ans[1] == UTF8_STRING.encode()
+        elif expected_type == str:
+            assert is_pure_str(raw_ans[1])
+            assert raw_ans[1] == UTF8_STRING
+        else:
+            assert isinstance(raw_ans[1], bytearray)
+            assert raw_ans[1] == bytearray(UTF8_STRING.encode())
+
     class TestDevice(Device):
         green_mode = server_green_mode
-        attr_value = ("uint8", b"\xd2\xd3")
+        attr_value = None
+        command_value = None
 
         @attribute(dtype=DevEncoded, access=AttrWriteType.READ_WRITE)
         def attr(self):
             return self.attr_value
 
         @attr.write
         def attr(self, value):
+            check_ans(value, bytes)
             self.attr_value = value
 
         @command(dtype_in=DevEncoded)
         def cmd_in(self, value):
-            self.attr_value = value
+            check_ans(value, bytes)
+            self.command_value = value
 
         @command(dtype_out=DevEncoded)
         def cmd_out(self):
-            return self.attr_value
+            return self.command_value
 
         @command(dtype_in=DevEncoded, dtype_out=DevEncoded)
         def cmd_in_out(self, value):
-            self.attr_value = value
-            return self.attr_value
+            check_ans(value, bytes)
+            return value
 
     with DeviceTestContext(TestDevice) as proxy:
-        assert proxy.attr == ("uint8", b"\xd2\xd3")
+        proxy.attr = dev_encoded_values
+        raw_ans = proxy.read_attribute("attr", extract_as=ExtractAs.Bytes)
+        check_ans(raw_ans.value, bytes)
+        check_ans(raw_ans.w_value, bytes)
+
+        raw_ans = proxy.read_attribute("attr", extract_as=ExtractAs.String)
+        check_ans(raw_ans.value, str)
+        check_ans(raw_ans.w_value, str)
+
+        raw_ans = proxy.read_attribute("attr", extract_as=ExtractAs.ByteArray)
+        check_ans(raw_ans.value, bytearray)
+        check_ans(raw_ans.w_value, bytearray)
+
+        proxy.cmd_in(dev_encoded_values)
+        raw_ans = proxy.cmd_out()
+        check_ans(raw_ans, bytes)
+
+        raw_ans = proxy.cmd_in_out(dev_encoded_values)
+        check_ans(raw_ans, bytes)
 
-        proxy.attr = ("uint8", b"\xde")
-        assert proxy.attr == ("uint8", b"\xde")
 
-        proxy.cmd_in(("uint8", b"\xd4\xd5"))
-        assert proxy.cmd_out() == ("uint8", b"\xd4\xd5")
+def test_dev_encoded_wrong_encoding():
+    class TestDevice(Device):
+        @attribute(dtype=DevEncoded, access=AttrWriteType.READ)
+        def attr_bad_encoding(self):
+            return "utf-16", UTF8_STRING.encode("utf-16")
+
+        @attribute(dtype=DevEncoded, access=AttrWriteType.READ)
+        def attr_bad_string(self):
+            return "bad_one", b"\xff"
+
+    with DeviceTestContext(TestDevice) as proxy:
+        with pytest.raises(UnicodeDecodeError):
+            _ = proxy.read_attribute("attr_bad_encoding", extract_as=ExtractAs.String)
 
-        proxy.cmd_in_out(("uint8", b"\xd6\xd7"))
-        assert proxy.attr == ("uint8", b"\xd6\xd7")
+        with pytest.raises(UnicodeDecodeError):
+            _ = proxy.read_attribute("attr_bad_string", extract_as=ExtractAs.String)
+
+
+def test_dev_encoded_memory_usage():
+    LARGE_DATA_SIZE = 10 * 1024 * 1024  # 1 Mb should be enough, but 10 more reliable
+    NUM_CYCLES = 5
+
+    def check_ans(raw_ans):
+        assert len(raw_ans) == 2
+        assert is_pure_str(raw_ans[0])
+        assert isinstance(raw_ans[1], bytes)
+        assert len(raw_ans[1]) == LARGE_DATA_SIZE
+        if raw_ans[0] == "str":
+            assert raw_ans[1] == b"a" * LARGE_DATA_SIZE
+        elif raw_ans[0] == "bytes":
+            assert raw_ans[1] == b"b" * LARGE_DATA_SIZE
+        else:
+            assert raw_ans[1] == b"c" * LARGE_DATA_SIZE
+
+    class TestDevice(Device):
+        attr_str_read = attribute(
+            dtype=DevEncoded, access=AttrWriteType.READ, fget="read_str"
+        )
+        attr_str_write = attribute(
+            dtype=DevEncoded, access=AttrWriteType.WRITE, fset="write_str"
+        )
+        attr_str_read_write = attribute(
+            dtype=DevEncoded,
+            access=AttrWriteType.READ_WRITE,
+            fget="read_str",
+            fset="write_str",
+        )
+
+        attr_bytes_read = attribute(
+            dtype=DevEncoded, access=AttrWriteType.READ, fget="read_bytes"
+        )
+        attr_bytes_write = attribute(
+            dtype=DevEncoded, access=AttrWriteType.WRITE, fset="write_bytes"
+        )
+        attr_bytes_read_write = attribute(
+            dtype=DevEncoded,
+            access=AttrWriteType.READ_WRITE,
+            fget="read_bytes",
+            fset="write_bytes",
+        )
+
+        attr_bytearray_read = attribute(
+            dtype=DevEncoded, access=AttrWriteType.READ, fget="read_bytearray"
+        )
+        attr_bytearray_write = attribute(
+            dtype=DevEncoded, access=AttrWriteType.WRITE, fset="write_bytearray"
+        )
+        attr_bytearray_read_write = attribute(
+            dtype=DevEncoded,
+            access=AttrWriteType.READ_WRITE,
+            fget="read_bytearray",
+            fset="write_bytearray",
+        )
+
+        def read_str(self):
+            return "str", "a" * LARGE_DATA_SIZE
+
+        def write_str(self, value):
+            check_ans(value)
+
+        def read_bytes(self):
+            return "bytes", b"b" * LARGE_DATA_SIZE
+
+        def write_bytes(self, value):
+            check_ans(value)
+
+        def read_bytearray(self):
+            return "bytearray", bytearray(b"c" * LARGE_DATA_SIZE)
+
+        def write_bytearray(self, value):
+            check_ans(value)
+
+        @command(dtype_in=DevEncoded, dtype_out=DevEncoded)
+        def cmd_in_out(self, value):
+            check_ans(value)
+            if value[0] == "str":
+                return "str", "a" * LARGE_DATA_SIZE
+            elif value[0] == "bytes":
+                return "bytes", b"b" * LARGE_DATA_SIZE
+            else:
+                return "bytearray", bytearray(b"c" * LARGE_DATA_SIZE)
+
+    with DeviceTestContext(TestDevice) as proxy:
+        last_memory_usage = None
+        for cycle in range(NUM_CYCLES):
+            proxy.attr_str_write = "str", "a" * LARGE_DATA_SIZE
+            proxy.attr_bytes_write = "bytes", b"b" * LARGE_DATA_SIZE
+            proxy.attr_bytearray_write = "bytearray", bytearray(b"c" * LARGE_DATA_SIZE)
+
+            proxy.attr_str_read_write = "str", "a" * LARGE_DATA_SIZE
+            proxy.attr_bytes_read_write = "bytes", b"b" * LARGE_DATA_SIZE
+            proxy.attr_bytearray_read_write = "bytearray", bytearray(
+                b"c" * LARGE_DATA_SIZE
+            )
+
+            check_ans(proxy.attr_str_read)
+            check_ans(proxy.attr_bytes_read)
+            check_ans(proxy.attr_bytearray_read)
+
+            check_ans(proxy.attr_str_read_write)
+            check_ans(proxy.attr_bytes_read_write)
+            check_ans(proxy.attr_bytearray_read_write)
+
+            check_ans(proxy.cmd_in_out(("str", "a" * LARGE_DATA_SIZE)))
+            check_ans(proxy.cmd_in_out(("bytes", b"b" * LARGE_DATA_SIZE)))
+            check_ans(
+                proxy.cmd_in_out(("bytearray", bytearray(b"c" * LARGE_DATA_SIZE)))
+            )
+
+            current_memory_usage = int(psutil.Process(os.getpid()).memory_info().rss)
+            if cycle > 2:  # first two cycles we memory usage grows....
+                assert np.isclose(
+                    last_memory_usage, current_memory_usage, atol=LARGE_DATA_SIZE / 2
+                )
+            last_memory_usage = current_memory_usage
 
 
 # Test Exception propagation
 
 
 def test_exception_propagation(server_green_mode):
     class TestDevice(Device):
@@ -2841,7 +3294,259 @@
     ids=_avoid_double_colon_node_ids,
 )
 def test_arguments(applicable_os, test_input, expected_output, os_system):
     try:
         assert set(parse_args(test_input.split())) == set(expected_output)
     except SystemExit:
         assert sys.platform not in applicable_os
+
+
+# Test Server init hook
+
+
+def test_server_init_hook_called(server_green_mode):
+    class TestDevice(Device):
+        green_mode = server_green_mode
+        server_init_hook_called = False
+
+        def server_init_hook(self):
+            TestDevice.server_init_hook_called = True
+
+    with DeviceTestContext(TestDevice):
+        assert TestDevice.server_init_hook_called
+
+
+def test_asyncio_server_init_hook_called():
+    class TestDevice(Device):
+        green_mode = GreenMode.Asyncio
+        has_been_called = False
+
+        async def server_init_hook(self):
+            await asyncio.sleep(0.01)
+            TestDevice.has_been_called = True
+
+    with DeviceTestContext(TestDevice):
+        assert TestDevice.has_been_called
+
+
+def test_server_init_hook_change_state(server_green_mode):
+    class TestDevice(Device):
+        green_mode = server_green_mode
+
+        def server_init_hook(self):
+            self.set_state(DevState.ON)
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == DevState.ON
+
+
+def test_asyncio_server_init_hook_change_state():
+    class TestDevice(Device):
+        green_mode = GreenMode.Asyncio
+
+        async def server_init_hook(self):
+            await asyncio.sleep(0.01)
+            self.set_state(DevState.ON)
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == DevState.ON
+
+
+def test_server_init_hook_called_after_init():
+    class TestDevice(Device):
+        def init_device(self):
+            self.set_state(DevState.INIT)
+
+        def server_init_hook(self):
+            self.set_state(DevState.ON)
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == DevState.ON
+
+
+def test_async_server_init_hook_called_after_init():
+    class TestDevice(Device):
+        green_mode = GreenMode.Asyncio
+
+        async def init_device(self):
+            await asyncio.sleep(0.01)
+            self.set_state(DevState.INIT)
+
+        async def server_init_hook(self):
+            await asyncio.sleep(0.01)
+            self.set_state(DevState.ON)
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == DevState.ON
+
+
+def test_server_init_hook_exception(server_green_mode):
+    class TestDevice(Device):
+        green_mode = server_green_mode
+
+        def server_init_hook(self):
+            self.set_state(DevState.ON)
+            raise RuntimeError("Force exception for test")
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == DevState.FAULT
+
+
+def test_asyncio_server_init_hook_exception():
+    class TestDevice(Device):
+        green_mode = GreenMode.Asyncio
+
+        async def server_init_hook(self):
+            await asyncio.sleep(0.01)
+            raise RuntimeError("Force exception for test")
+
+    with DeviceTestContext(TestDevice) as proxy:
+        assert proxy.state() == DevState.FAULT
+
+
+def test_server_init_hook_with_low_level_api_called(server_green_mode):
+    class ClassicAPISimpleDeviceImpl(LatestDeviceImpl):
+        green_mode = server_green_mode
+        has_been_called = False
+
+        def server_init_hook(self):
+            self.set_state(DevState.ON)
+            ClassicAPISimpleDeviceImpl.has_been_called = True
+
+    class ClassicAPISimpleDeviceClass(DeviceClass):
+        pass
+
+    with DeviceTestContext(ClassicAPISimpleDeviceImpl, ClassicAPISimpleDeviceClass):
+        assert ClassicAPISimpleDeviceImpl.has_been_called
+
+
+def test_server_init_hook_with_low_level_api_change_state(server_green_mode):
+    class ClassicAPISimpleDeviceImpl(LatestDeviceImpl):
+        green_mode = server_green_mode
+
+        def server_init_hook(self):
+            self.set_state(DevState.ON)
+
+    class ClassicAPISimpleDeviceClass(DeviceClass):
+        pass
+
+    with DeviceTestContext(
+        ClassicAPISimpleDeviceImpl, ClassicAPISimpleDeviceClass
+    ) as proxy:
+        assert proxy.state() == DevState.ON
+
+
+def test_server_init_hook_with_low_level_api_called_after_init():
+    class ClassicAPISimpleDeviceImpl(LatestDeviceImpl):
+        def init_device(self):
+            self.set_state(DevState.INIT)
+
+        def server_init_hook(self):
+            self.set_state(DevState.ON)
+
+    class ClassicAPISimpleDeviceClass(DeviceClass):
+        pass
+
+    with DeviceTestContext(
+        ClassicAPISimpleDeviceImpl, ClassicAPISimpleDeviceClass
+    ) as proxy:
+        assert proxy.state() == DevState.ON
+
+
+def test_server_init_hook_with_low_level_api_exception(server_green_mode):
+    class ClassicAPISimpleDeviceImpl(LatestDeviceImpl):
+        green_mode = server_green_mode
+
+        def server_init_hook(self):
+            self.set_state(DevState.ON)
+            raise RuntimeError("Force exception for test")
+
+    class ClassicAPISimpleDeviceClass(DeviceClass):
+        pass
+
+    with DeviceTestContext(
+        ClassicAPISimpleDeviceImpl, ClassicAPISimpleDeviceClass
+    ) as proxy:
+        assert proxy.state() == DevState.FAULT
+
+
+def test_server_init_multiple_devices():
+    event_list = []
+
+    class DeviceOne(Device):
+        def server_init_hook(self):
+            event_list.append("DeviceOne")
+
+    class DeviceTwo(Device):
+        def server_init_hook(self):
+            event_list.append("DeviceTwo")
+
+    devices_info = (
+        {"class": DeviceOne, "devices": [{"name": "test/device1/1"}]},
+        {
+            "class": DeviceTwo,
+            "devices": [{"name": "test/device2/1"}, {"name": "test/device3/1"}],
+        },
+    )
+
+    with MultiDeviceTestContext(
+        devices_info, host="127.0.0.1", port=11000, process=False
+    ):
+        assert len(event_list) == 3
+        assert "DeviceOne" in event_list
+        assert "DeviceTwo" in event_list
+
+
+def test_server_init_hook_subscribe_event_multiple_devices():
+    if "win" in sys.platform:
+        pytest.xfail("This test fails in Windows, will be fixed soon")
+
+    event_queue = multiprocessing.Queue()
+
+    class DeviceOne(Device):
+        @attribute(dtype=int)
+        def some_attribute(self):
+            return 42
+
+        def init_device(self):
+            super().init_device()
+            self.set_change_event("some_attribute", True, False)
+
+        @command
+        def push_event_cmd(self):
+            self.push_change_event("some_attribute", 43)
+
+    class DeviceTwo(Device):
+        def event_handler(self, data):
+            event_queue.put(data.attr_value.value)
+
+        def server_init_hook(self):
+            self.dev1_proxy = DeviceProxy(
+                "tango://127.0.0.1:11000/test/device1/1#dbase=no"
+            )
+            self.dev1_proxy.subscribe_event(
+                "some_attribute", EventType.CHANGE_EVENT, self.event_handler
+            )
+
+    devices_info = (
+        {"class": DeviceOne, "devices": [{"name": "test/device1/1"}]},
+        {
+            "class": DeviceTwo,
+            "devices": [{"name": "test/device2/1"}, {"name": "test/device3/1"}],
+        },
+    )
+
+    with MultiDeviceTestContext(
+        devices_info, host="127.0.0.1", port=11000, process=True
+    ) as context:
+        proxy = context.get_device("test/device1/1")
+
+        # synchronous event
+        assert 42 == event_queue.get(timeout=TIMEOUT)
+        assert 42 == event_queue.get(timeout=TIMEOUT)
+        assert event_queue.empty()
+
+        # asynchronous event pushed from user code
+        proxy.push_event_cmd()
+        assert 43 == event_queue.get(timeout=TIMEOUT)
+        assert 43 == event_queue.get(timeout=TIMEOUT)
+        assert event_queue.empty()
```

### Comparing `pytango-9.4.1rc1/tests/test_test_context.py` & `pytango-9.4.2rc1/tests/test_test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
-
 import pytest
-
 import tango
 
+import numpy as np
+
 from tango import AttrWriteType, GreenMode
 from tango.asyncio_executor import AsyncioExecutor
 from tango.device_server import get_worker
 from tango.gevent_executor import GeventExecutor
 from tango.green import SynchronousExecutor
 from tango.server import Device
 from tango.server import command, attribute, device_property
@@ -441,14 +441,23 @@
     with MultiDeviceTestContext(devices_info) as context:
         proxy1 = context.get_device("test/device1/1")
         proxy2 = context.get_device("test/device2/2")
         assert proxy1.get_prop1() == "abcd"
         assert proxy2.get_prop2() == 5555
 
 
+def test_multi_raises_on_invalid_file_database_properties():
+    class TestDevice(Device):
+        empty = device_property(dtype=(str,))
+
+    with pytest.raises(RuntimeError, match="FileDatabase"):
+        with DeviceTestContext(TestDevice, properties={"empty": []}):
+            pass
+
+
 @pytest.fixture(
     # Per test we have the input config tuple, and then the expected exception type
     params=[
         # empty config
         [tuple(), IndexError],
         # missing/invalid keys
         [({"not-class": Device1, "devices": [{"name": "test/device1/1"}]},), KeyError],
@@ -571,7 +580,29 @@
 
     kwargs = (
         {"memorized": {"attr": memorized_value}} if memorized_value is not None else {}
     )
 
     with DeviceTestContext(TestDevice, **kwargs) as proxy:
         assert proxy.attr == expected_value
+
+
+@pytest.mark.parametrize(
+    "property_type, property_value, expected_outcome",
+    [
+        (str, {"prop": ""}, " "),
+        ((str,), {"prop": ["", ""]}, (" ", " ")),
+        ((str,), {"prop": np.array(["", ""])}, (" ", " ")),
+    ],
+)
+def test_empty_string_property_bug(property_type, property_value, expected_outcome):
+    class TestDevice(Device):
+        prop = device_property(
+            dtype=property_type,
+        )
+
+        @attribute(dtype=property_type, max_dim_x=10)
+        def attr(self):
+            return self.prop
+
+    with DeviceTestContext(TestDevice, properties=property_value) as proxy:
+        assert proxy.attr == expected_outcome
```

### Comparing `pytango-9.4.1rc1/winsetup.py` & `pytango-9.4.2rc1/winsetup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,75 +11,54 @@
 # ------------------------------------------------------------------------------
 
 # ------------------------------------------------------------------------------
 # WARNING: This script should only be executed as a Post-Build Event from inside
 #          Microsoft Visual Studio and not from the command line
 # ------------------------------------------------------------------------------
 
-
-import sys
 import os
-import os.path as osp
+import sys
+import traceback
 
 
 def main():
-    executable = sys.executable
-
-    curr_dir = os.getcwd()
-
-    winsetup_dir = osp.dirname(osp.abspath(__file__))
-    os.chdir(winsetup_dir)
-    setup_name = "setup.py"
-    bitmap = osp.join(winsetup_dir, "doc", "logo-medium.bmp")
-    ver = ".".join(map(str, sys.version_info[:2]))
-
     print("winsetup: invoked with: " + " ".join(sys.argv))
     if len(sys.argv) < 6:
         print(
-            "winsetup: need to supply build directory, distribution directory, temporary binary install directory, configuration name and platform name"
+            "winsetup: need to supply build directory, distribution directory, "
+            "temporary binary install directory, configuration name and platform name"
         )
         return 1
 
-    build_dir, dist_dir, bdist_dir = map(osp.abspath, sys.argv[1:4])
+    build_dir, dist_dir, bdist_dir = map(os.path.abspath, sys.argv[1:4])
     config_name, plat_name = sys.argv[4:6]
     # Pypi is picky about platform name. Make sure we obey his/her majesty
     plat_name = plat_name.lower()
-    #    temp_base_dir = osp.abspath(os.environ["TEMP"])
-    #    temp_dir = osp.join(temp_base_dir, "PyTango", config_name)
     if plat_name == "x64":
         plat_name = "win-amd64"
 
+    executable = sys.executable
+    setup_name = "setup.py"
+    curr_dir = os.getcwd()
+    winsetup_dir = os.path.dirname(os.path.abspath(__file__))
+    os.chdir(winsetup_dir)
     try:
-        cmd_line = f"{executable} {setup_name} "
-        cmd_line += f"build_py --force --no-compile --build-lib={build_dir} "
-        cmd_line += "build_scripts --force "
-        cmd_line += f"install_lib --skip-build --no-compile --build-dir={build_dir} "
-        #        cmd_line += 'bdist_msi --skip-build --target-version=%s ' \
-        #                    '--bdist-dir=%s ' \
-        #                    '--dist-dir=%s ' \
-        #                    '--plat-name=%s ' % (ver, bdist_dir, dist_dir, plat_name)
-        cmd_line += (
-            f"bdist_wininst --skip-build --target-version={ver} "
-            f"--bdist-dir={bdist_dir} "
-            f"--dist-dir={dist_dir} "
-            f'--title="PyTango 9" '
-            f'--bitmap="{bitmap}" '
-            f"--plat-name={plat_name} "
-        )
-        cmd_line += (
+        cmd_line = (
+            f"{executable} {setup_name} "
+            f"build_py --force --no-compile --build-lib={build_dir} "
+            f"build_scripts --force "
+            f"install_lib --skip-build --no-compile --build-dir={build_dir} "
             f"bdist_wheel --skip-build "
             f"--bdist-dir={bdist_dir} "
             f"--dist-dir={dist_dir} "
             f"--plat-name={plat_name} "
         )
         os.system(cmd_line)
     except Exception:
         print("Failed:")
-        import traceback
-
         traceback.print_exc()
         return 2
     finally:
         os.chdir(curr_dir)
 
     return 0
```

