# Comparing `tmp/flea-9.1.0.tar.gz` & `tmp/flea-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flea-9.1.0.tar", last modified: Thu Mar 23 11:19:48 2023, max compression
+gzip compressed data, was "flea-9.1.1.tar", last modified: Thu Jul 13 11:09:28 2023, max compression
```

## Comparing `flea-9.1.0.tar` & `flea-9.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-03-23 11:19:48.887736 flea-9.1.0/
--rw-r--r--   0 oliver    (1001) wheel        (0)     7409 2023-03-23 11:14:57.000000 flea-9.1.0/CHANGELOG.rst
--rw-r--r--   0 oliver    (1001) wheel        (0)    11359 2023-03-23 11:14:57.000000 flea-9.1.0/LICENCE.TXT
--rw-r--r--   0 oliver    (1001) wheel        (0)       91 2023-03-23 11:14:57.000000 flea-9.1.0/MANIFEST.in
--rw-r--r--   0 oliver    (1001) wheel        (0)     1324 2023-03-23 11:19:48.887844 flea-9.1.0/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      618 2023-03-23 11:14:57.000000 flea-9.1.0/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-03-23 11:19:48.885101 flea-9.1.0/doc/
--rw-r--r--   0 oliver    (1001) wheel        (0)      637 2023-03-23 11:14:57.000000 flea-9.1.0/doc/Makefile
--rw-r--r--   0 oliver    (1001) wheel        (0)     5535 2023-03-23 11:14:57.000000 flea-9.1.0/doc/conf.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    17934 2023-03-23 11:14:57.000000 flea-9.1.0/doc/index.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-03-23 11:19:48.886514 flea-9.1.0/flea/
--rw-r--r--   0 oliver    (1001) wheel        (0)      713 2023-03-23 11:19:46.000000 flea-9.1.0/flea/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    35443 2023-03-23 11:14:57.000000 flea-9.1.0/flea/agent.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      884 2023-03-23 11:14:57.000000 flea-9.1.0/flea/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    30854 2023-03-23 11:14:57.000000 flea-9.1.0/flea/html.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4917 2023-03-23 11:14:57.000000 flea-9.1.0/flea/util.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3045 2023-03-23 11:14:57.000000 flea-9.1.0/flea/wsgi.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-03-23 11:19:48.887557 flea-9.1.0/flea.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)     1324 2023-03-23 11:19:48.000000 flea-9.1.0/flea.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      334 2023-03-23 11:19:48.000000 flea-9.1.0/flea.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-03-23 11:19:48.000000 flea-9.1.0/flea.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       29 2023-03-23 11:19:48.000000 flea-9.1.0/flea.egg-info/requires.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        5 2023-03-23 11:19:48.000000 flea-9.1.0/flea.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      922 2023-03-23 11:19:48.888527 flea-9.1.0/setup.cfg
--rw-r--r--   0 oliver    (1001) wheel        (0)      613 2023-03-23 11:14:57.000000 flea-9.1.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-13 11:09:28.468123 flea-9.1.1/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7593 2023-07-13 11:08:23.000000 flea-9.1.1/CHANGELOG.rst
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11359 2023-07-13 11:08:22.000000 flea-9.1.1/LICENCE.TXT
+-rw-r--r--   0 oliver    (1001) wheel        (0)       91 2023-07-13 11:08:22.000000 flea-9.1.1/MANIFEST.in
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1324 2023-07-13 11:09:28.468233 flea-9.1.1/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      618 2023-07-13 11:08:22.000000 flea-9.1.1/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-13 11:09:28.465562 flea-9.1.1/doc/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      638 2023-07-13 11:08:22.000000 flea-9.1.1/doc/Makefile
+-rw-r--r--   0 oliver    (1001) wheel        (0)     5535 2023-07-13 11:08:22.000000 flea-9.1.1/doc/conf.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    17934 2023-07-13 11:08:22.000000 flea-9.1.1/doc/index.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-13 11:09:28.466901 flea-9.1.1/flea/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      713 2023-07-13 11:09:27.000000 flea-9.1.1/flea/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    35031 2023-07-13 11:08:22.000000 flea-9.1.1/flea/agent.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      884 2023-07-13 11:08:22.000000 flea-9.1.1/flea/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    30854 2023-07-13 11:08:22.000000 flea-9.1.1/flea/html.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4917 2023-07-13 11:08:22.000000 flea-9.1.1/flea/util.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3045 2023-07-13 11:08:22.000000 flea-9.1.1/flea/wsgi.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-13 11:09:28.467942 flea-9.1.1/flea.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1324 2023-07-13 11:09:28.000000 flea-9.1.1/flea.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      334 2023-07-13 11:09:28.000000 flea-9.1.1/flea.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-07-13 11:09:28.000000 flea-9.1.1/flea.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       29 2023-07-13 11:09:28.000000 flea-9.1.1/flea.egg-info/requires.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        5 2023-07-13 11:09:28.000000 flea-9.1.1/flea.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      922 2023-07-13 11:09:28.469032 flea-9.1.1/setup.cfg
+-rw-r--r--   0 oliver    (1001) wheel        (0)      613 2023-07-13 11:08:22.000000 flea-9.1.1/setup.py
```

### Comparing `flea-9.1.0/CHANGELOG.rst` & `flea-9.1.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Changes
 ---------
 
-9.1.0 (released 2023-03-23)
+9.1.1 (released 2023-07-13)
+---------------------------
+
+* Bugfix: ensure WSGI iterator close methods are always called
+
+9.1.0 (released 2023-03-21)
 ---------------------------
 
 * Support Python 3.11
 * Added ``json`` argument to Agent request methods, for example ``Agent.post("/", json={"x": 2})``.
+* Bugfix: ensure WSGI iterator close methods are always called
 
 9.0.1 (released 2020-08-21)
 ---------------------------
 
 * Bugfix: cookies with the SameSite attribute are correctly handled in Python<=3.7
 
 9.0.0 (released 2020-04-14)
```

### Comparing `flea-9.1.0/LICENCE.TXT` & `flea-9.1.1/LICENCE.TXT`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/PKG-INFO` & `flea-9.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flea
-Version: 9.1.0
+Version: 9.1.1
 Summary: Functional testing for WSGI: drive WSGI apps from your test suite
 Home-page: https://ollycope.com/software/flea/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi,tests,testing,pytest,nose
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flea Version: 9.1.0 Summary: Functional testing for
+Metadata-Version: 2.1 Name: flea Version: 9.1.1 Summary: Functional testing for
 WSGI: drive WSGI apps from your test suite Home-page: https://ollycope.com/
 software/flea/latest/ Author: Oliver Cope Author-email: oliver@redgecko.org
 License: Apache Keywords: wsgi,tests,testing,pytest,nose Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Classifier: Topic :: Software
```

### Comparing `flea-9.1.0/README.rst` & `flea-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/doc/Makefile` & `flea-9.1.1/doc/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
-SPHINXBUILD   = ../.tox/py37-sphinx/bin/sphinx-build
+SPHINXBUILD   = ../.tox/py311-sphinx/bin/sphinx-build
 SPHINXPROJ    = yoyo-migrations
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `flea-9.1.0/doc/conf.py` & `flea-9.1.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/doc/index.rst` & `flea-9.1.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/flea/__init__.py` & `flea-9.1.1/flea/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import unicode_literals, absolute_import
 from .agent import *  # noqa
 from .html import *  # noqa
 
-__version__ = "9.1.0"
+__version__ = "9.1.1"
```

### Comparing `flea-9.1.0/flea/agent.py` & `flea-9.1.1/flea/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,42 +225,34 @@
                 self._read_response()
         else:
             self.charset = self.default_charset
 
         # Stores file upload field values in forms
         self.file_uploads = {}
 
-        self.environ_defaults = (
-            environ_defaults or self.environ_defaults
-        ).copy()
-        self.environ_defaults.update(
-            {"SERVER_NAME": host, "SERVER_PORT": str(port)}
-        )
+        self.environ_defaults = (environ_defaults or self.environ_defaults).copy()
+        self.environ_defaults.update({"SERVER_NAME": host, "SERVER_PORT": str(port)})
 
     def __repr__(self):
         if self.request:
-            return ("<{} {!r}>").format(
-                self.__class__.__name__, self.request.path
-            )
+            return ("<{} {!r}>").format(self.__class__.__name__, self.request.path)
         else:
             return ("<{} (no request yet)>").format(self.__class__.__name__)
 
     def make_environ(
         self, REQUEST_METHOD="GET", PATH_INFO="", wsgi_input=b"", **kwargs
     ):
         """
         Return a dictionary suitable for use as the WSGI environ.
 
         PATH_INFO must be URL encoded. As a convenience it may also contain a
         query string portion which will be used as the QUERY_STRING WSGI
         variable.
         """
-        SCRIPT_NAME = kwargs.pop(
-            "SCRIPT_NAME", self.environ_defaults["SCRIPT_NAME"]
-        )
+        SCRIPT_NAME = kwargs.pop("SCRIPT_NAME", self.environ_defaults["SCRIPT_NAME"])
 
         if SCRIPT_NAME and SCRIPT_NAME[-1] == "/":
             SCRIPT_NAME = SCRIPT_NAME[:-1]
             PATH_INFO = "/" + PATH_INFO
 
         if "?" in PATH_INFO:
             if "QUERY_STRING" in kwargs:
@@ -268,20 +260,17 @@
                     "QUERY_STRING specified both in "
                     "PATH_INFO and as argument to "
                     "make_environ"
                 )
             PATH_INFO, querystring = PATH_INFO.split("?", 1)
             kwargs["QUERY_STRING"] = str_to_environ(querystring)
 
-        assert re.match(
-            r"^[/A-Za-z0-9\-._~!$/&\'()*+,;=:@%]*$", PATH_INFO
-        ), "Path info not URL encoded"
-
-        assert not re.search(
-            r"%(?![A-F0-9]{2})", PATH_INFO
+        assert is_url_encoded_pattern.match(PATH_INFO), "Path info not URL encoded"
+        assert not contains_invalid_escapes_pattern.search(
+            PATH_INFO
         ), "Path info not URL encoded"
 
         # Unquote requires a string argument
         if isinstance(PATH_INFO, bytes):
             PATH_INFO = PATH_INFO.decode("ascii")
         if isinstance(SCRIPT_NAME, bytes):
             SCRIPT_NAME = SCRIPT_NAME.decode("ascii")
@@ -315,17 +304,15 @@
             environ["PATH_INFO"] = "/" + environ["PATH_INFO"]
 
         while PATH_INFO.startswith("//"):
             PATH_INFO = PATH_INFO[1:]
 
         return environ
 
-    def _wsgi_request(
-        self, environ, follow=True, history=False, check_status=True
-    ):
+    def _wsgi_request(self, environ, follow=True, history=False, check_status=True):
         """
         Low level entry point for making requests to the WSGI application.
 
         Return a Agent object representing the new state resulting from the
         request.
 
         :param environ: WSGI environ to be used for the request
@@ -350,26 +337,25 @@
         else:
             history = self.history
 
         if self.options["logger"]:
             request = Request(environ.copy())
             self.options["logger"].info("%s %s", request.method, request.url)
             if environ["HTTP_COOKIE"]:
-                self.options["logger"].debug(
-                    "Cookie: %s", environ["HTTP_COOKIE"]
-                )
+                self.options["logger"].debug("Cookie: %s", environ["HTTP_COOKIE"])
             postdata = environ["wsgi.input"].getvalue()
             environ["wsgi.input"].seek(0)
             if postdata:
                 self.options["logger"].info("wsgi.input: %r", postdata)
 
         original_environ = environ.copy()
         response = self.response_class.from_wsgi(
             self.validated_app, environ, self.start_response
         )
+
         agent = self.__class__(
             self.app,
             environ,
             response,
             self.cookies,
             history,
             original_environ=original_environ,
@@ -458,28 +444,24 @@
         else:
             envargs = kwargs
 
         wsgi_input = BytesIO(data)
         wsgi_input.seek(0)
 
         return self._wsgi_request(
-            self.make_environ(
-                method, PATH_INFO, wsgi_input=wsgi_input, **envargs
-            ),
+            self.make_environ(method, PATH_INFO, wsgi_input=wsgi_input, **envargs),
             follow,
             history,
             check_status,
         )
 
     def get(self, PATH_INFO="/", data=None, charset="UTF-8", *args, **kwargs):
         kwargs.setdefault("method", "GET")
         if data is not None:
-            kwargs.setdefault(
-                "QUERY_STRING", urlencode_wrapper(data, encoding=charset)
-            )
+            kwargs.setdefault("QUERY_STRING", urlencode_wrapper(data, encoding=charset))
             data = None
         return self._request(PATH_INFO, data, charset, *args, **kwargs)
 
     def head(self, *args, **kwargs):
         return self.get(method="HEAD", *args, **kwargs)
 
     def post(self, *args, **kwargs):
@@ -491,21 +473,15 @@
     def put(self, *args, **kwargs):
         return self._request(method="PUT", *args, **kwargs)
 
     def patch(self, *args, **kwargs):
         return self._request(method="PATCH", *args, **kwargs)
 
     def post_multipart(
-        self,
-        PATH_INFO="/",
-        data=None,
-        charset="UTF-8",
-        files=None,
-        *args,
-        **kwargs
+        self, PATH_INFO="/", data=None, charset="UTF-8", files=None, *args, **kwargs
     ):
         """
         POST a request to the given URI using multipart/form-data encoding.
 
         :param PATH_INFO: The path to request from the application. This must
                           be a URL encoded string.
 
@@ -537,34 +513,28 @@
             for the given key/value pair
             """
             if isinstance(value, tuple):
                 filename, content_type, data = value
                 headers = [
                     (
                         "Content-Disposition",
-                        'form-data; name="%s"; filename="%s"'
-                        % (key, filename),
+                        'form-data; name="%s"; filename="%s"' % (key, filename),
                     ),
                     ("Content-Type", content_type),
                 ]
                 return headers, data
             else:
                 if not isinstance(value, bytes):
                     value = value.encode(charset)
-                headers = [
-                    ("Content-Disposition", 'form-data; name="%s"' % (key,))
-                ]
+                headers = [("Content-Disposition", 'form-data; name="%s"' % (key,))]
                 return headers, value
 
         items = chain(
             (add_headers(k, v) for k, v in data),
-            (
-                add_headers(k, (fname, ctype, data))
-                for k, fname, ctype, data in files
-            ),
+            (add_headers(k, (fname, ctype, data)) for k, fname, ctype, data in files),
         )
 
         CRLF = b"\r\n"
         post_data = BytesIO()
         post_data.write(b"--" + boundary)
         for headers, data in items:
             post_data.write(CRLF)
@@ -586,22 +556,18 @@
             post_data.write(b"--" + boundary)
         post_data.write(b"--" + CRLF)
         length = post_data.tell()
         kwargs.setdefault("method", "POST")
         kwargs.setdefault("CONTENT_LENGTH", str(length))
         kwargs.setdefault(
             "CONTENT_TYPE",
-            str_to_environ(
-                "multipart/form-data; boundary=" + boundary.decode("ascii")
-            ),
+            str_to_environ("multipart/form-data; boundary=" + boundary.decode("ascii")),
         )
 
-        return self._request(
-            PATH_INFO, post_data.getvalue(), charset=charset, **kwargs
-        )
+        return self._request(PATH_INFO, post_data.getvalue(), charset=charset, **kwargs)
 
     def post_json(self, path, data, ajax=False, *args, **kwargs):
         """
         POST JSON-encoded data to the application.
 
         :param ajax: if True, an 'X-Requested-With: XMLHttpRequest'
                      header will be added
@@ -632,30 +598,28 @@
             **kwargs
         )
 
     def reload(self, follow=True, check_status=True):
         """
         Reload the current page, if necessary re-posting any data.
 
-        Form fields that have been filled in on the loaded page, they will be
+        Form fields that have been filled in on the loaded page will be
         refilled on the reloaded page, provided that the reloaded page has
         exactly the same fields present in the same order.
         """
         if self.options["logger"]:
             self.options["logger"].debug("Reload: %s", self.request.path)
         env = self.original_environ.copy()
 
         wsgi_input = env["wsgi.input"]
         if isinstance(wsgi_input, wsgiref.validate.InputWrapper):
             wsgi_input = wsgi_input.input
         wsgi_input.seek(0)
         env["wsgi.input"] = wsgi_input
-        agent = self._wsgi_request(
-            env, follow=follow, check_status=check_status
-        )
+        agent = self._wsgi_request(env, follow=follow, check_status=check_status)
 
         if self._lxml is not None:
             for src, dst in zip(
                 self.find("//input|//textarea|//option"),
                 agent.find("//input|//textarea|//option"),
             ):
                 if not all(
@@ -708,26 +672,23 @@
     def __str__(self):
         if self.response:
             return str(self.response)
         else:
             return super(Agent, self).__str__()
 
     def _read_response(self):
-
         if not self.response:
             return
         if self._body is not None:
             return
         try:
             self._body = b"".join(self.response.content)
         finally:
-            try:
-                self.response.content.close()
-            except AttributeError:
-                pass
+            for close in self.response.onclose:
+                close()
 
     @property
     def status(self):
         """
         The server reponse status, as a string (eg ``200 OK``)
         """
         try:
@@ -980,15 +941,17 @@
                     self.response.status,
                     self.request.method,
                     self.request.path,
                 )
             )
 
         return self.get(
-            self.response.get_header("Location"), history=False, follow=False,
+            self.response.get_header("Location"),
+            history=False,
+            follow=False,
         )
 
     def follow_all(self):
         """
         If response has a ``30x`` status code, fetch (``GET``) the redirect
         target, until a non-redirect code is received. No entries are recorded
         in the agent's history list.
@@ -1037,21 +1000,16 @@
         Subsequent requests from the browser are then proxied directly to the
         WSGI application under test.
         """
         host = self.environ_defaults["SERVER_NAME"]
         port = int(self.environ_defaults["SERVER_PORT"])
 
         url = self.request.make_url(netloc="{0}:{1}".format(host, port))
-        print(
-            "\nStarting HTTP server on {0}\n"
-            "Press ctrl-c to exit.".format(url)
-        )
-        server = make_server(
-            host, port, PassStateWSGIApp(self, self.request.path)
-        )
+        print("\nStarting HTTP server on {0}\n" "Press ctrl-c to exit.".format(url))
+        server = make_server(host, port, PassStateWSGIApp(self, self.request.path))
         if open_in_browser:
             webbrowser.open_new_tab(url)
         try:
             server.serve_forever()
         except KeyboardInterrupt:
             pass
 
@@ -1062,7 +1020,11 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """
         At end of context block, reset the lxml document
         """
         self.reset()
+
+
+is_url_encoded_pattern = re.compile(r"^[/A-Za-z0-9\-._~!$/&\'()*+,;=:@%]*$")
+contains_invalid_escapes_pattern = re.compile(r"%(?![A-F0-9]{2})")
```

### Comparing `flea-9.1.0/flea/exceptions.py` & `flea-9.1.1/flea/exceptions.py`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/flea/html.py` & `flea-9.1.1/flea/html.py`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/flea/util.py` & `flea-9.1.1/flea/util.py`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/flea/wsgi.py` & `flea-9.1.1/flea/wsgi.py`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/flea.egg-info/PKG-INFO` & `flea-9.1.1/flea.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flea
-Version: 9.1.0
+Version: 9.1.1
 Summary: Functional testing for WSGI: drive WSGI apps from your test suite
 Home-page: https://ollycope.com/software/flea/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi,tests,testing,pytest,nose
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flea Version: 9.1.0 Summary: Functional testing for
+Metadata-Version: 2.1 Name: flea Version: 9.1.1 Summary: Functional testing for
 WSGI: drive WSGI apps from your test suite Home-page: https://ollycope.com/
 software/flea/latest/ Author: Oliver Cope Author-email: oliver@redgecko.org
 License: Apache Keywords: wsgi,tests,testing,pytest,nose Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Classifier: Topic :: Software
```

### Comparing `flea-9.1.0/setup.cfg` & `flea-9.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `flea-9.1.0/setup.py` & `flea-9.1.1/setup.py`

 * *Files identical despite different names*

