# Comparing `tmp/shandy-sqlfmt-0.8.0.tar.gz` & `tmp/shandy-sqlfmt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shandy-sqlfmt-0.8.0.tar", max compression
+gzip compressed data, was "shandy-sqlfmt-0.9.0.tar", max compression
```

## Comparing `shandy-sqlfmt-0.8.0.tar` & `shandy-sqlfmt-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2022-05-04 02:14:05.509009 shandy-sqlfmt-0.8.0/LICENSE
--rwxr-xr-x   0        0        0    15227 2022-05-04 02:14:05.509009 shandy-sqlfmt-0.8.0/README.md
--rw-r--r--   0        0        0     1798 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/pyproject.toml
--rwxr-xr-x   0        0        0       86 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/__init__.py
--rw-r--r--   0        0        0    11926 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/actions.py
--rw-r--r--   0        0        0     7110 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/analyzer.py
--rwxr-xr-x   0        0        0     6002 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/api.py
--rw-r--r--   0        0        0     3220 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/cache.py
--rwxr-xr-x   0        0        0     5636 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/cli.py
--rw-r--r--   0        0        0     4953 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/comment.py
--rw-r--r--   0        0        0     2718 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/config.py
--rw-r--r--   0        0        0    20879 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/dialect.py
--rw-r--r--   0        0        0     1536 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/exception.py
--rw-r--r--   0        0        0     3081 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/formatter.py
--rw-r--r--   0        0        0     6495 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/jinjafmt.py
--rw-r--r--   0        0        0    12611 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/line.py
--rw-r--r--   0        0        0    12557 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/merger.py
--rw-r--r--   0        0        0     1390 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/mode.py
--rw-r--r--   0        0        0    16711 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/node.py
--rw-r--r--   0        0        0      934 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/query.py
--rw-r--r--   0        0        0     6471 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/report.py
--rw-r--r--   0        0        0     3635 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/splitter.py
--rw-r--r--   0        0        0     2355 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt/token.py
--rw-r--r--   0        0        0        0 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt_primer/__init__.py
--rw-r--r--   0        0        0       64 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt_primer/__main__.py
--rw-r--r--   0        0        0     8393 2022-05-04 02:14:05.513009 shandy-sqlfmt-0.8.0/src/sqlfmt_primer/primer.py
--rw-r--r--   0        0        0    16714 2022-05-04 02:14:24.840541 shandy-sqlfmt-0.8.0/setup.py
--rw-r--r--   0        0        0    16649 2022-05-04 02:14:24.841764 shandy-sqlfmt-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/LICENSE
+-rwxr-xr-x   0        0        0    15968 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/README.md
+-rw-r--r--   0        0        0     1798 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0       86 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/__init__.py
+-rw-r--r--   0        0        0    11926 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/actions.py
+-rw-r--r--   0        0        0     7110 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/analyzer.py
+-rwxr-xr-x   0        0        0     6096 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/api.py
+-rw-r--r--   0        0        0     3410 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/cache.py
+-rwxr-xr-x   0        0        0     5862 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/cli.py
+-rw-r--r--   0        0        0     4953 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/comment.py
+-rw-r--r--   0        0        0     2718 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/config.py
+-rw-r--r--   0        0        0    20879 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/dialect.py
+-rw-r--r--   0        0        0     1536 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/exception.py
+-rw-r--r--   0        0        0     3081 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/formatter.py
+-rw-r--r--   0        0        0    13017 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/jinjafmt.py
+-rw-r--r--   0        0        0    12611 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/line.py
+-rw-r--r--   0        0        0    12557 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/merger.py
+-rw-r--r--   0        0        0     1420 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/mode.py
+-rw-r--r--   0        0        0    16711 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/node.py
+-rw-r--r--   0        0        0      934 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/query.py
+-rw-r--r--   0        0        0     6471 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/report.py
+-rw-r--r--   0        0        0     3635 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/splitter.py
+-rw-r--r--   0        0        0     2355 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt/token.py
+-rw-r--r--   0        0        0        0 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt_primer/__init__.py
+-rw-r--r--   0        0        0       64 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt_primer/__main__.py
+-rw-r--r--   0        0        0     8400 2022-06-02 22:46:13.310138 shandy-sqlfmt-0.9.0/src/sqlfmt_primer/primer.py
+-rw-r--r--   0        0        0    17464 2022-06-02 22:46:38.931214 shandy-sqlfmt-0.9.0/setup.py
+-rw-r--r--   0        0        0    17390 2022-06-02 22:46:38.932616 shandy-sqlfmt-0.9.0/PKG-INFO
```

### Comparing `shandy-sqlfmt-0.8.0/LICENSE` & `shandy-sqlfmt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/README.md` & `shandy-sqlfmt-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 You can configure [pre-commit](https://pre-commit.com/) to run sqlfmt on your repository before you commit changes.
 
 Add the following config to your `.pre-commit-config.yaml` file:
 
 ```
 repos:
   - repo: https://github.com/tconbeer/sqlfmt
-    rev: v0.7.0
+    rev: v0.9.0
     hooks:
       - id: sqlfmt
         language_version: python
 ```
 
 You should replace `rev` with the latest available release, but we do suggest pinning to a specific rev, to avoid unexpected formatting changes.
 
@@ -266,7 +266,17 @@
 1. Install [Poetry](https://python-poetry.org/docs/#installation) if you don't have it already. You may also need or want pyenv, make, and gcc. A complete setup from a fresh install of Ubuntu can be found [here](https://github.com/tconbeer/linux_setup)
 1. Clone this repo into a directory (let's call it `sqlfmt`), then `cd sqlfmt`
 1. Use `poetry install -E jinjafmt` to install the project (editable) and its dependencies into a new virtual env. To run `sqlfmt_primer`, you will need to install it (and its dependencies) by specifying it as an extra: `poetry install -E jinjafmt -E sqlfmt_primer`
 1. Use `poetry shell` to spawn a subshell
 1. Type `make` to run all tests and linters, or run `pytest`, `black`, `flake8`, `isort`, and `mypy` individually.
 
 Note: If encountering a JSONDecodeError during `poetry install`, you will want to clear the poetry cache with `poetry cache clear pypi --all`, or upgrade to poetry >= 1.12 with `poetry self upgrade`
+
+### Updating primer repos to reflect formatting changes
+
+1. Make sure all changes are committed to sqlfmt
+1. Check out the `unformatted` tag in the repo with `git checkout -b chore/apply-abc123 unformatted` where `abc123` is the hash of the most recent sqlfmt commit (from 1)
+1. Run sqlfmt against the working tree, then `git add .` and `git commit -m "chore: apply sqlfmt abc123"`
+1. We will have conflicts with main that we want to ignore, so merge main into this branch, ignoring anything on main: `git merge -s ours main`
+1. Push and open a PR; squash and merge. Grab the commit SHA
+1. Paste the commit SHA as a ref into `primer.py`
+1. Run `sqlfmt_primer -k` to clear the cache, then update the stats in `primer.py` to match the results
```

### Comparing `shandy-sqlfmt-0.8.0/pyproject.toml` & `shandy-sqlfmt-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "shandy-sqlfmt"
-version = "0.8.0"
+version = "0.9.0"
 description = "sqlfmt is an opinionated CLI tool that formats your sql files"
 readme = "README.md"
 authors = ["Ted Conbeer <ted@shandy.io>"]
 license = "Apache-2.0"
 homepage = "http://sqlfmt.com"
 repository = "https://github.com/tconbeer/sqlfmt"
 classifiers = [
@@ -38,16 +38,16 @@
 gitpython = { version = "^3.1.24", optional = true }
 black = { version = "*", optional = true }
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 isort = "^5.9.3"
-mypy = "^0.950"
-pre-commit = "^2.18.1"
+mypy = "^0.960"
+pre-commit = "^2.19.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 snakeviz = { version = "^2.1.1", optional = true }
 
 [tool.poetry.scripts]
 sqlfmt = "sqlfmt.cli:sqlfmt"
 sqlfmt_primer = "sqlfmt_primer.primer:sqlfmt_primer"
```

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/actions.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/actions.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/analyzer.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/analyzer.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/api.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import concurrent.futures
 import sys
 from functools import partial
 from glob import glob
 from pathlib import Path
 from typing import Callable, Collection, Iterable, List, Set, TypeVar
 
-from sqlfmt.cache import Cache, check_cache, load_cache, write_cache
+from sqlfmt.cache import Cache, check_cache, clear_cache, load_cache, write_cache
 from sqlfmt.exception import SqlfmtError
 from sqlfmt.formatter import QueryFormatter
 from sqlfmt.mode import Mode
 from sqlfmt.report import STDIN_PATH, Report, SqlFormatResult
 
 T = TypeVar("T")
 R = TypeVar("R")
@@ -34,15 +34,20 @@
 
     Modifies sql files in place, by default. Check or diff mode do not modify files,
     they only create a report.
 
     Returns a Report that can be queried or printed.
     """
 
-    cache = load_cache()
+    if mode.reset_cache:
+        clear_cache()
+        cache = {}
+    else:
+        cache = load_cache()
+
     matched_paths = _get_matching_paths(files, mode)
     results = _format_many(matched_paths, cache, mode)
 
     report = Report(results, mode)
 
     if not (mode.check or mode.diff):
         _update_source_files(results)
```

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/cache.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,25 @@
     for path in _gen_cache_keys_for_updates(results, mode):
         updated_info = _get_cache_info(path)
         new_cache[path] = updated_info
     with open(cache_file, "wb") as f:
         pickle.dump(new_cache, f)
 
 
+def clear_cache() -> None:
+    """
+    Deletes the cache file on disk, if it exists
+    """
+    p = get_cache_file()
+    try:
+        p.unlink()
+    except FileNotFoundError:
+        pass
+
+
 def _get_cache_info(path: Path) -> Tuple[float, int]:
     """
     Returns a tuple of (modified_time, file_size) for the path; this tuple is
     persisted to the cache, and we check the files on disk against this cached
     value to determine if we need to format the file again
     """
     stat = path.resolve().stat()
```

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/cli.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,23 @@
     help=(
         "Run sqlfmt in a single process, even when formatting multiple "
         "files. If not set, defaults to multiprocessing using as many "
         "cores as possible"
     ),
 )
 @click.option(
+    "-k",
+    "--reset-cache",
+    is_flag=True,
+    help=(
+        "Clear the sqlfmt cache before running, effectively forcing sqlfmt "
+        "to operate on every file. Will slow down runs"
+    ),
+)
+@click.option(
     "--no-jinjafmt",
     is_flag=True,
     help=(
         "Do not format jinja tags (the code between the curlies). Only necessary "
         "to specify this flag if sqlfmt was installed with the jinjafmt extra, "
         "or if black was already available in this environment"
     ),
```

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/comment.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/comment.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/config.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/config.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/dialect.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/dialect.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/exception.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/exception.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/formatter.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/formatter.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/jinjafmt.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,188 +1,211 @@
-import re
-from dataclasses import dataclass, field
-from importlib import import_module
-from types import ModuleType
-from typing import Optional
+import difflib
+from dataclasses import dataclass
+from pathlib import Path
+from typing import List, Optional
 
-from sqlfmt.line import Line
+import click
+
+from sqlfmt.exception import SqlfmtError
 from sqlfmt.mode import Mode
-from sqlfmt.node import Node
 
+STDIN_PATH = Path("-")
 
-class BlackWrapper:
-    """
-    A thin wrapper around black. Tries to import black when
-    instantiated. Provides a safe interface, format_string
+
+def style_output(
+    msg: str, fg: Optional[str] = None, bg: Optional[str] = None, bold: bool = False
+) -> str:
     """
+    A thin wrapper around click.style.
 
-    def __init__(self) -> None:
-        try:
-            self.black: Optional[ModuleType] = import_module("black")
-        except ImportError:
-            self.black = None
-
-    def format_string(self, source_string: str, max_length: int) -> str:
-        """
-        Attempt to use black to format source_string to a line_length of max_length.
-        Return source_string if black isn't installed or it can't parse source_string
-        """
-        formatted_string = source_string
-
-        if not self.black:
-            return formatted_string
-
-        black_mode = self.black.Mode(line_length=max_length)
-        try:
-            formatted_string = self.black.format_str(
-                source_string, mode=black_mode
-            ).rstrip()
-        except ValueError:
-            # the string isn't valid python.
-            # Jinja allows linebreaks where python doesn't
-            # so let's try again without newlines in the code
-            try:
-                flat_code = source_string.replace("\n", " ")
-                formatted_string = self.black.format_str(
-                    flat_code, mode=black_mode
-                ).rstrip()
-            except ValueError:
-                # there is other jinja syntax that isn't valid python,
-                # so if this still fails, just stop trying
-                pass
-        finally:
-            return formatted_string
+    See https://click.palletsprojects.com/en/8.0.x/api/?highlight=style#click.style
+    """
+    s: str = click.style(msg, fg=fg, bg=bg, bold=bold)
+    return s
 
 
-@dataclass
-class JinjaTag:
+def unstyle_output(msg: str) -> str:
+    """
+    A thin wrapper around click.unstyle.
     """
-    A simple representation of a jinja tag.
+    s: str = click.unstyle(msg)
+    return s
 
-    "verb" is one of {set, do, for, if, elif, else, test, macro}
 
-    For example, "{%- set my_var=4 %}" is split into it parts:
-    (opening_marker, verb, code, closing_marker) = ("{%-", "set", "my_var=4", "%}")
+def display_output(msg: str, err: bool = True) -> None:
     """
+    A thin wrapper around click.echo; defaults to printing to stderr.
+    """
+    click.echo(msg, err=err)
 
-    opening_marker: str
-    verb: str
-    code: str
-    closing_marker: str
-    depth: int
-
-    def __str__(self) -> str:
-        if self.is_indented_multiline_tag:
-            return self._multiline_str()
-        else:
-            s = f"{self.opening_marker} {self.verb}{self.code} {self.closing_marker}"
-            return s
 
-    @property
-    def is_indented_multiline_tag(self) -> bool:
-        return self.code != "" and self.verb == "" and "\n" in self.code
+@dataclass
+class SqlFormatResult:
+    """
+    A SqlfmtResult is a summary of the changes made by sqlfmt to a single file.
+    """
 
-    def _multiline_str(self) -> str:
-        """
-        if the formatted code is on multiple lines, and does not use a verb,
-        we want the code indented four spaces past the opening and
-        closing markers. The opening marker will already be indented to the
-        proper depth
-        """
-        indent = " " * (4 * self.depth)
-        lines = [f"{self.opening_marker}"]
-        for code_line in self.code.splitlines(keepends=False):
-            lines.append(f"{indent}    {code_line}")
-        lines.append(f"{indent}{self.closing_marker}")
-        return "\n".join(lines)
+    source_path: Path
+    source_string: str
+    formatted_string: str
+    exception: Optional[SqlfmtError] = None
+    from_cache: bool = False
 
-    @classmethod
-    def from_string(cls, source_string: str, depth: int) -> "JinjaTag":
+    def maybe_print_to_stdout(self) -> None:
         """
-        Takes a jinja statement or expression as a string and returns
-        a JinjaTag object (basically a tuple of its parts).
+        If sqlfmt received a query via stdin, print the formatted string to stdout
         """
-        opening_marker_len = 3 if source_string[2] == "-" else 2
-        opening_marker = source_string[:opening_marker_len]
-        closing_marker_len = 3 if source_string[-3] == "-" else 2
-        closing_marker = source_string[-closing_marker_len:]
-
-        verb_pattern = r"\s*(set|do|for|if|elif|else|test|macro)\s+"
-        verb_program = re.compile(verb_pattern, re.DOTALL | re.IGNORECASE)
-        verb_match = verb_program.match(source_string[opening_marker_len:])
-        if verb_match:
-            verb_pos = opening_marker_len + verb_match.span(1)[0]
-            verb_epos = opening_marker_len + verb_match.span(1)[1]
-            verb = source_string[verb_pos:verb_epos].lower()
-        else:
-            verb = ""
-        verb_len = verb_match.span(0)[1] - verb_match.span(0)[0] if verb_match else 0
+        if self.source_path == STDIN_PATH:
+            display_output(self.formatted_string, err=False)
 
-        code_pos = opening_marker_len + verb_len
-        code = source_string[code_pos:-closing_marker_len].strip()
-
-        if verb and code:
-            verb = f"{verb} "
-
-        return JinjaTag(opening_marker, verb, code, closing_marker, depth)
+    @property
+    def has_changed(self) -> bool:
+        return self.source_string != self.formatted_string
 
-    def max_code_length(self, max_length: int) -> int:
-        """
-        For a tag with max_length remaining characters on the line, return the
-        max length that the code inside the curlies (exc. the verb) can occupy.
-        """
-        return (
-            max_length
-            - len(self.opening_marker)
-            - len(self.verb)
-            - len(self.closing_marker)
-            - 2
-        )
+    @property
+    def has_error(self) -> bool:
+        return self.exception is not None
 
 
 @dataclass
-class JinjaFormatter:
+class Report:
     """
-    Provides a simple interface, format_line, to format all jinja tags
-    on a Line, using black if it is installed
+    An abstraction for a summary of results generated by a sqlfmt run.
+    Can be printed to stderr using display_report()
     """
 
+    results: List[SqlFormatResult]
     mode: Mode
-    code_formatter: BlackWrapper = field(default_factory=lambda: BlackWrapper())
 
-    def __post_init__(self) -> None:
-        self.use_black = (
-            self.code_formatter.black is not None and not self.mode.no_jinjafmt
+    def __str__(self) -> str:
+        """
+        Returns the full contents of the Report
+        """
+        report = []
+        formatted = (
+            "failed formatting check"
+            if (self.mode.check or self.mode.diff)
+            else "formatted"
+        )
+        unchanged = (
+            "passed formatting check"
+            if (self.mode.check or self.mode.diff)
+            else "left unchanged"
         )
+        if self.number_errored > 0:
+            error_msg = (
+                f"{self._pluralize_file(self.number_errored)} had errors while "
+                f"formatting."
+            )
+            report.append(style_output(error_msg, fg="red", bold=True))
+        if self.number_changed > 0:
+            changed_msg = f"{self._pluralize_file(self.number_changed)} {formatted}."
+            report.append(style_output(changed_msg, bold=True))
+        report.append(f"{self._pluralize_file(self.number_unchanged)} {unchanged}.")
+        for res in self.errored_results[0:50]:
+            err = style_output(str(res.exception), fg="red")
+            report.append(f"{res.source_path}\n    {err}")
+        if not self.mode.quiet or self.mode.diff:
+            for res in self.changed_results:
+                report.append(f"{res.source_path} {formatted}.")
+                if self.mode.diff:
+                    report.append(self._generate_diff(res))
+        if self.mode.verbose:
+            for res in self.unchanged_results:
+                report.append(f"{res.source_path} {unchanged}.")
+
+        msg = "\n".join(report)
+        if self.mode.color is False:
+            msg = unstyle_output(msg)
+        return msg
 
-    def format_line(self, line: Line) -> None:
+    @staticmethod
+    def _pluralize_file(n: int) -> str:
         """
-        Format each jinja tag in a line, in turn
+        Returns either "1 file" or "n files", depending on n
         """
-        line_length = self.mode.line_length
-        if line.contains_jinja:
-            running_length = len(line.prefix) - len(line.nodes[0].prefix)
-            for node in line.nodes:
-                self._format_jinja_node(node, max_length=line_length - running_length)
-                running_length += len(node)
+        suffix = "s" if n != 1 else ""
+        return f"{n} file{suffix}"
 
-    def _format_jinja_node(self, node: Node, max_length: int) -> None:
+    @classmethod
+    def _generate_diff(cls, result: SqlFormatResult) -> str:
         """
-        Format a single jinja tag. No-ops for nodes that
-        are not jinja
+        Returns a non-colorized diff of the source and formatted
+        strings in the SqlfmtResult
         """
-        if node.is_jinja:
-            tag = JinjaTag.from_string(node.value, node.depth[0])
-
-            if tag.code and self.use_black:
-                tag.code = self._format_python_string(
-                    tag.code,
-                    max_length=tag.max_code_length(max_length),
+        cleaned_lines = []
+        # Work around https://bugs.python.org/issue2142
+        for line in difflib.unified_diff(
+            result.source_string.splitlines(keepends=True),
+            result.formatted_string.splitlines(keepends=True),
+            fromfile="source_query",
+            tofile="formatted_query",
+        ):
+            if line[-1] == "\n":
+                cleaned_lines.append(cls._style_diff_line(line))
+            else:
+                cleaned_lines.append(cls._style_diff_line(line + "\n"))
+                cleaned_lines.append(
+                    cls._style_diff_line("\\ No newline at end of file\n")
                 )
 
-            if (not self.use_black) and tag.is_indented_multiline_tag:
-                return
-            else:
-                node.value = str(tag)
+        return "".join(cleaned_lines)
+
+    @staticmethod
+    def _style_diff_line(line: str) -> str:
+        """
+        Colorizes the diff created by _generate_diff
+        """
+        if line.startswith("@@"):
+            styled = style_output(line, fg="cyan")
+        elif line.startswith("+"):
+            styled = style_output(line, fg="green")
+        elif line.startswith("-"):
+            styled = style_output(line, fg="red")
+        else:
+            styled = line
+        return styled
+
+    def display_report(self) -> None:
+        """
+        If sqlfmt received a query via stdin, print the formatted string to stdout.
+
+        Then print the report that summarizes all results
+        """
+        if not self.mode.check and not self.mode.diff:
+            for res in self.results:
+                res.maybe_print_to_stdout()
+        display_output(str(self), err=True)
+
+    @property
+    def changed_results(self) -> List[SqlFormatResult]:
+        return self._filtered_results(has_changed=True, has_error=False)
+
+    @property
+    def unchanged_results(self) -> List[SqlFormatResult]:
+        return self._filtered_results(has_changed=False, has_error=False)
+
+    @property
+    def errored_results(self) -> List[SqlFormatResult]:
+        return self._filtered_results(has_changed=True, has_error=True)
 
-    def _format_python_string(self, source_string: str, max_length: int) -> str:
-        return self.code_formatter.format_string(source_string, max_length)
+    def _filtered_results(
+        self, has_changed: bool = True, has_error: bool = False
+    ) -> List[SqlFormatResult]:
+        filtered = [
+            r
+            for r in self.results
+            if r.has_changed == has_changed and r.has_error == has_error
+        ]
+        return sorted(filtered, key=lambda res: res.source_path)
+
+    @property
+    def number_changed(self) -> int:
+        return len(self.changed_results)
+
+    @property
+    def number_unchanged(self) -> int:
+        return len(self.unchanged_results)
+
+    @property
+    def number_errored(self) -> int:
+        return len(self.errored_results)
```

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/line.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/line.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/merger.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/merger.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/mode.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     dialect: Dialect = field(default_factory=lambda: Polyglot())
     line_length: int = 88
     check: bool = False
     diff: bool = False
     exclude: List[str] = field(default_factory=list)
     single_process: bool = False
     no_jinjafmt: bool = False
+    reset_cache: bool = False
     verbose: bool = False
     quiet: bool = False
     no_color: bool = False
     force_color: bool = False
 
     @property
     def color(self) -> bool:
```

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/node.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/node.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/query.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/query.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/splitter.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/splitter.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt/token.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt/token.py`

 * *Files identical despite different names*

### Comparing `shandy-sqlfmt-0.8.0/src/sqlfmt_primer/primer.py` & `shandy-sqlfmt-0.9.0/src/sqlfmt_primer/primer.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,36 +25,36 @@
     sub_directory: Optional[Path] = None
 
 
 def get_projects() -> List[SQLProject]:
     projects = [
         SQLProject(
             name="gitlab",
-            git_url="https://gitlab.com/gitlab-data/analytics.git",
-            git_ref="7161e509b62f53344f19de80d40db2bdba190806",  # Nov 12, 2021
-            expected_changed=1857,
-            expected_unchanged=7,
+            git_url="https://github.com/tconbeer/gitlab-analytics-sqlfmt.git",
+            git_ref="28526934a3e9215449b4ae33bb9b23a5a6f4f759",  # sqlfmt d0e14b9
+            expected_changed=13,
+            expected_unchanged=2404,
             expected_errored=0,
-            sub_directory=Path("transform/snowflake-dbt/models"),
+            sub_directory=Path("transform/snowflake-dbt/"),
         ),
         SQLProject(
             name="rittman",
-            git_url="https://github.com/rittmananalytics/ra_data_warehouse.git",
-            git_ref="ecde71faa9a4400d864ad2e484a4ac478298e53a",  # v1.2.1
-            expected_changed=212,
-            expected_unchanged=0,
+            git_url="https://github.com/tconbeer/rittman_ra_data_warehouse.git",
+            git_ref="5758cbed868c1aaa3912dc168912d7bcf7cdb4de",  # sqlfmt d0e14b9
+            expected_changed=14,
+            expected_unchanged=293,
             expected_errored=4,  # true mismatching brackets
-            sub_directory=Path("models"),
+            sub_directory=Path(""),
         ),
         SQLProject(
             name="http_archive",
-            git_url="https://github.com/HTTPArchive/almanac.httparchive.org.git",
-            git_ref="db9fd2e1405a549c96ae5091b571989f13a8a539",  # Nov 14, 2021
-            expected_changed=1631,
-            expected_unchanged=0,
+            git_url="https://github.com/tconbeer/http_archive_almanac.git",
+            git_ref="5e1b84de98cba81fa6e21f34e4defca352b980b0",  # sqlfmt 0.8.0
+            expected_changed=0,
+            expected_unchanged=1702,
             expected_errored=0,
             sub_directory=Path("sql"),
         ),
         SQLProject(
             name="aqi",
             git_url="https://github.com/tconbeer/aqi_livibility_analysis.git",
             git_ref="8004f3383897d9066e3167fdfddcdd4c8418b7ea",  # sqlfmt 0.5.0
@@ -70,19 +70,19 @@
             expected_changed=0,
             expected_unchanged=5,
             expected_errored=0,
             sub_directory=Path(""),
         ),
         SQLProject(
             name="dbt_utils",
-            git_url="https://github.com/dbt-labs/dbt-utils.git",
-            git_ref="51ed999a44fcc7f9f502be11e5f190f5bc84ba4b",  # Jan 17, 2022
-            expected_changed=113,
-            expected_unchanged=1,
-            expected_errored=1,
+            git_url="https://github.com/tconbeer/dbt-utils.git",
+            git_ref="cc17535ad47862605da51cc19777fe8736d6a886",  # sqlfmt d0e14b9
+            expected_changed=4,
+            expected_unchanged=127,
+            expected_errored=0,
             sub_directory=Path(""),
         ),
     ]
     return projects
 
 
 @click.command()
```

### Comparing `shandy-sqlfmt-0.8.0/setup.py` & `shandy-sqlfmt-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 entry_points = \
 {'console_scripts': ['sqlfmt = sqlfmt.cli:sqlfmt',
                      'sqlfmt_primer = sqlfmt_primer.primer:sqlfmt_primer']}
 
 setup_kwargs = {
     'name': 'shandy-sqlfmt',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'sqlfmt is an opinionated CLI tool that formats your sql files',
-    'long_description': '# sqlfmt\n\n![PyPI](https://img.shields.io/pypi/v/shandy-sqlfmt)\n[![Lint and Test](https://github.com/tconbeer/sqlfmt/actions/workflows/test.yml/badge.svg)](https://github.com/tconbeer/sqlfmt/actions/workflows/test.yml)\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/shandy-sqlfmt)\n![Runs on Linux | MacOS | Windows](https://img.shields.io/badge/runs%20on-Linux%20%7C%20MacOS%20%7C%20Windows-blue)\n\n\nsqlfmt formats your dbt SQL files so you don\'t have to. It is similar in nature to black, gofmt, \nand rustfmt (but for SQL). When you use sqlfmt:\n\n1. You never have to mention (or argue about) code style in code reviews again\n1. You make it easier to collaborate and solicit contributions from new people\n1. You will be able to read your team\'s code as if you wrote it\n1. You can forget about formatting your code, and spend your time on business logic instead\n\nsqlfmt is not configurable, except for line length. It enforces a single style. sqlfmt maintains comments and some extra newlines, but largely ignores all indentation and line breaks in the input file.\n\nsqlfmt is not a linter. It does not parse your code into an AST; it just lexes it and tracks a small subset of tokens that impact formatting. This lets us "do one thing and do it well:" sqlfmt is very fast, and easier to maintain and extend than linters that need a full SQL grammar.\n\nsqlfmt is designed to work with templated SQL files that contain jinja tags and blocks. It formats the code that users look at, and therefore doesn\'t need to know anything about what happens after the templates are rendered.\n\nFor now, sqlfmt only works on `select` statements (which is all you need if you use sqlfmt with a dbt project). In the future, it will be extended to DDL statements, as well.\n\n## Installation\n\n### Try it first\nWant to test out sqlfmt on a query before you install it? Go to [sqlfmt.com](http://sqlfmt.com) to use the interactive, web-based version.\n\n### Prerequisites\nYou will need Python 3.7-3.10 installed. You should use pipx or install into a virtual environment (maybe as a dev-dependency in your project). If you do not know how to install python and use pipx and/or virtual environments, go read about that first.\n\n### Install Using pipx (recommended)\n\n```\npipx install shandy-sqlfmt\n```\n\nTo install with the jinjafmt extra (which will also install the Python code formatter, *black*):\n\n```\npipx install shandy-sqlfmt[jinjafmt]\n```\n\n### Other Installation Options\nYou should use a virtual environment to isolate sqlfmt\'s dependencies from others on your system. We recommend poetry (`poetry add -D shandy-sqlfmt[jinjafmt]` or `poetry add -D shandy-sqlfmt`), or pipenv (`pipenv install -d shandy-sqlfmt[jinjafmt]`, etc.), but a simple `pip install shandy-sqlfmt` will also work.\n\n## Getting Started\n\n### Other prerequisites\n**sqlfmt is an alpha product** and will not always produce the formatted output you might want. It might even break your SQL syntax. It is **highly recommended** to only run sqlfmt on files in a version control system (like git), so that it is easy for you to revert any changes made by sqlfmt. On your first run, be sure to make a commit before running sqlfmt.\n\n### Using sqlfmt\nsqlfmt is a command-line tool. It works on any posix terminal and on Windows Powershell. If you have used `black`, the sqlfmt commands will look familiar. \n\n> Note: The `$` in the code snippets below indicate that these are commands that can be typed into your terminal. The `$` is the prompt symbol in bash; it is equivalent to `>` on Windows or `%` on zsh. Do not include the `$` in the command you type into your terminal\n\nTo list commands and options:\n\n```bash\n$ sqlfmt --help\n```\n\nIf you want to format all `.sql` and `.sql.jinja` files in your current working directory (and all nested directories), simply type:\n```bash\n$ sqlfmt .\n```\nYou can also supply a path to a one or more files or directories as arguments:\n```bash\n$ sqlfmt /path/to/my/dir /path/to/a/file.sql\n```\nIf you don\'t want to format the files you have on disk, you can run sqlfmt with the `--check` option. sqlfmt will exit with code 1 if the files on disk are not properly formatted:\n```bash\n$ sqlfmt --check .\n$ sqlfmt --check path/to/my/dir\n```\nIf you want to print a diff of changes that sqlfmt would make to format a file (but not update the file on disk), you can use the `--diff` option. `--diff` also exits with 1 on changes:\n```bash\n$ sqlfmt --diff .\n```\n\n### Disabling sqlfmt\n\nIf you would like sqlfmt to ignore a file, or part of a file, you can add `-- fmt: off` and `-- fmt: on` comments to your code (or `# fmt: off` on MySQL or BigQuery). sqlfmt will not change any code between those comments; a single `-- fmt: off` at the top of a file will keep the entire file intact.\n\n### The jinjafmt extra\n\nsqlfmt loves properly-formatted jinja, too.\n\nsqlfmt will safely attempt to import the Python code formatter, *black*. If it is successful (either because sqlfmt was installed with the **jinjafmt** extra or because black was installed separately in the same environment), it will use *black* to format the contents of jinja tags. If you do not want sqlfmt to use *black* to format your jinja, then specify the `--no-jinjafmt` flag when running sqlfmt.\n\nInstalling sqlfmt with the jinjafmt extra will also install *black*. You can do this with `pipx install sqlfmt[jinjafmt]` If you want to pin a specific *black* version, you should specify that separately, as a direct dependency of your project (in your Pipfile, pyproject.toml, etc.).\n\nIf sqlfmt was installed without the jinjafmt extra, and *black* is not otherwise installed, then sqlfmt will not attempt to format the contents of jinja tags, except for enforcing a single space inside each curly.\n\n### Configuring sqlfmt using pyproject.toml\n\nAny command-line option for sqlfmt can also be set in a `pyproject.toml` file, under a `[tool.sqlfmt]` section header. Options passed at the command line will override the settings in the config file.\n\nsqlfmt will search for the `pyproject.toml` file using the `files` passed to it as arguments. It starts in the lowest (most specific) common parent directory to all the `files` and recurses up to the root directory. It will load settings from the first `pyproject.toml` file it finds in this search.\n\nExample of a `pyproject.toml` file to override the default behaviors (run `sqlfmt --help` for more options):\n\n```\n[tool.sqlfmt]\nline_length = 100\ncheck = true\n```\n\n### Using sqlfmt with dbt\n\nsqlfmt was built for dbt, so only minimal configuration is required. We recommend excluding your `target` and `dbt_packages` directories from formatting. You can do this with the command-line `--exclude` option, or by setting `exclude` in your `pyproject.toml` file\n\n```\n[tool.sqlfmt]\nexclude=["target/**/*", "dbt_packages/**/*"]\n```\n\n### Using sqlfmt with pre-commit\nYou can configure [pre-commit](https://pre-commit.com/) to run sqlfmt on your repository before you commit changes.\n\nAdd the following config to your `.pre-commit-config.yaml` file:\n\n```\nrepos:\n  - repo: https://github.com/tconbeer/sqlfmt\n    rev: v0.7.0\n    hooks:\n      - id: sqlfmt\n        language_version: python\n```\n\nYou should replace `rev` with the latest available release, but we do suggest pinning to a specific rev, to avoid unexpected formatting changes.\n\n### Using sqlfmt with SQLFluff\n\nYou can (and should!) use SQLFluff to lint your SQL queries after they are formatted by sqlfmt. However, the two tools do not see eye-to-eye on formatting (by default), so to avoid lint errors, add the following to your `.sqlfluff` config file:\n\n```\n[sqlfluff]\nexclude_rules = L003, L018, L036\n\n[sqlfluff:rules]\nmax_line_length = 88  # or whatever you set in sqlfmt\ncapitalisation_policy = lower\nextended_capitalisation_policy = lower\n\n[sqlfluff:indentation]\nindented_joins = False\nindented_using_on = True\ntemplate_blocks_indent = False\n\n[sqlfluff:rules:L052]\nmultiline_newline = True\n```\n\n## The sqlfmt style\nThe only thing you can configure with sqlfmt is the desired line length of the formatted file. You can do this with the `--line-length` or `-l` options. The default is 88.\n\nGiven the desired line length, sqlfmt has four objectives:\n1. Break and indent lines to make the syntactical structure of the code apparent\n2. Break lines so they are shorter than the desired line length, if possible\n3. Combine lines to use the least possible vertical space, without violating #1 and #2\n4. Standardize capitalization (to lowercase) and in-line whitespace\n\nsqlfmt borrows elements from well-accepted styles from other programming languages. It places opening brackets on the same line as preceding function names (like *black* for python and *1TBS* for C). It indents closing brackets to the same depth as the opening bracket (this is extended to statements that must be closed, like `case` and `end`).\n\nThe sqlfmt style is as simple as possible, with little-to-no special-casing of formatting concerns. While at first blush, this may not create a format that is as "nice" or "expressive" as hand-crafted indentation, over time, as you grow accustomed to the style, formatting becomes transparent and the consistency will allow you to jump between files, projects, and even companies much faster.\n\n### Why lowercase?\nThere are several reasons that sqlfmt insists on lowercase SQL keywords:\n1. We believe that SQL is code (this is a surprisingly controversial statement!). Shouting-case keywords perpetuate the myth that SQL isn\'t "real code", or isn\'t "modern" and somehow is trapped in the era of low-level imperative languages: BASIC, COBOL, and FORTRAN. The reality is that SQL is an incredibly powerful, declarative, and modern language. It should look like one\n1. Syntax highlighting for SQL makes shouting-case keywords redundant; the syntax highlighter in any text editor is going to be more consistent than any manual shout-casing. If you have a SQL query as a string inside of a block of code in another language, you may want to capitalize your keywords; sqlfmt only operates on dedicated SQL (and templated sql) files, so this is not relevant. However, even without syntax highlighting, the hierarchical and consistent indentation provided by sqlfmt provides sufficient visual structure without shout-casing keywords\n1. Even among people who like shout-cased keywords, there are disagreements between what gets shout-cased. SELECT, sure, but SUM? AS? OVER? AND? All-lowercase keywords eliminates this potential source of irregularity and disagreement.\n1. Research shows that generally, lowercase words are more readable\n\n### Why trailing commas?\n1. Using trailing commas follows the convention of every other written language and programming language\n1. Leading commas require placing the first field name on the same line as `select`, which can obscure that field\n1. SQL query compilation is extremely fast; the "cost" of "last field" errors is very low. Some dialects (e.g., BigQuery) even allow a trailing comma in the final field of a select statement\n1. Trailing commas generalize better within `select` statements (e.g. `group by` and `partition by` clauses) and in other kinds of SQL statements (e.g. `insert` statements)\n\n### Examples\n\nsqlfmt will put very short queries on a single line:\n\n```sql\nSELECT a,\nb,\n   c\nFROM my_table\n```\nbecomes\n```sql\nselect a, b, c from my_table\n```\n\nIf a query doesn\'t fit on a single line, sqlfmt will format the query to make its hierarchy apparent. The main keywords in a `select` statement are the top nodes in hierarchy. Individual fields are indented a single level; unless all fields fit on the same line as `select`, they must all be individually split onto their own lines. This is properly formatted code:\n```sql\nwith t as (select * from my_schema."my_QUOTED_ table!")\nselect\n    a_long_field_name,\n    another_long_field_name,\n    (one_field + another_field) as c,\n    a_final_field\nfrom t\nwhere one_field < another_field\n```\n\nNote that the main keywords, `with`, `select`, `from`, and `where`, are indented to the same depth. If their arguments fit on a single line (as in `with`, `from`, and `where`), they stay on that line, with the keyword. However, unless all arguments for a keyword fit on one line, they are all wrapped to their own line, and indented:\n\n```sql\nwith\n    a_long_cte_name as (\n        select my_field, sum(another_field) from my_schema."my_QUOTED_ table!"\n    )\nselect\n    a_long_field_name,\n    another_long_field_name,\n    (one_field + another_field) as c,\n    a_final_field\nfrom a_long_cte_name\nwhere\n    one_field < another_field\n    and two_field > another_field\n    and three_field = another_field\n```\n\nAny expressions wrapped in parentheses are similarly one-lined if possible, and split if they are too long.\n\nThis hierarchical indentation scales to arbitrarily complex and nested expressions. Another example of properly formatted code (at line length of 88):\n\n```sql\nselect\n    a,\n    sum(a) over () as b,\n    row_number() over () as c,\n    count(case when a is null then 1 end) over (\n        partition by user_id, date_trunc(\'year\', performed_at)\n    ) as d,\n    first_value(\n        coalesce(one_field, another_field, yet_another_field) ignore nulls\n    ) over (\n        partition by user_id\n        order by performed_at desc\n        rows between unbounded preceding and unbounded following\n    ) as e\nfrom my_table\n```\nWant more examples? See the `tests/data` directory, or go to http://sqlfmt.com to see how sqlfmt will format your queries.\n\n## Contributing\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Maintainability](https://api.codeclimate.com/v1/badges/8928f6662a67b8eaf092/maintainability)](https://codeclimate.com/github/tconbeer/sqlfmt/maintainability)\n[![Test Coverage](https://api.codeclimate.com/v1/badges/8928f6662a67b8eaf092/test_coverage)](https://codeclimate.com/github/tconbeer/sqlfmt/test_coverage)\n\n### Providing Feedback\n\nWe\'d love to hear from you! [Open an Issue](https://github.com/tconbeer/sqlfmt/issues/new/choose) to request new features, report bad formatting, or say hello.\n\n### Setting up Your Dev Environment and Running Tests\n\n1. Install [Poetry](https://python-poetry.org/docs/#installation) if you don\'t have it already. You may also need or want pyenv, make, and gcc. A complete setup from a fresh install of Ubuntu can be found [here](https://github.com/tconbeer/linux_setup)\n1. Clone this repo into a directory (let\'s call it `sqlfmt`), then `cd sqlfmt`\n1. Use `poetry install -E jinjafmt` to install the project (editable) and its dependencies into a new virtual env. To run `sqlfmt_primer`, you will need to install it (and its dependencies) by specifying it as an extra: `poetry install -E jinjafmt -E sqlfmt_primer`\n1. Use `poetry shell` to spawn a subshell\n1. Type `make` to run all tests and linters, or run `pytest`, `black`, `flake8`, `isort`, and `mypy` individually.\n\nNote: If encountering a JSONDecodeError during `poetry install`, you will want to clear the poetry cache with `poetry cache clear pypi --all`, or upgrade to poetry >= 1.12 with `poetry self upgrade`\n',
+    'long_description': '# sqlfmt\n\n![PyPI](https://img.shields.io/pypi/v/shandy-sqlfmt)\n[![Lint and Test](https://github.com/tconbeer/sqlfmt/actions/workflows/test.yml/badge.svg)](https://github.com/tconbeer/sqlfmt/actions/workflows/test.yml)\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/shandy-sqlfmt)\n![Runs on Linux | MacOS | Windows](https://img.shields.io/badge/runs%20on-Linux%20%7C%20MacOS%20%7C%20Windows-blue)\n\n\nsqlfmt formats your dbt SQL files so you don\'t have to. It is similar in nature to black, gofmt, \nand rustfmt (but for SQL). When you use sqlfmt:\n\n1. You never have to mention (or argue about) code style in code reviews again\n1. You make it easier to collaborate and solicit contributions from new people\n1. You will be able to read your team\'s code as if you wrote it\n1. You can forget about formatting your code, and spend your time on business logic instead\n\nsqlfmt is not configurable, except for line length. It enforces a single style. sqlfmt maintains comments and some extra newlines, but largely ignores all indentation and line breaks in the input file.\n\nsqlfmt is not a linter. It does not parse your code into an AST; it just lexes it and tracks a small subset of tokens that impact formatting. This lets us "do one thing and do it well:" sqlfmt is very fast, and easier to maintain and extend than linters that need a full SQL grammar.\n\nsqlfmt is designed to work with templated SQL files that contain jinja tags and blocks. It formats the code that users look at, and therefore doesn\'t need to know anything about what happens after the templates are rendered.\n\nFor now, sqlfmt only works on `select` statements (which is all you need if you use sqlfmt with a dbt project). In the future, it will be extended to DDL statements, as well.\n\n## Installation\n\n### Try it first\nWant to test out sqlfmt on a query before you install it? Go to [sqlfmt.com](http://sqlfmt.com) to use the interactive, web-based version.\n\n### Prerequisites\nYou will need Python 3.7-3.10 installed. You should use pipx or install into a virtual environment (maybe as a dev-dependency in your project). If you do not know how to install python and use pipx and/or virtual environments, go read about that first.\n\n### Install Using pipx (recommended)\n\n```\npipx install shandy-sqlfmt\n```\n\nTo install with the jinjafmt extra (which will also install the Python code formatter, *black*):\n\n```\npipx install shandy-sqlfmt[jinjafmt]\n```\n\n### Other Installation Options\nYou should use a virtual environment to isolate sqlfmt\'s dependencies from others on your system. We recommend poetry (`poetry add -D shandy-sqlfmt[jinjafmt]` or `poetry add -D shandy-sqlfmt`), or pipenv (`pipenv install -d shandy-sqlfmt[jinjafmt]`, etc.), but a simple `pip install shandy-sqlfmt` will also work.\n\n## Getting Started\n\n### Other prerequisites\n**sqlfmt is an alpha product** and will not always produce the formatted output you might want. It might even break your SQL syntax. It is **highly recommended** to only run sqlfmt on files in a version control system (like git), so that it is easy for you to revert any changes made by sqlfmt. On your first run, be sure to make a commit before running sqlfmt.\n\n### Using sqlfmt\nsqlfmt is a command-line tool. It works on any posix terminal and on Windows Powershell. If you have used `black`, the sqlfmt commands will look familiar. \n\n> Note: The `$` in the code snippets below indicate that these are commands that can be typed into your terminal. The `$` is the prompt symbol in bash; it is equivalent to `>` on Windows or `%` on zsh. Do not include the `$` in the command you type into your terminal\n\nTo list commands and options:\n\n```bash\n$ sqlfmt --help\n```\n\nIf you want to format all `.sql` and `.sql.jinja` files in your current working directory (and all nested directories), simply type:\n```bash\n$ sqlfmt .\n```\nYou can also supply a path to a one or more files or directories as arguments:\n```bash\n$ sqlfmt /path/to/my/dir /path/to/a/file.sql\n```\nIf you don\'t want to format the files you have on disk, you can run sqlfmt with the `--check` option. sqlfmt will exit with code 1 if the files on disk are not properly formatted:\n```bash\n$ sqlfmt --check .\n$ sqlfmt --check path/to/my/dir\n```\nIf you want to print a diff of changes that sqlfmt would make to format a file (but not update the file on disk), you can use the `--diff` option. `--diff` also exits with 1 on changes:\n```bash\n$ sqlfmt --diff .\n```\n\n### Disabling sqlfmt\n\nIf you would like sqlfmt to ignore a file, or part of a file, you can add `-- fmt: off` and `-- fmt: on` comments to your code (or `# fmt: off` on MySQL or BigQuery). sqlfmt will not change any code between those comments; a single `-- fmt: off` at the top of a file will keep the entire file intact.\n\n### The jinjafmt extra\n\nsqlfmt loves properly-formatted jinja, too.\n\nsqlfmt will safely attempt to import the Python code formatter, *black*. If it is successful (either because sqlfmt was installed with the **jinjafmt** extra or because black was installed separately in the same environment), it will use *black* to format the contents of jinja tags. If you do not want sqlfmt to use *black* to format your jinja, then specify the `--no-jinjafmt` flag when running sqlfmt.\n\nInstalling sqlfmt with the jinjafmt extra will also install *black*. You can do this with `pipx install sqlfmt[jinjafmt]` If you want to pin a specific *black* version, you should specify that separately, as a direct dependency of your project (in your Pipfile, pyproject.toml, etc.).\n\nIf sqlfmt was installed without the jinjafmt extra, and *black* is not otherwise installed, then sqlfmt will not attempt to format the contents of jinja tags, except for enforcing a single space inside each curly.\n\n### Configuring sqlfmt using pyproject.toml\n\nAny command-line option for sqlfmt can also be set in a `pyproject.toml` file, under a `[tool.sqlfmt]` section header. Options passed at the command line will override the settings in the config file.\n\nsqlfmt will search for the `pyproject.toml` file using the `files` passed to it as arguments. It starts in the lowest (most specific) common parent directory to all the `files` and recurses up to the root directory. It will load settings from the first `pyproject.toml` file it finds in this search.\n\nExample of a `pyproject.toml` file to override the default behaviors (run `sqlfmt --help` for more options):\n\n```\n[tool.sqlfmt]\nline_length = 100\ncheck = true\n```\n\n### Using sqlfmt with dbt\n\nsqlfmt was built for dbt, so only minimal configuration is required. We recommend excluding your `target` and `dbt_packages` directories from formatting. You can do this with the command-line `--exclude` option, or by setting `exclude` in your `pyproject.toml` file\n\n```\n[tool.sqlfmt]\nexclude=["target/**/*", "dbt_packages/**/*"]\n```\n\n### Using sqlfmt with pre-commit\nYou can configure [pre-commit](https://pre-commit.com/) to run sqlfmt on your repository before you commit changes.\n\nAdd the following config to your `.pre-commit-config.yaml` file:\n\n```\nrepos:\n  - repo: https://github.com/tconbeer/sqlfmt\n    rev: v0.9.0\n    hooks:\n      - id: sqlfmt\n        language_version: python\n```\n\nYou should replace `rev` with the latest available release, but we do suggest pinning to a specific rev, to avoid unexpected formatting changes.\n\n### Using sqlfmt with SQLFluff\n\nYou can (and should!) use SQLFluff to lint your SQL queries after they are formatted by sqlfmt. However, the two tools do not see eye-to-eye on formatting (by default), so to avoid lint errors, add the following to your `.sqlfluff` config file:\n\n```\n[sqlfluff]\nexclude_rules = L003, L018, L036\n\n[sqlfluff:rules]\nmax_line_length = 88  # or whatever you set in sqlfmt\ncapitalisation_policy = lower\nextended_capitalisation_policy = lower\n\n[sqlfluff:indentation]\nindented_joins = False\nindented_using_on = True\ntemplate_blocks_indent = False\n\n[sqlfluff:rules:L052]\nmultiline_newline = True\n```\n\n## The sqlfmt style\nThe only thing you can configure with sqlfmt is the desired line length of the formatted file. You can do this with the `--line-length` or `-l` options. The default is 88.\n\nGiven the desired line length, sqlfmt has four objectives:\n1. Break and indent lines to make the syntactical structure of the code apparent\n2. Break lines so they are shorter than the desired line length, if possible\n3. Combine lines to use the least possible vertical space, without violating #1 and #2\n4. Standardize capitalization (to lowercase) and in-line whitespace\n\nsqlfmt borrows elements from well-accepted styles from other programming languages. It places opening brackets on the same line as preceding function names (like *black* for python and *1TBS* for C). It indents closing brackets to the same depth as the opening bracket (this is extended to statements that must be closed, like `case` and `end`).\n\nThe sqlfmt style is as simple as possible, with little-to-no special-casing of formatting concerns. While at first blush, this may not create a format that is as "nice" or "expressive" as hand-crafted indentation, over time, as you grow accustomed to the style, formatting becomes transparent and the consistency will allow you to jump between files, projects, and even companies much faster.\n\n### Why lowercase?\nThere are several reasons that sqlfmt insists on lowercase SQL keywords:\n1. We believe that SQL is code (this is a surprisingly controversial statement!). Shouting-case keywords perpetuate the myth that SQL isn\'t "real code", or isn\'t "modern" and somehow is trapped in the era of low-level imperative languages: BASIC, COBOL, and FORTRAN. The reality is that SQL is an incredibly powerful, declarative, and modern language. It should look like one\n1. Syntax highlighting for SQL makes shouting-case keywords redundant; the syntax highlighter in any text editor is going to be more consistent than any manual shout-casing. If you have a SQL query as a string inside of a block of code in another language, you may want to capitalize your keywords; sqlfmt only operates on dedicated SQL (and templated sql) files, so this is not relevant. However, even without syntax highlighting, the hierarchical and consistent indentation provided by sqlfmt provides sufficient visual structure without shout-casing keywords\n1. Even among people who like shout-cased keywords, there are disagreements between what gets shout-cased. SELECT, sure, but SUM? AS? OVER? AND? All-lowercase keywords eliminates this potential source of irregularity and disagreement.\n1. Research shows that generally, lowercase words are more readable\n\n### Why trailing commas?\n1. Using trailing commas follows the convention of every other written language and programming language\n1. Leading commas require placing the first field name on the same line as `select`, which can obscure that field\n1. SQL query compilation is extremely fast; the "cost" of "last field" errors is very low. Some dialects (e.g., BigQuery) even allow a trailing comma in the final field of a select statement\n1. Trailing commas generalize better within `select` statements (e.g. `group by` and `partition by` clauses) and in other kinds of SQL statements (e.g. `insert` statements)\n\n### Examples\n\nsqlfmt will put very short queries on a single line:\n\n```sql\nSELECT a,\nb,\n   c\nFROM my_table\n```\nbecomes\n```sql\nselect a, b, c from my_table\n```\n\nIf a query doesn\'t fit on a single line, sqlfmt will format the query to make its hierarchy apparent. The main keywords in a `select` statement are the top nodes in hierarchy. Individual fields are indented a single level; unless all fields fit on the same line as `select`, they must all be individually split onto their own lines. This is properly formatted code:\n```sql\nwith t as (select * from my_schema."my_QUOTED_ table!")\nselect\n    a_long_field_name,\n    another_long_field_name,\n    (one_field + another_field) as c,\n    a_final_field\nfrom t\nwhere one_field < another_field\n```\n\nNote that the main keywords, `with`, `select`, `from`, and `where`, are indented to the same depth. If their arguments fit on a single line (as in `with`, `from`, and `where`), they stay on that line, with the keyword. However, unless all arguments for a keyword fit on one line, they are all wrapped to their own line, and indented:\n\n```sql\nwith\n    a_long_cte_name as (\n        select my_field, sum(another_field) from my_schema."my_QUOTED_ table!"\n    )\nselect\n    a_long_field_name,\n    another_long_field_name,\n    (one_field + another_field) as c,\n    a_final_field\nfrom a_long_cte_name\nwhere\n    one_field < another_field\n    and two_field > another_field\n    and three_field = another_field\n```\n\nAny expressions wrapped in parentheses are similarly one-lined if possible, and split if they are too long.\n\nThis hierarchical indentation scales to arbitrarily complex and nested expressions. Another example of properly formatted code (at line length of 88):\n\n```sql\nselect\n    a,\n    sum(a) over () as b,\n    row_number() over () as c,\n    count(case when a is null then 1 end) over (\n        partition by user_id, date_trunc(\'year\', performed_at)\n    ) as d,\n    first_value(\n        coalesce(one_field, another_field, yet_another_field) ignore nulls\n    ) over (\n        partition by user_id\n        order by performed_at desc\n        rows between unbounded preceding and unbounded following\n    ) as e\nfrom my_table\n```\nWant more examples? See the `tests/data` directory, or go to http://sqlfmt.com to see how sqlfmt will format your queries.\n\n## Contributing\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Maintainability](https://api.codeclimate.com/v1/badges/8928f6662a67b8eaf092/maintainability)](https://codeclimate.com/github/tconbeer/sqlfmt/maintainability)\n[![Test Coverage](https://api.codeclimate.com/v1/badges/8928f6662a67b8eaf092/test_coverage)](https://codeclimate.com/github/tconbeer/sqlfmt/test_coverage)\n\n### Providing Feedback\n\nWe\'d love to hear from you! [Open an Issue](https://github.com/tconbeer/sqlfmt/issues/new/choose) to request new features, report bad formatting, or say hello.\n\n### Setting up Your Dev Environment and Running Tests\n\n1. Install [Poetry](https://python-poetry.org/docs/#installation) if you don\'t have it already. You may also need or want pyenv, make, and gcc. A complete setup from a fresh install of Ubuntu can be found [here](https://github.com/tconbeer/linux_setup)\n1. Clone this repo into a directory (let\'s call it `sqlfmt`), then `cd sqlfmt`\n1. Use `poetry install -E jinjafmt` to install the project (editable) and its dependencies into a new virtual env. To run `sqlfmt_primer`, you will need to install it (and its dependencies) by specifying it as an extra: `poetry install -E jinjafmt -E sqlfmt_primer`\n1. Use `poetry shell` to spawn a subshell\n1. Type `make` to run all tests and linters, or run `pytest`, `black`, `flake8`, `isort`, and `mypy` individually.\n\nNote: If encountering a JSONDecodeError during `poetry install`, you will want to clear the poetry cache with `poetry cache clear pypi --all`, or upgrade to poetry >= 1.12 with `poetry self upgrade`\n\n### Updating primer repos to reflect formatting changes\n\n1. Make sure all changes are committed to sqlfmt\n1. Check out the `unformatted` tag in the repo with `git checkout -b chore/apply-abc123 unformatted` where `abc123` is the hash of the most recent sqlfmt commit (from 1)\n1. Run sqlfmt against the working tree, then `git add .` and `git commit -m "chore: apply sqlfmt abc123"`\n1. We will have conflicts with main that we want to ignore, so merge main into this branch, ignoring anything on main: `git merge -s ours main`\n1. Push and open a PR; squash and merge. Grab the commit SHA\n1. Paste the commit SHA as a ref into `primer.py`\n1. Run `sqlfmt_primer -k` to clear the cache, then update the stats in `primer.py` to match the results',
     'author': 'Ted Conbeer',
     'author_email': 'ted@shandy.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'http://sqlfmt.com',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `shandy-sqlfmt-0.8.0/PKG-INFO` & `shandy-sqlfmt-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shandy-sqlfmt
-Version: 0.8.0
+Version: 0.9.0
 Summary: sqlfmt is an opinionated CLI tool that formats your sql files
 Home-page: http://sqlfmt.com
 License: Apache-2.0
 Author: Ted Conbeer
 Author-email: ted@shandy.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -155,15 +155,15 @@
 You can configure [pre-commit](https://pre-commit.com/) to run sqlfmt on your repository before you commit changes.
 
 Add the following config to your `.pre-commit-config.yaml` file:
 
 ```
 repos:
   - repo: https://github.com/tconbeer/sqlfmt
-    rev: v0.7.0
+    rev: v0.9.0
     hooks:
       - id: sqlfmt
         language_version: python
 ```
 
 You should replace `rev` with the latest available release, but we do suggest pinning to a specific rev, to avoid unexpected formatting changes.
 
@@ -301,7 +301,16 @@
 1. Clone this repo into a directory (let's call it `sqlfmt`), then `cd sqlfmt`
 1. Use `poetry install -E jinjafmt` to install the project (editable) and its dependencies into a new virtual env. To run `sqlfmt_primer`, you will need to install it (and its dependencies) by specifying it as an extra: `poetry install -E jinjafmt -E sqlfmt_primer`
 1. Use `poetry shell` to spawn a subshell
 1. Type `make` to run all tests and linters, or run `pytest`, `black`, `flake8`, `isort`, and `mypy` individually.
 
 Note: If encountering a JSONDecodeError during `poetry install`, you will want to clear the poetry cache with `poetry cache clear pypi --all`, or upgrade to poetry >= 1.12 with `poetry self upgrade`
 
+### Updating primer repos to reflect formatting changes
+
+1. Make sure all changes are committed to sqlfmt
+1. Check out the `unformatted` tag in the repo with `git checkout -b chore/apply-abc123 unformatted` where `abc123` is the hash of the most recent sqlfmt commit (from 1)
+1. Run sqlfmt against the working tree, then `git add .` and `git commit -m "chore: apply sqlfmt abc123"`
+1. We will have conflicts with main that we want to ignore, so merge main into this branch, ignoring anything on main: `git merge -s ours main`
+1. Push and open a PR; squash and merge. Grab the commit SHA
+1. Paste the commit SHA as a ref into `primer.py`
+1. Run `sqlfmt_primer -k` to clear the cache, then update the stats in `primer.py` to match the results
```

