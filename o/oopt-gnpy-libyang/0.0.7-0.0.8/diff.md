# Comparing `tmp/oopt-gnpy-libyang-0.0.7.tar.gz` & `tmp/oopt-gnpy-libyang-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oopt-gnpy-libyang-0.0.7.tar", last modified: Tue May 30 13:38:50 2023, max compression
+gzip compressed data, was "oopt-gnpy-libyang-0.0.8.tar", last modified: Thu Jul 13 13:15:21 2023, max compression
```

## Comparing `oopt-gnpy-libyang-0.0.7.tar` & `oopt-gnpy-libyang-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.673618 oopt-gnpy-libyang-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/oopt-gnpy-libyang.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/tests/yang/
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/iana-hardware@2018-03-13.yang
--rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/iana-if-type@2017-01-19.yang
--rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/ietf-hardware@2018-03-13.yang
--rw-r--r--   0 runner    (1001) docker     (123)    39365 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/ietf-interfaces@2018-02-20.yang
--rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/ietf-ip@2018-02-22.yang
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:15:21.268693 oopt-gnpy-libyang-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:15:21.264693 oopt-gnpy-libyang-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:15:21.264693 oopt-gnpy-libyang-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-13 13:15:21.264693 oopt-gnpy-libyang-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/oopt-gnpy-libyang.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:15:21.264693 oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-13 13:15:21.000000 oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-13 13:15:21.000000 oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:15:21.000000 oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:15:21.000000 oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 13:15:21.000000 oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 13:15:21.000000 oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:15:21.268693 oopt-gnpy-libyang-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:15:21.264693 oopt-gnpy-libyang-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:15:21.264693 oopt-gnpy-libyang-0.0.8/tests/yang/
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/yang/iana-hardware@2018-03-13.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/yang/iana-if-type@2017-01-19.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/yang/ietf-hardware@2018-03-13.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    39365 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/yang/ietf-interfaces@2018-02-20.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-07-13 13:13:20.000000 oopt-gnpy-libyang-0.0.8/tests/yang/ietf-ip@2018-02-22.yang
```

### Comparing `oopt-gnpy-libyang-0.0.7/.github/workflows/ci.yaml` & `oopt-gnpy-libyang-0.0.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/CMakeLists.txt` & `oopt-gnpy-libyang-0.0.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/LICENSE` & `oopt-gnpy-libyang-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/PKG-INFO` & `oopt-gnpy-libyang-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oopt-gnpy-libyang
-Version: 0.0.7
+Version: 0.0.8
 Summary: Opinionated Python bindings for the libyang library
 Home-page: https://github.com/Telecominfraproject/oopt-gnpy-libyang
 Download-URL: https://pypi.org/project/oopt-gnpy-libyang/
 Author: Telecom Infra Project
 Author-email: jan.kundrat@telecominfraproject.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
```

### Comparing `oopt-gnpy-libyang-0.0.7/README.md` & `oopt-gnpy-libyang-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/oopt-gnpy-libyang.cpp` & `oopt-gnpy-libyang-0.0.8/oopt-gnpy-libyang.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 #include <pybind11/functional.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/stl/filesystem.h>
+#include <regex>
+#include <sstream>
 #include <libyang-cpp/Context.hpp>
 #include <libyang/version.h>
 
 using namespace std::literals;
 using namespace pybind11::literals;
 using namespace libyang;
 namespace py = pybind11;
 
+namespace {
+std::string quote_string(const std::string& what)
+{
+    return "\"" +
+        std::regex_replace( // escape quotes
+                std::regex_replace( // escape backslashes
+                    what, std::regex("\\\\"), "\\\\"),
+                std::regex("\""), "\\\"")
+        + "\"";
+}
+
+std::string repr_optional_string(const std::optional<std::string>& what)
+{
+    return what ? quote_string(*what) : "None"s;
+}
+}
+
 PYBIND11_MODULE(oopt_gnpy_libyang, m) {
     m.doc() = "Opinionated Python bindings for the libyang library";
 
     py::enum_<ContextOptions>(m, "ContextOptions")
         .value("AllImplemented", ContextOptions::AllImplemented)
         .value("RefImplemented", ContextOptions::RefImplemented)
         .value("NoYangLibrary", ContextOptions::NoYangLibrary)
@@ -28,14 +47,21 @@
     py::enum_<LogLevel>(m, "LogLevel")
         .value("Error", LogLevel::Error)
         .value("Warning", LogLevel::Warning)
         .value("Verbose", LogLevel::Verbose)
         .value("Debug", LogLevel::Debug)
         ;
 
+    py::enum_<LogOptions>(m, "LogOptions")
+        .value("Log", LogOptions::Log)
+        .value("Store", LogOptions::Store)
+        .value("StoreLast", LogOptions::StoreLast)
+        .def("__or__", [](LogOptions a, LogOptions b){ return a | b; })
+        ;
+
     py::enum_<ErrorCode>(m, "ErrorCode")
         .value("Success", ErrorCode::Success)
         .value("MemoryFailure", ErrorCode::MemoryFailure)
         .value("SyscallFail", ErrorCode::SyscallFail)
         .value("InvalidValue", ErrorCode::InvalidValue)
         .value("ItemAlreadyExists", ErrorCode::ItemAlreadyExists)
         .value("NotFound", ErrorCode::NotFound)
@@ -134,14 +160,26 @@
     py::class_<ErrorInfo>(m, "ErrorInfo")
         .def_readonly("app_tag", &ErrorInfo::appTag)
         .def_readonly("level", &ErrorInfo::level)
         .def_readonly("message", &ErrorInfo::message)
         .def_readonly("code", &ErrorInfo::code)
         .def_readonly("path", &ErrorInfo::path)
         .def_readonly("validation_code", &ErrorInfo::validationCode)
+        .def("__repr__", [](const ErrorInfo& e) {
+                    std::ostringstream ss;
+                    ss << "ErrorInfo(";
+                    ss << "level = " << e.level;
+                    ss << ", code = " << e.code;
+                    ss << ", validation_code = " << e.validationCode;
+                    ss << ", message = " << repr_optional_string(e.message);
+                    ss << ", path = " << repr_optional_string(e.path);
+                    ss << ", app_tag = " << repr_optional_string(e.appTag);
+                    ss << ")";
+                    return ss.str();
+                })
         ;
 
     py::class_<DataNode>(m, "DataNode")
         .def_property("path", &DataNode::path, nullptr)
         .def_property("is_term", &DataNode::isTerm, nullptr)
         .def("as_term", &DataNode::asTerm)
         .def("print", &DataNode::printStr, "format"_a, "flags"_a)
@@ -204,8 +242,11 @@
         .def("parse_module",
                 py::overload_cast<const std::filesystem::path&, const SchemaFormat>(&Context::parseModule, py::const_),
                 "path"_a, "format"_a)
         ;
 
     m.def("libyang_version", []() { return LY_VERSION; });
     m.def("libyang_version_info", []() { return py::make_tuple(LY_VERSION_MAJOR, LY_VERSION_MINOR, LY_VERSION_MICRO); });
+
+    m.def("set_log_level", &setLogLevel, "level"_a);
+    m.def("set_log_options", &setLogOptions, "options"_a);
 }
```

### Comparing `oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/PKG-INFO` & `oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oopt-gnpy-libyang
-Version: 0.0.7
+Version: 0.0.8
 Summary: Opinionated Python bindings for the libyang library
 Home-page: https://github.com/Telecominfraproject/oopt-gnpy-libyang
 Download-URL: https://pypi.org/project/oopt-gnpy-libyang/
 Author: Telecom Infra Project
 Author-email: jan.kundrat@telecominfraproject.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
```

### Comparing `oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/SOURCES.txt` & `oopt-gnpy-libyang-0.0.8/oopt_gnpy_libyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/pyproject.toml` & `oopt-gnpy-libyang-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/setup.py` & `oopt-gnpy-libyang-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/conftest.py` & `oopt-gnpy-libyang-0.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/test_context.py` & `oopt-gnpy-libyang-0.0.8/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/test_validation.py` & `oopt-gnpy-libyang-0.0.8/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/yang/iana-hardware@2018-03-13.yang` & `oopt-gnpy-libyang-0.0.8/tests/yang/iana-hardware@2018-03-13.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/yang/iana-if-type@2017-01-19.yang` & `oopt-gnpy-libyang-0.0.8/tests/yang/iana-if-type@2017-01-19.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/yang/ietf-hardware@2018-03-13.yang` & `oopt-gnpy-libyang-0.0.8/tests/yang/ietf-hardware@2018-03-13.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/yang/ietf-interfaces@2018-02-20.yang` & `oopt-gnpy-libyang-0.0.8/tests/yang/ietf-interfaces@2018-02-20.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.7/tests/yang/ietf-ip@2018-02-22.yang` & `oopt-gnpy-libyang-0.0.8/tests/yang/ietf-ip@2018-02-22.yang`

 * *Files identical despite different names*

