# Comparing `tmp/docleaf-0.8.1-cp39-none-win_amd64.whl.zip` & `tmp/docleaf-0.8.2-cp311-cp311-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 1076462 bytes, number of entries: 10
--rw-r--r--  4.6 unx     6820 b- defN 23-Jul-03 11:09 docleaf-0.8.1.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jul-03 11:09 docleaf-0.8.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     3573 b- defN 23-Jul-03 11:09 docleaf-0.8.1.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     5450 b- defN 23-Jul-03 11:09 docleaf/copied.py
--rw-r--r--  4.6 unx     3709 b- defN 23-Jul-03 11:09 docleaf/domains.py
--rw-r--r--  4.6 unx    17707 b- defN 23-Jul-03 11:09 docleaf/doxygen.py
--rw-r--r--  4.6 unx       99 b- defN 23-Jul-03 11:09 docleaf/errors.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-03 11:09 docleaf/__init__.py
--rwxr-xr-x  4.6 unx  3032576 b- defN 23-Jul-03 11:09 docleaf/backend.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      775 b- defN 23-Jul-03 11:09 docleaf-0.8.1.dist-info/RECORD
-10 files, 3070805 bytes uncompressed, 1075156 bytes compressed:  65.0%
+Zip file size: 2584855 bytes, number of entries: 11
+-rw-r--r--  4.6 unx     6673 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/METADATA
+-rw-r--r--  4.6 unx      148 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3502 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx   137320 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/license_files/LICENSES_THIRD_PARTY.md
+-rw-r--r--  4.6 unx     3545 b- defN 23-Jul-13 15:02 docleaf/domains.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-13 15:02 docleaf/__init__.py
+-rw-r--r--  4.6 unx    17008 b- defN 23-Jul-13 15:02 docleaf/doxygen.py
+-rw-r--r--  4.6 unx     5379 b- defN 23-Jul-13 15:02 docleaf/copied.py
+-rw-r--r--  4.6 unx       93 b- defN 23-Jul-13 15:02 docleaf/errors.py
+-rwxr-xr-x  4.6 unx  7546330 b- defN 23-Jul-13 15:02 docleaf/backend.cpython-311-darwin.so
+-rw-r--r--  4.6 unx      899 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/RECORD
+11 files, 7720897 bytes uncompressed, 2583345 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
-Filename: docleaf-0.8.1.dist-info/METADATA
+Filename: docleaf-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.8.1.dist-info/WHEEL
+Filename: docleaf-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.8.1.dist-info/license_files/LICENSE.md
+Filename: docleaf-0.8.2.dist-info/license_files/LICENSE.md
 Comment: 
 
-Filename: docleaf/copied.py
+Filename: docleaf-0.8.2.dist-info/license_files/LICENSES_THIRD_PARTY.md
 Comment: 
 
 Filename: docleaf/domains.py
 Comment: 
 
+Filename: docleaf/__init__.py
+Comment: 
+
 Filename: docleaf/doxygen.py
 Comment: 
 
-Filename: docleaf/errors.py
+Filename: docleaf/copied.py
 Comment: 
 
-Filename: docleaf/__init__.py
+Filename: docleaf/errors.py
 Comment: 
 
-Filename: docleaf/backend.cp39-win_amd64.pyd
+Filename: docleaf/backend.cpython-311-darwin.so
 Comment: 
 
-Filename: docleaf-0.8.1.dist-info/RECORD
+Filename: docleaf-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docleaf/copied.py

```diff
@@ -1,132 +1,133 @@
-# This code is taken from the Breathe project. The Breathe license is below.
-#
-# Copyright (c) 2009, Michael Jones
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#  * Redistributions of source code must retain the above copyright notice,
-#    this list of conditions and the following disclaimer.
-#  * Redistributions in binary form must reproduce the above copyright notice,
-#    this list of conditions and the following disclaimer in the documentation
-#    and/or other materials provided with the distribution.
-#  * The names of its contributors may not be used to endorse or promote
-#    products derived from this software without specific prior written
-#    permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
-
-from docutils.parsers.rst.states import Text
-from docutils import nodes
-
-
-class NodeFinder(nodes.SparseNodeVisitor):
-    """Find the Docutils desc_signature declarator and desc_content nodes."""
-
-    def __init__(self, document):
-        super().__init__(document)
-        self.declarator = None
-        self.signature = None
-        self.content = None
-
-    def visit_desc_signature(self, node):
-        # Find the last signature node because it contains the actual declarator
-        # rather than "template <...>". In Sphinx 1.4.1 we'll be able to use sphinx_cpp_tagname:
-        # https://github.com/michaeljones/breathe/issues/242
-        self.declarator = node
-        self.signature = node
-
-    def visit_desc_signature_line(self, node):
-        # In sphinx 1.5, there is now a desc_signature_line node within the desc_signature
-        # This should be used instead
-        self.declarator = node
-
-    def visit_desc_content(self, node):
-        self.content = node
-        # The SparseNodeVisitor seems to not actually be universally Sparse,
-        # but only for nodes known to Docutils.
-        # So if there are extensions with new node types in the content,
-        # then the visitation will fail.
-        # We anyway don't need to visit the actual content, so skip it.
-        raise nodes.SkipChildren
-
-
-# Taken from the Breathe code base
-class InlineText(Text):
-    """
-    Add a custom docutils class to allow parsing inline text. This is to be
-    used inside a @verbatim/@endverbatim block but only the first line is
-    consumed and a inline element is generated as the parent, instead of the
-    paragraph used by Text.
-    """
-
-    patterns = {"inlinetext": r""}
-    initial_transitions = [("inlinetext",)]
-
-    def indent(self, match, context, next_state):
-        """
-        Avoid Text's indent from detecting space prefixed text and
-        doing "funny" stuff; always rely on inlinetext for parsing.
-        """
-        return self.inlinetext(match, context, next_state)
-
-    def eof(self, context):
-        """
-        Text.eof() inserts a paragraph, so override it to skip adding elements.
-        """
-        return []
-
-    def inlinetext(self, match, context, next_state):
-        """
-        Called by the StateMachine when an inline element is found (which is
-        any text when this class is added as the single transition.
-        """
-        startline = self.state_machine.abs_line_number() - 1
-        msg = None
-        try:
-            block = self.state_machine.get_text_block()
-        except UnexpectedIndentationError as err:
-            block, src, srcline = err.args
-            msg = self.reporter.error("Unexpected indentation.", source=src, line=srcline)
-        lines = context + list(block)
-        text, _ = self.inline_text(lines[0], startline)
-        self.parent += text
-        self.parent += msg
-        return [], next_state, []
-
-
-# Taken from the Breathe code base
-def nested_inline_parse_with_titles(state, content, node) -> str:
-    """
-    This code is basically a customized nested_parse_with_titles from
-    docutils, using the InlineText class on the statemachine.
-    """
-    surrounding_title_styles = state.memo.title_styles
-    surrounding_section_level = state.memo.section_level
-    state.memo.title_styles = []
-    state.memo.section_level = 0
-    try:
-        return state.nested_parse(
-            content,
-            0,
-            node,
-            match_titles=1,
-            state_machine_kwargs={
-                "state_classes": (InlineText,),
-                "initial_state": "InlineText",
-            },
-        )
-    finally:
-        state.memo.title_styles = surrounding_title_styles
-        state.memo.section_level = surrounding_section_level
+# This code is taken from the Breathe project. The Breathe license is below.
+#
+# Copyright (c) 2009, Michael Jones
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without modification,
+# are permitted provided that the following conditions are met:
+#
+#  * Redistributions of source code must retain the above copyright notice,
+#    this list of conditions and the following disclaimer.
+#  * Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#  * The names of its contributors may not be used to endorse or promote
+#    products derived from this software without specific prior written
+#    permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+#
+
+from docutils.statemachine import UnexpectedIndentationError
+from docutils.parsers.rst.states import Text
+from docutils import nodes
+
+
+class NodeFinder(nodes.SparseNodeVisitor):
+    """Find the Docutils desc_signature declarator and desc_content nodes."""
+
+    def __init__(self, document):
+        super().__init__(document)
+        self.declarator = None
+        self.signature = None
+        self.content = None
+
+    def visit_desc_signature(self, node):
+        # Find the last signature node because it contains the actual declarator
+        # rather than "template <...>". In Sphinx 1.4.1 we'll be able to use sphinx_cpp_tagname:
+        # https://github.com/michaeljones/breathe/issues/242
+        self.declarator = node
+        self.signature = node
+
+    def visit_desc_signature_line(self, node):
+        # In sphinx 1.5, there is now a desc_signature_line node within the desc_signature
+        # This should be used instead
+        self.declarator = node
+
+    def visit_desc_content(self, node):
+        self.content = node
+        # The SparseNodeVisitor seems to not actually be universally Sparse,
+        # but only for nodes known to Docutils.
+        # So if there are extensions with new node types in the content,
+        # then the visitation will fail.
+        # We anyway don't need to visit the actual content, so skip it.
+        raise nodes.SkipChildren
+
+
+# Taken from the Breathe code base
+class InlineText(Text):
+    """
+    Add a custom docutils class to allow parsing inline text. This is to be
+    used inside a @verbatim/@endverbatim block but only the first line is
+    consumed and a inline element is generated as the parent, instead of the
+    paragraph used by Text.
+    """
+
+    patterns = {"inlinetext": r""}
+    initial_transitions = [("inlinetext",)]
+
+    def indent(self, match, context, next_state):
+        """
+        Avoid Text's indent from detecting space prefixed text and
+        doing "funny" stuff; always rely on inlinetext for parsing.
+        """
+        return self.inlinetext(match, context, next_state)
+
+    def eof(self, context):
+        """
+        Text.eof() inserts a paragraph, so override it to skip adding elements.
+        """
+        return []
+
+    def inlinetext(self, match, context, next_state):
+        """
+        Called by the StateMachine when an inline element is found (which is
+        any text when this class is added as the single transition.
+        """
+        startline = self.state_machine.abs_line_number() - 1
+        msg = None
+        try:
+            block = self.state_machine.get_text_block()
+        except UnexpectedIndentationError as err:
+            block, src, srcline = err.args
+            msg = self.reporter.error("Unexpected indentation.", source=src, line=srcline)
+        lines = context + list(block)
+        text, _ = self.inline_text(lines[0], startline)
+        self.parent += text
+        self.parent += msg
+        return [], next_state, []
+
+
+# Taken from the Breathe code base
+def nested_inline_parse_with_titles(state, content, node) -> str:
+    """
+    This code is basically a customized nested_parse_with_titles from
+    docutils, using the InlineText class on the statemachine.
+    """
+    surrounding_title_styles = state.memo.title_styles
+    surrounding_section_level = state.memo.section_level
+    state.memo.title_styles = []
+    state.memo.section_level = 0
+    try:
+        return state.nested_parse(
+            content,
+            0,
+            node,
+            match_titles=1,
+            state_machine_kwargs={
+                "state_classes": (InlineText,),
+                "initial_state": "InlineText",
+            },
+        )
+    finally:
+        state.memo.title_styles = surrounding_title_styles
+        state.memo.section_level = surrounding_section_level
```

## docleaf/domains.py

```diff
@@ -1,117 +1,114 @@
-import logging
-
-from sphinx.domains import cpp, c
-from docutils import nodes
-
-from . import copied
-from .errors import DocleafError
-
-
-def null_handler(finder, location):
-    return
-
-
-def strip_desc_addname(finder, location):
-    # We pass qualified values to the domain directives but we don't always want Sphinx to show the qualified part
-    # in the output as normally it is shown but the nesting of the entities so we strip it out which involes removing
-    # the 'desc_addname' node in the output
-    finder.declarator.children = [
-        node for node in finder.declarator.children if node.tagname != "desc_addname"
-    ]
-
-
-def add_location_via_names(finder, location):
-    if finder.signature and location:
-        finder.signature["names"] = f"{location['path']}:{location['line']}"
-
-
-def chain(*funcs):
-    def inner(finder, location):
-        for func in funcs:
-            func(finder, location)
-
-    return inner
-
-
-cpp_domain = {
-    "class": (cpp.CPPClassObject, "class", add_location_via_names),
-    "enum": (cpp.CPPEnumObject, "enum", add_location_via_names),
-    "enumerator": (
-        cpp.CPPEnumeratorObject,
-        "enumerator",
-        chain(strip_desc_addname, add_location_via_names),
-    ),
-    "function": (
-        cpp.CPPFunctionObject,
-        "function",
-        chain(strip_desc_addname, add_location_via_names),
-    ),
-    "member": (cpp.CPPMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
-    "struct": (cpp.CPPClassObject, "struct", add_location_via_names),
-}
-
-c_domain = {
-    "define": (c.CMacroObject, "macro", add_location_via_names),
-    "enum": (c.CEnumObject, "enum", add_location_via_names),
-    "enumerator": (
-        c.CEnumeratorObject,
-        "enumerator",
-        chain(strip_desc_addname, add_location_via_names),
-    ),
-    "function": (c.CFunctionObject, "function", add_location_via_names),
-    "member": (c.CMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
-    "struct": (c.CStructObject, "struct", add_location_via_names),
-    "typedef": (c.CTypeObject, "type", add_location_via_names),
-    "union": (c.CUnionObject, "union", chain(strip_desc_addname, add_location_via_names)),
-}
-
-domains = {"cpp": cpp_domain, "c": c_domain}
-
-
-def render_domain_entry(
-    domain_name: str,
-    type: str,
-    declaration: str,
-    location,
-    target,
-    directive_args: list,
-    content: list,
-):
-    # print("render_domain_entry", domain_name, type, declaration)
-    try:
-        domain = domains[domain_name]
-    except KeyError:
-        raise DocleafError(f"Unsupported domain: {domain_name}")
-
-    try:
-        (Directive, domain_specific_type, handler) = domain[type]
-    except KeyError:
-        raise DocleafError(f'Unsupported type "{type}" on domain "{domain_name}"')
-
-    directive_name = f"{domain_name}:{domain_specific_type}"
-
-    args = [directive_name, [declaration]] + directive_args[2:]
-    directive = Directive(*args)
-
-    nodes = directive.run()
-
-    rst_node = nodes[1]
-    finder = copied.NodeFinder(rst_node.document)
-    rst_node.walk(finder)
-
-    set_children(finder.content, content)
-    finder.declarator.children.insert(0, target)
-
-    handler(finder, location)
-
-    return nodes
-
-
-def set_children(node, children):
-    """
-    The children have to be informed of the parent and that happens in the parents helper methods like 'append' and
-    'extend' so we can't just replace 'node.children' with 'children'. Instead we empty the children list and then
-    add the children so they are set up properly.
-    """
-    node.children.clear()
-    node.extend(children)
+from sphinx.domains import cpp, c
+
+from . import copied
+from .errors import DocleafError
+
+
+def null_handler(finder, location):
+    return
+
+
+def strip_desc_addname(finder, location):
+    # We pass qualified values to the domain directives but we don't always want Sphinx
+    # to show the qualified part in the output as normally it is shown but the nesting
+    # of the entities so we strip it out which involes removing the 'desc_addname' node
+    # in the output
+    finder.declarator.children = [node for node in finder.declarator.children if node.tagname != "desc_addname"]
+
+
+def add_location_via_names(finder, location):
+    if finder.signature and location:
+        finder.signature["names"] = f"{location['path']}:{location['line']}"
+
+
+def chain(*funcs):
+    def inner(finder, location):
+        for func in funcs:
+            func(finder, location)
+
+    return inner
+
+
+cpp_domain = {
+    "class": (cpp.CPPClassObject, "class", add_location_via_names),
+    "enum": (cpp.CPPEnumObject, "enum", add_location_via_names),
+    "enumerator": (
+        cpp.CPPEnumeratorObject,
+        "enumerator",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "function": (
+        cpp.CPPFunctionObject,
+        "function",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "member": (cpp.CPPMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
+    "struct": (cpp.CPPClassObject, "struct", add_location_via_names),
+}
+
+c_domain = {
+    "define": (c.CMacroObject, "macro", add_location_via_names),
+    "enum": (c.CEnumObject, "enum", add_location_via_names),
+    "enumerator": (
+        c.CEnumeratorObject,
+        "enumerator",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "function": (c.CFunctionObject, "function", add_location_via_names),
+    "member": (c.CMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
+    "struct": (c.CStructObject, "struct", add_location_via_names),
+    "typedef": (c.CTypeObject, "type", add_location_via_names),
+    "union": (c.CUnionObject, "union", chain(strip_desc_addname, add_location_via_names)),
+}
+
+domains = {"cpp": cpp_domain, "c": c_domain}
+
+
+def render_domain_entry(
+    domain_name: str,
+    type: str,
+    declaration: str,
+    location,
+    target,
+    directive_args: list,
+    content: list,
+):
+    # print("render_domain_entry", domain_name, type, declaration)
+    try:
+        domain = domains[domain_name]
+    except KeyError:
+        raise DocleafError(f"Unsupported domain: {domain_name}")
+
+    try:
+        (Directive, domain_specific_type, handler) = domain[type]
+    except KeyError:
+        raise DocleafError(f'Unsupported type "{type}" on domain "{domain_name}"')
+
+    directive_name = f"{domain_name}:{domain_specific_type}"
+
+    args = [directive_name, [declaration]] + directive_args[2:]
+    directive = Directive(*args)
+
+    nodes = directive.run()
+
+    rst_node = nodes[1]
+    finder = copied.NodeFinder(rst_node.document)
+    rst_node.walk(finder)
+
+    set_children(finder.content, content)
+    finder.declarator.children.insert(0, target)
+
+    handler(finder, location)
+
+    return nodes
+
+
+def set_children(node, children):
+    """
+    The children have to be informed of the parent and that happens in the parents
+    helper methods like 'append' and 'extend' so we can't just replace 'node.children'
+    with 'children'. Instead we empty the children list and then add the children so
+    they are set up properly.
+    """
+    node.children.clear()
+    node.extend(children)
```

## docleaf/doxygen.py

```diff
@@ -1,503 +1,498 @@
-from typing import List
-from collections import defaultdict
-from pathlib import Path
-import itertools
-import textwrap
-import hashlib
-import pprint
-import time
-import sys
-import os
-
-from docutils.nodes import Node
-from docutils.parsers.rst.directives import unchanged_required, unchanged, flag
-from docutils.parsers.rst.states import Text
-from docutils.parsers.rst import Directive, directives
-from docutils.statemachine import StringList
-from docutils import nodes
-
-from sphinx.application import Sphinx
-from sphinx.environment import BuildEnvironment
-from sphinx.util.nodes import nested_parse_with_titles
-from sphinx.domains import c
-from sphinx.util import logging
-import sphinx.addnodes
-
-from . import backend, domains, copied
-from .errors import DocleafError
-
-__version__ = "0.0.0"
-
-logger = logging.getLogger(__name__)
-
-
-class GitHubLinkResolver:
-    """
-    This works on the assumption that we can insert our own data into the 'names' field of desc_signature nodes in
-    domain entries. That assumption might fail or clash with other things so we try to be careful when extracting the
-    data from 'names' and fail early and quietly.
-    """
-
-    def __init__(self, *, root, user, repo, tag=None, branch=None, revision=None):
-        self.root = Path(root).resolve()
-        self.user = user
-        self.repo = repo
-        self.tag = tag
-        self.branch = branch
-        self.revision = revision
-
-    def __call__(self, domain, info):
-        if domain not in ["c", "cpp"]:
-            return None
-
-        names = info.get("names")
-        if not names:
-            return None
-
-        entries = names.rsplit(":", 1)
-        if len(entries) != 2:
-            return None
-
-        path = Path(entries[0]).resolve()
-        relative = path.relative_to(self.root)
-
-        try:
-            line = int(entries[1])
-        except ValueError:
-            # Unable to get line number - exit quietly
-            return None
-
-        reference = self.tag or self.branch or self.revision
-        if not reference:
-            return None
-
-        return f"https://github.com/{self.user}/{self.repo}/blob/{reference}/{relative}#L{line}"
-
-
-def as_list(node):
-    def wrapper(*children, **attributes):
-        return [node(*children, **attributes)]
-
-    return wrapper
-
-
-class NodeManager:
-    def __init__(self, state, directive_arguments):
-        self.state = state
-        self.directive_arguments = directive_arguments
-        self.lookup = {
-            "bullet_list": as_list(nodes.bullet_list),
-            "container": as_list(nodes.container),
-            "colspec": as_list(nodes.colspec),
-            "desc": as_list(sphinx.addnodes.desc),
-            "desc_content": as_list(sphinx.addnodes.desc_content),
-            "desc_name": as_list(sphinx.addnodes.desc_name),
-            "desc_parameter": as_list(sphinx.addnodes.desc_parameter),
-            "desc_parameterlist": as_list(sphinx.addnodes.desc_parameterlist),
-            "desc_sig_keyword": as_list(sphinx.addnodes.desc_sig_keyword),
-            "desc_sig_name": as_list(sphinx.addnodes.desc_sig_name),
-            "desc_sig_space": as_list(sphinx.addnodes.desc_sig_space),
-            "desc_signature": as_list(sphinx.addnodes.desc_signature),
-            "desc_signature_line": as_list(sphinx.addnodes.desc_signature_line),
-            "emphasis": as_list(nodes.emphasis),
-            "entry": as_list(nodes.entry),
-            "enumerated_list": as_list(nodes.enumerated_list),
-            "field_list": as_list(nodes.field_list),
-            "field": as_list(nodes.field),
-            "field_name": as_list(nodes.field_name),
-            "field_body": as_list(nodes.field_body),
-            "index": as_list(sphinx.addnodes.index),
-            "inline": as_list(nodes.inline),
-            "list_item": as_list(nodes.list_item),
-            "literal": as_list(nodes.literal),
-            "literal_block": as_list(nodes.literal_block),
-            "literal_strong": as_list(sphinx.addnodes.literal_strong),
-            "note": as_list(nodes.note),
-            "only": as_list(sphinx.addnodes.only),
-            "paragraph": as_list(nodes.paragraph),
-            "raw": as_list(nodes.raw),
-            "internal_reference": self.build_internal_reference,
-            "external_reference": as_list(nodes.reference),
-            "restructured_text_block": self.build_restructured_text_block,
-            "restructured_text_inline": self.build_restructured_text_inline,
-            "row": as_list(nodes.row),
-            "rubric": as_list(nodes.rubric),
-            "strong": as_list(nodes.strong),
-            "see_also": as_list(sphinx.addnodes.seealso),
-            "table": as_list(nodes.table),
-            "tbody": as_list(nodes.tbody),
-            "tgroup": as_list(nodes.tgroup),
-            "thead": as_list(nodes.thead),
-            "warning": as_list(nodes.warning),
-            # Special
-            "target": as_list(self.build_target),
-            "domain_entry": self.build_domain_entry,
-        }
-
-    def get_builder(self, node_type):
-        builder = self.lookup[node_type]
-        return builder
-
-    def build_target(self, *children, **attributes):
-        target = nodes.target(*children, **attributes)
-        self.state.document.note_explicit_target(target)
-        return target
-
-    def build_domain_entry(self, *children, **attributes):
-        return domains.render_domain_entry(
-            attributes["domain"],
-            attributes["type"],
-            attributes["declaration"],
-            attributes.get("location"),
-            self.build_target(**attributes["target"]),
-            self.directive_arguments,
-            children,
-        )
-
-    def build_internal_reference(self, *children, **attributes):
-        reference = sphinx.addnodes.pending_xref(
-            "",
-            *children,
-            reftype="ref",
-            refdomain="std",
-            refexplicit=True,
-            refid=attributes["refid"],
-            reftarget=attributes["refid"],
-        )
-        return [reference]
-
-    def build_restructured_text_block(self, *children, **attributes):
-        text = textwrap.dedent(children[0])
-
-        # Inspired by autodoc.py in Sphinx
-        rst = StringList()
-        for line in text.split("\n"):
-            rst.append(line, "<docleaf>")
-
-        # Parent node for the generated node subtree
-        rst_node = nodes.paragraph()
-        rst_node.document = self.state.document
-
-        nested_parse_with_titles(self.state, rst, rst_node)
-
-        # We render the block into a paragraph node but the rendred block will contain
-        # its own paragraph nodes at the top level so we don't need to return our
-        # paragraph node so we return its children (the top layer of rendered nodes) as
-        # the output
-        return rst_node.children
-
-    def build_restructured_text_inline(self, *children, **attributes):
-        text = children[0]
-
-        # Inspired by autodoc.py in Sphinx
-        rst = StringList()
-        for line in text.split("\n"):
-            rst.append(line, "<docleaf>")
-
-        rst_node = nodes.inline()
-        rst_node.document = self.state.document
-
-        copied.nested_inline_parse_with_titles(self.state, rst, rst_node)
-
-        return [rst_node]
-
-
-def render_node_list(node_list, node_manager):
-    # Use nested comprehension to flatten nodes lists coming back from render_node
-    return flatten(render_node(node, node_manager) for node in node_list)
-
-
-def flatten(list_of_lists):
-    return list(itertools.chain.from_iterable(list_of_lists))
-
-
-def render_node(node, node_manager):
-    if node.type == "text":
-        return [nodes.Text(node.text)]
-
-    node_builder = node_manager.get_builder(node.type)
-    children = render_node_list(node.children, node_manager)
-
-    if node.call_as == "text-element":
-        return node_builder("", "", *children, **node.attributes)
-    elif node.call_as == "element":
-        return node_builder("", *children, **node.attributes)
-    elif node.call_as == "function":
-        return node_builder(*children, **node.attributes)
-    else:
-        raise DocleafError("Call As not implemented: " + node.call_as)
-
-
-class Project:
-    def __init__(self, root, xml):
-        self._root = root
-        self._xml = xml
-
-    def root(self):
-        return self._root
-
-    def xml(self):
-        return self._xml
-
-    def get(projects, name: str):
-        # For each 'try' block we need to catch KeyError and TypeError (if project is a string) so we catch everything
-        # as there isn't much else that could go wrong
-
-        try:
-            data = projects[name]
-        except Exception:
-            raise DocleafError(
-                f"Unable to find a project called '{name}' defined in the docleaf_projects config variable"
-            )
-
-        try:
-            root = data["root"]
-        except Exception:
-            raise DocleafError(
-                f"Unable to find the 'root' entry in the data for '{name}' project defined in the docleaf_projects config variable"
-            )
-
-        try:
-            xml = data["xml"]
-        except Exception:
-            raise DocleafError(
-                f"Unable to find the 'xml' entry in the data for '{name}' project defined in the docleaf_projects config variable"
-            )
-
-        return Project(root, xml)
-
-
-class BaseDirective(Directive):
-    def get_directive_args(self) -> list:
-        # Must match order in docutils.parsers.rst.Directive.__init__
-        return [
-            self.name,
-            self.arguments,
-            self.options,
-            self.content,
-            self.lineno,
-            self.content_offset,
-            self.block_text,
-            self.state,
-            self.state_machine,
-        ]
-
-
-class BasicDoxygenDirective(BaseDirective):
-    has_content = True
-    required_arguments = 1
-    optional_arguments = 0
-    final_argument_whitespace = True
-    option_spec = {
-        "project": directives.unchanged,
-        "skip-xml-nodes": directives.unchanged,
-    }
-
-    def run(self) -> List[Node]:
-        name = self.arguments[0]
-        project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = Project.get(self.app.config.docleaf_projects, project_name)
-        skip_settings = get_skip_settings(self.app, self.options)
-
-        context = backend.Context(
-            project.root(),
-            skip_settings,
-            self.app.config.docleaf_domain_by_extension,
-        )
-
-        tracked_cache = backend.TrackedCache(self.cache)
-        node_list = self.render_function(name, project.xml(), context, tracked_cache)
-        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
-
-        node_builder = NodeManager(self.state, self.get_directive_args())
-        return render_node_list(node_list, node_builder)
-
-
-class ClassDirective(BasicDoxygenDirective):
-    render_function = backend.render_class
-
-
-class StructDirective(BasicDoxygenDirective):
-    render_function = backend.render_struct
-
-
-class EnumDirective(BasicDoxygenDirective):
-    render_function = backend.render_enum
-
-
-class FunctionDirective(BasicDoxygenDirective):
-    render_function = backend.render_function
-
-
-class GroupDirective(BaseDirective):
-    has_content = True
-    required_arguments = 1
-    optional_arguments = 0
-    final_argument_whitespace = True
-    option_spec = {
-        "project": directives.unchanged,
-        "content-only": directives.flag,  # TODO: Implement
-        "inner": directives.flag,  # TODO: Implement
-        "skip-xml-nodes": directives.unchanged,
-    }
-
-    def run(self) -> List[Node]:
-        name = self.arguments[0]
-        project_name = self.options.get("project", self.app.config.docleaf_default_project)
-        project = Project.get(self.app.config.docleaf_projects, project_name)
-
-        skip_settings = get_skip_settings(self.app, self.options)
-        content_only = "content-only" in self.options
-        inner_group = "inner" in self.options
-        context = backend.Context(
-            project.root(),
-            skip_settings,
-            self.app.config.docleaf_domain_by_extension,
-        )
-
-        tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_group(
-            name,
-            project.xml(),
-            context,
-            content_only,
-            inner_group,
-            tracked_cache,
-        )
-        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
-
-        node_builder = NodeManager(self.state, self.get_directive_args())
-        return render_node_list(node_list, node_builder)
-
-
-def get_skip_settings(app, options):
-    """
-    Get the option for the directive and fallback to the app option if not defined on the directive
-    """
-    skip_settings = options.get("skip", None)
-    if skip_settings is None:
-        skip_settings = app.config.docleaf_doxygen_skip
-    else:
-        skip_settings = skip_settings.split(",")
-    return skip_settings
-
-
-class XmlFileInfo:
-    def __init__(self, hash, rst_files):
-        self.hash = hash
-        self.rst_files = rst_files
-
-
-def hash_file(path):
-    logger.debug(f"docleaf: hashing {path}")
-    if sys.version_info >= (3, 11):
-        with open(path, "rb") as f:
-            digest = hashlib.file_digest(f, "sha1")
-            return digest.hexdigest()
-    else:
-        contents = open(path, "rb").read()
-        hash = hashlib.sha1()
-        hash.update(contents)
-        return hash.hexdigest()
-
-
-def update_sphinx_env_file_data(env: BuildEnvironment, xml_paths: List[str], rst_file: str):
-    """
-    Update our file_data store to indicate which rst files are dependent on which xml files
-    """
-    if not hasattr(env, "docleaf_file_data"):
-        env.docleaf_file_data = {}
-
-    for path in xml_paths:
-        if path in env.docleaf_file_data:
-            env.docleaf_file_data[path].rst_files.add(rst_file)
-        else:
-            env.docleaf_file_data[path] = XmlFileInfo(hash_file(path), set([rst_file]))
-
-
-def calculate_files_to_refresh(app: Sphinx, env, added, changed, removed):
-    """
-    Sphinx tells us which rst files have changed on disk and we can tell it (by returning a list of doc names) which
-    documents need to be re-read and have their output re-generated.
-
-    We calculate which files to refresh by storing the last build time and comparing the modified time of each xml file
-    against the last build time and see if any are newer. From there we need to get from the xml files to the rst files
-    that they impact and return those rst files to be refreshed.
-    """
-    logger.debug("docleaf: calculate_files_to_refresh")
-
-    # Get the last build time before updating it
-    last_build_time = getattr(app.env, "docleaf_last_build_time", None)
-
-    # Store the current time as the build time
-    app.env.docleaf_last_build_time = time.time()
-
-    if not last_build_time:
-        return []
-
-    if not hasattr(app.env, "docleaf_file_data"):
-        return []
-
-    rst_files_to_refresh = set()
-
-    for xml_file_path, info in app.env.docleaf_file_data.items():
-        stat = os.stat(xml_file_path)
-        if stat.st_mtime > last_build_time:
-            hash = hash_file(xml_file_path)
-            logger.debug(
-                f"docleaf: stored hash for {xml_file_path} = {hash}. Calculated hash: {info.hash}"
-            )
-            if hash != info.hash:
-                # Store the new hash
-                info.hash = hash
-                # Tell Sphinx to refresh all rst files associated with this file
-                rst_files_to_refresh.update(info.rst_files)
-
-    logger.verbose(f"docleaf: calculate_files_to_refresh - Rebuild: {rst_files_to_refresh}")
-    return rst_files_to_refresh
-
-
-def purge_file_data(app, env, docname):
-    """
-    Clear any file data associated with 'docname' in accordance with the Sphinx API
-    """
-    logger.debug("docleaf: purge_file_data - %s", docname)
-    if not hasattr(app.env, "docleaf_file_data"):
-        return
-
-    for xml_file_path, info in app.env.docleaf_file_data.items():
-        info.rst_files.discard(docname)
-
-
-class ExtensionContext:
-    def __init__(self, app: Sphinx, cache):
-        self.app = app
-        self.cache = cache
-
-
-def add_directive(context, name, Cls):
-    Cls.app = context.app
-    Cls.cache = context.cache
-    context.app.add_directive(name, Cls)
-
-
-def setup(app: Sphinx):
-    cache = backend.FileCache()
-
-    context = ExtensionContext(app, cache)
-
-    add_directive(context, "doxygenclass", ClassDirective)
-    add_directive(context, "doxygenenum", EnumDirective)
-    add_directive(context, "doxygenfunction", FunctionDirective)
-    add_directive(context, "doxygengroup", GroupDirective)
-    add_directive(context, "doxygenstruct", StructDirective)
-
-    app.add_config_value("docleaf_projects", {}, "env")
-    app.add_config_value("docleaf_default_project", None, "env")
-    app.add_config_value("docleaf_doxygen_skip", [], "env")
-    app.add_config_value("docleaf_domain_by_extension", {}, True)
-
-    app.connect("env-get-outdated", calculate_files_to_refresh)
-    app.connect("env-purge-doc", purge_file_data)
-
-    return {"version": __version__, "parallel_read_safe": True, "parallel_write_safe": True}
+from typing import List
+from pathlib import Path
+import itertools
+import textwrap
+import hashlib
+import time
+import sys
+import os
+
+from docutils.nodes import Node
+from docutils.parsers.rst import Directive, directives
+from docutils.statemachine import StringList
+from docutils import nodes
+
+from sphinx.application import Sphinx
+from sphinx.environment import BuildEnvironment
+from sphinx.util.nodes import nested_parse_with_titles
+from sphinx.util import logging
+import sphinx.addnodes
+
+from . import backend, domains, copied
+from .errors import DocleafError
+
+__version__ = "0.0.0"
+
+logger = logging.getLogger(__name__)
+
+
+class GitHubLinkResolver:
+    """
+    This works on the assumption that we can insert our own data into the 'names' field of desc_signature nodes in
+    domain entries. That assumption might fail or clash with other things so we try to be careful when extracting the
+    data from 'names' and fail early and quietly.
+    """
+
+    def __init__(self, *, root, user, repo, tag=None, branch=None, revision=None):
+        self.root = Path(root).resolve()
+        self.user = user
+        self.repo = repo
+        self.tag = tag
+        self.branch = branch
+        self.revision = revision
+
+    def __call__(self, domain, info):
+        if domain not in ["c", "cpp"]:
+            return None
+
+        names = info.get("names")
+        if not names:
+            return None
+
+        entries = names.rsplit(":", 1)
+        if len(entries) != 2:
+            return None
+
+        path = Path(entries[0]).resolve()
+        relative = path.relative_to(self.root)
+
+        try:
+            line = int(entries[1])
+        except ValueError:
+            # Unable to get line number - exit quietly
+            return None
+
+        reference = self.tag or self.branch or self.revision
+        if not reference:
+            return None
+
+        return f"https://github.com/{self.user}/{self.repo}/blob/{reference}/{relative}#L{line}"
+
+
+def as_list(node):
+    def wrapper(*children, **attributes):
+        return [node(*children, **attributes)]
+
+    return wrapper
+
+
+class NodeManager:
+    def __init__(self, state, directive_arguments):
+        self.state = state
+        self.directive_arguments = directive_arguments
+        self.lookup = {
+            "bullet_list": as_list(nodes.bullet_list),
+            "container": as_list(nodes.container),
+            "colspec": as_list(nodes.colspec),
+            "desc": as_list(sphinx.addnodes.desc),
+            "desc_content": as_list(sphinx.addnodes.desc_content),
+            "desc_name": as_list(sphinx.addnodes.desc_name),
+            "desc_parameter": as_list(sphinx.addnodes.desc_parameter),
+            "desc_parameterlist": as_list(sphinx.addnodes.desc_parameterlist),
+            "desc_sig_keyword": as_list(sphinx.addnodes.desc_sig_keyword),
+            "desc_sig_name": as_list(sphinx.addnodes.desc_sig_name),
+            "desc_sig_space": as_list(sphinx.addnodes.desc_sig_space),
+            "desc_signature": as_list(sphinx.addnodes.desc_signature),
+            "desc_signature_line": as_list(sphinx.addnodes.desc_signature_line),
+            "emphasis": as_list(nodes.emphasis),
+            "entry": as_list(nodes.entry),
+            "enumerated_list": as_list(nodes.enumerated_list),
+            "field_list": as_list(nodes.field_list),
+            "field": as_list(nodes.field),
+            "field_name": as_list(nodes.field_name),
+            "field_body": as_list(nodes.field_body),
+            "index": as_list(sphinx.addnodes.index),
+            "inline": as_list(nodes.inline),
+            "list_item": as_list(nodes.list_item),
+            "literal": as_list(nodes.literal),
+            "literal_block": as_list(nodes.literal_block),
+            "literal_strong": as_list(sphinx.addnodes.literal_strong),
+            "note": as_list(nodes.note),
+            "only": as_list(sphinx.addnodes.only),
+            "paragraph": as_list(nodes.paragraph),
+            "raw": as_list(nodes.raw),
+            "internal_reference": self.build_internal_reference,
+            "external_reference": as_list(nodes.reference),
+            "restructured_text_block": self.build_restructured_text_block,
+            "restructured_text_inline": self.build_restructured_text_inline,
+            "row": as_list(nodes.row),
+            "rubric": as_list(nodes.rubric),
+            "strong": as_list(nodes.strong),
+            "see_also": as_list(sphinx.addnodes.seealso),
+            "table": as_list(nodes.table),
+            "tbody": as_list(nodes.tbody),
+            "tgroup": as_list(nodes.tgroup),
+            "thead": as_list(nodes.thead),
+            "warning": as_list(nodes.warning),
+            # Special
+            "target": as_list(self.build_target),
+            "domain_entry": self.build_domain_entry,
+        }
+
+    def get_builder(self, node_type):
+        builder = self.lookup[node_type]
+        return builder
+
+    def build_target(self, *children, **attributes):
+        target = nodes.target(*children, **attributes)
+        self.state.document.note_explicit_target(target)
+        return target
+
+    def build_domain_entry(self, *children, **attributes):
+        return domains.render_domain_entry(
+            attributes["domain"],
+            attributes["type"],
+            attributes["declaration"],
+            attributes.get("location"),
+            self.build_target(**attributes["target"]),
+            self.directive_arguments,
+            children,
+        )
+
+    def build_internal_reference(self, *children, **attributes):
+        reference = sphinx.addnodes.pending_xref(
+            "",
+            *children,
+            reftype="ref",
+            refdomain="std",
+            refexplicit=True,
+            refid=attributes["refid"],
+            reftarget=attributes["refid"],
+        )
+        return [reference]
+
+    def build_restructured_text_block(self, *children, **attributes):
+        text = textwrap.dedent(children[0])
+
+        # Inspired by autodoc.py in Sphinx
+        rst = StringList()
+        for line in text.split("\n"):
+            rst.append(line, "<docleaf>")
+
+        # Parent node for the generated node subtree
+        rst_node = nodes.paragraph()
+        rst_node.document = self.state.document
+
+        nested_parse_with_titles(self.state, rst, rst_node)
+
+        # We render the block into a paragraph node but the rendred block will contain
+        # its own paragraph nodes at the top level so we don't need to return our
+        # paragraph node so we return its children (the top layer of rendered nodes) as
+        # the output
+        return rst_node.children
+
+    def build_restructured_text_inline(self, *children, **attributes):
+        text = children[0]
+
+        # Inspired by autodoc.py in Sphinx
+        rst = StringList()
+        for line in text.split("\n"):
+            rst.append(line, "<docleaf>")
+
+        rst_node = nodes.inline()
+        rst_node.document = self.state.document
+
+        copied.nested_inline_parse_with_titles(self.state, rst, rst_node)
+
+        return [rst_node]
+
+
+def render_node_list(node_list, node_manager):
+    # Use nested comprehension to flatten nodes lists coming back from render_node
+    return flatten(render_node(node, node_manager) for node in node_list)
+
+
+def flatten(list_of_lists):
+    return list(itertools.chain.from_iterable(list_of_lists))
+
+
+def render_node(node, node_manager):
+    if node.type == "text":
+        return [nodes.Text(node.text)]
+
+    node_builder = node_manager.get_builder(node.type)
+    children = render_node_list(node.children, node_manager)
+
+    if node.call_as == "text-element":
+        return node_builder("", "", *children, **node.attributes)
+    elif node.call_as == "element":
+        return node_builder("", *children, **node.attributes)
+    elif node.call_as == "function":
+        return node_builder(*children, **node.attributes)
+    else:
+        raise DocleafError("Call As not implemented: " + node.call_as)
+
+
+class Project:
+    def __init__(self, root, xml):
+        self._root = root
+        self._xml = xml
+
+    def root(self):
+        return self._root
+
+    def xml(self):
+        return self._xml
+
+    def get(projects, name: str):
+        # For each 'try' block we need to catch KeyError and TypeError (if project is a string) so we catch everything
+        # as there isn't much else that could go wrong
+
+        try:
+            data = projects[name]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find a project called '{name}' defined in the docleaf_projects config variable"
+            )
+
+        try:
+            root = data["root"]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find the 'root' entry in the data for '{name}' project defined in the docleaf_projects "
+                "config variable"
+            )
+
+        try:
+            xml = data["xml"]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find the 'xml' entry in the data for '{name}' project defined in the docleaf_projects "
+                "config variable"
+            )
+
+        return Project(root, xml)
+
+
+class BaseDirective(Directive):
+    def get_directive_args(self) -> list:
+        # Must match order in docutils.parsers.rst.Directive.__init__
+        return [
+            self.name,
+            self.arguments,
+            self.options,
+            self.content,
+            self.lineno,
+            self.content_offset,
+            self.block_text,
+            self.state,
+            self.state_machine,
+        ]
+
+
+class BasicDoxygenDirective(BaseDirective):
+    has_content = True
+    required_arguments = 1
+    optional_arguments = 0
+    final_argument_whitespace = True
+    option_spec = {
+        "project": directives.unchanged,
+        "skip-xml-nodes": directives.unchanged,
+    }
+
+    def run(self) -> List[Node]:
+        name = self.arguments[0]
+        project_name = self.options["project"] or self.app.config.docleaf_default_project
+        project = Project.get(self.app.config.docleaf_projects, project_name)
+        skip_settings = get_skip_settings(self.app, self.options)
+
+        context = backend.Context(
+            project.root(),
+            skip_settings,
+            self.app.config.docleaf_domain_by_extension,
+        )
+
+        tracked_cache = backend.TrackedCache(self.cache)
+        node_list = self.render_function(name, project.xml(), context, tracked_cache)
+        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
+
+        node_builder = NodeManager(self.state, self.get_directive_args())
+        return render_node_list(node_list, node_builder)
+
+
+class ClassDirective(BasicDoxygenDirective):
+    render_function = backend.render_class
+
+
+class StructDirective(BasicDoxygenDirective):
+    render_function = backend.render_struct
+
+
+class EnumDirective(BasicDoxygenDirective):
+    render_function = backend.render_enum
+
+
+class FunctionDirective(BasicDoxygenDirective):
+    render_function = backend.render_function
+
+
+class GroupDirective(BaseDirective):
+    has_content = True
+    required_arguments = 1
+    optional_arguments = 0
+    final_argument_whitespace = True
+    option_spec = {
+        "project": directives.unchanged,
+        "content-only": directives.flag,  # TODO: Implement
+        "inner": directives.flag,  # TODO: Implement
+        "skip-xml-nodes": directives.unchanged,
+    }
+
+    def run(self) -> List[Node]:
+        name = self.arguments[0]
+        project_name = self.options.get("project", self.app.config.docleaf_default_project)
+        project = Project.get(self.app.config.docleaf_projects, project_name)
+
+        skip_settings = get_skip_settings(self.app, self.options)
+        content_only = "content-only" in self.options
+        inner_group = "inner" in self.options
+        context = backend.Context(
+            project.root(),
+            skip_settings,
+            self.app.config.docleaf_domain_by_extension,
+        )
+
+        tracked_cache = backend.TrackedCache(self.cache)
+        node_list = backend.render_group(
+            name,
+            project.xml(),
+            context,
+            content_only,
+            inner_group,
+            tracked_cache,
+        )
+        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
+
+        node_builder = NodeManager(self.state, self.get_directive_args())
+        return render_node_list(node_list, node_builder)
+
+
+def get_skip_settings(app, options):
+    """
+    Get the option for the directive and fallback to the app option if not defined on the directive
+    """
+    skip_settings = options.get("skip", None)
+    if skip_settings is None:
+        skip_settings = app.config.docleaf_doxygen_skip
+    else:
+        skip_settings = skip_settings.split(",")
+    return skip_settings
+
+
+class XmlFileInfo:
+    def __init__(self, hash, rst_files):
+        self.hash = hash
+        self.rst_files = rst_files
+
+
+def hash_file(path):
+    logger.debug(f"docleaf: hashing {path}")
+    if sys.version_info >= (3, 11):
+        with open(path, "rb") as f:
+            digest = hashlib.file_digest(f, "sha1")
+            return digest.hexdigest()
+    else:
+        contents = open(path, "rb").read()
+        hash = hashlib.sha1()
+        hash.update(contents)
+        return hash.hexdigest()
+
+
+def update_sphinx_env_file_data(env: BuildEnvironment, xml_paths: List[str], rst_file: str):
+    """
+    Update our file_data store to indicate which rst files are dependent on which xml files
+    """
+    if not hasattr(env, "docleaf_file_data"):
+        env.docleaf_file_data = {}
+
+    for path in xml_paths:
+        if path in env.docleaf_file_data:
+            env.docleaf_file_data[path].rst_files.add(rst_file)
+        else:
+            env.docleaf_file_data[path] = XmlFileInfo(hash_file(path), set([rst_file]))
+
+
+def calculate_files_to_refresh(app: Sphinx, env, added, changed, removed):
+    """
+    Sphinx tells us which rst files have changed on disk and we can tell it (by returning a list of doc names) which
+    documents need to be re-read and have their output re-generated.
+
+    We calculate which files to refresh by storing the last build time and comparing the modified time of each xml file
+    against the last build time and see if any are newer. From there we need to get from the xml files to the rst files
+    that they impact and return those rst files to be refreshed.
+    """
+    logger.debug("docleaf: calculate_files_to_refresh")
+
+    # Get the last build time before updating it
+    last_build_time = getattr(app.env, "docleaf_last_build_time", None)
+
+    # Store the current time as the build time
+    app.env.docleaf_last_build_time = time.time()
+
+    if not last_build_time:
+        return []
+
+    if not hasattr(app.env, "docleaf_file_data"):
+        return []
+
+    rst_files_to_refresh = set()
+
+    for xml_file_path, info in app.env.docleaf_file_data.items():
+        stat = os.stat(xml_file_path)
+        if stat.st_mtime > last_build_time:
+            hash = hash_file(xml_file_path)
+            logger.debug(f"docleaf: stored hash for {xml_file_path} = {hash}. Calculated hash: {info.hash}")
+            if hash != info.hash:
+                # Store the new hash
+                info.hash = hash
+                # Tell Sphinx to refresh all rst files associated with this file
+                rst_files_to_refresh.update(info.rst_files)
+
+    logger.verbose(f"docleaf: calculate_files_to_refresh - Rebuild: {rst_files_to_refresh}")
+    return rst_files_to_refresh
+
+
+def purge_file_data(app, env, docname):
+    """
+    Clear any file data associated with 'docname' in accordance with the Sphinx API
+    """
+    logger.debug("docleaf: purge_file_data - %s", docname)
+    if not hasattr(app.env, "docleaf_file_data"):
+        return
+
+    for xml_file_path, info in app.env.docleaf_file_data.items():
+        info.rst_files.discard(docname)
+
+
+class ExtensionContext:
+    def __init__(self, app: Sphinx, cache):
+        self.app = app
+        self.cache = cache
+
+
+def add_directive(context, name, Cls):
+    Cls.app = context.app
+    Cls.cache = context.cache
+    context.app.add_directive(name, Cls)
+
+
+def setup(app: Sphinx):
+    cache = backend.FileCache()
+
+    context = ExtensionContext(app, cache)
+
+    add_directive(context, "doxygenclass", ClassDirective)
+    add_directive(context, "doxygenenum", EnumDirective)
+    add_directive(context, "doxygenfunction", FunctionDirective)
+    add_directive(context, "doxygengroup", GroupDirective)
+    add_directive(context, "doxygenstruct", StructDirective)
+
+    app.add_config_value("docleaf_projects", {}, "env")
+    app.add_config_value("docleaf_default_project", None, "env")
+    app.add_config_value("docleaf_doxygen_skip", [], "env")
+    app.add_config_value("docleaf_domain_by_extension", {}, True)
+
+    app.connect("env-get-outdated", calculate_files_to_refresh)
+    app.connect("env-purge-doc", purge_file_data)
+
+    return {"version": __version__, "parallel_read_safe": True, "parallel_write_safe": True}
```

## docleaf/errors.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-class DocleafError(Exception):
-    """
-    Standard error type for docleaf
-    """
-
-    pass
+class DocleafError(Exception):
+    """
+    Standard error type for docleaf
+    """
+
+    pass
```

## Comparing `docleaf-0.8.1.dist-info/METADATA` & `docleaf-0.8.2.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,205 +1,206 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.8.1
+Version: 0.8.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,!=5.0.0
 License-File: LICENSE.md
+License-File: LICENSES_THIRD_PARTY.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
 Keywords: sphinx,doxygen
 Author-email: Michael Jones <michael.jones@docleaf.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
 Project-URL: repository, https://github.com/docleaf-labs/docleaf
+Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
 Project-URL: homepage, https://docleaf.io
 
-<h1 align="center">
-  Docleaf
-</h1>
-
-<p align="center">
-   Your technical docs, beautifully integrated
-</p>
-
-Docleaf smoothly integrates your technical and long-form documentation. It is a Sphinx extension which reads Doxygen
-XML output and formats the information seamlessly with your user documentation.
-
-## License
-
-Docleaf is licensed under the [Parity Public License](./LICENSE.md). The Parity license allows permissive use of 
-Docleaf to help document open source projects. If you have a closed source project that you would like to document with
-Docleaf then you must purchase a commercial license.
-
-For further information please email: [support@docleaf.io](mailto:support@docleaf.io)
-
-## Features
-
-- Custom directives allowing you to target various parts of C and C++ code bases.
-- Integration with Sphinx C and C++ domains to support easily linking to your generated output.
-- Hash-based content checks, as well as timestamp checks, to minimize incremental build times after a Doxygen run.
-- Integration with the `sphinx.ext.linkcode` extension to support links to source code locations in a GitHub
-  repository.
-
-## Installation
-
-Docleaf can be installed from [PyPI](https://pypi.org/project/docleaf/):
-
-```
-pip install docleaf
-```
-
-## Usage
-
-Include `docleaf.doxygen` as an extension in your Sphinx `conf.py` file:
-
-```python
-extensions = ["docleaf.doxygen"]
-```
-
-Configure the extension to know where your source code is stored and the Doxygen XML output has been generated for
-your project. Optionally set the default project:
-
-```python
-docleaf_projects = {
-  "my_project": {
-    "root": "../src",
-    "xml": "../doxygen/xml"
-  }
-
-}
-docleaf_default_project = "my_project"
-```
-
-The use the provided directives in your reStructuredText files:
-
-```rst
-.. doxygenstruct:: ExampleStruct
-```
-
-See below for available directives.
-
-### Directives
-
-Generate documentation for a C++ class.
-
-```rst
-.. doxygenclass:: ClassName
-```
-
-Generate documentation for a C or C++ struct.
-
-```rst
-.. doxygenstruct:: StructName
-```
-
-Generate documentation for a C or C++ function.
-
-```rst
-.. doxygenfunction:: function_name
-```
-
-Generate documentation for a C or C++ enum.
-
-```rst
-.. doxygenenum:: EnumName
-```
-
-Generate documentation for specific group as specified within your Doxygen set up and code comments.
-
-```rst
-.. doxygengroup:: group_name
-```
-
-All directives take a `:project:` option to specify the project to use from your `conf.py` if you don't want to use
-the default project.
-
-### Settings
-
-- `docleaf_projects` 
-
-  A Python dictionary mapping each project name to the folders where its source code and Doxygen XML output are stored.
-
-- `docleaf_default_project`
-
-  The default project to use when none is specified on the directive itself.
-  
-- `docleaf_domain_by_extension`
-
-  A Python dictionary mapping from file extension to Sphinx domain. Docleaf uses Doxygen's language classifications
-  where possible but for optimal control of how source files are classified it is useful to use this setting. For
-  example:
-
-  ```python
-  docleaf_domain_by_extension = {"hpp": "cpp", "h": "c"}
-  ```
-
-  Will make sure that all files that end in `.hpp` will be considered as C++ files and processed using the C++ Sphinx
-  domain whilst files that end in `.h` will be considered C files and processed with the C Sphinx domain.
-
-- `docleaf_doxygen_skip`
-
-  A list of instructions describing any parts of the Doxygen XML to skip when generating the output documentation.
-  Supported entries are:
-
-  - `members:all_caps` - Skips any function or variable members (as defined as a 'memberdef' by Doxygen) which have 
-    names which are all capital letters and underscores. This is to allow users to filter our unprocessed C/C++ macros
-    if desirable.
-  - `xml-nodes:<node name>` - Skips reading and process of the given XML node and its children in the Doxygen XML 
-    output. Support is limited to the `htmlonly` node.
-
-### Integration with `sphinx.ext.linkcode`
-
-Docleaf can integrate with the `sphinx.ext.linkcode` extension in order to add `[source]` links next to various
-supported entries in your documentation. Linking to GitHub based repositories is supported.
-
-In order to use it, add the `sphinx.ext.linkcode` extension to the `extensions` list in your Sphinx `conf.py` and use
-the `docleaf.doxygen.GitHubLinkResolver` with appropriate parameters for your repository.
-
-```python
-extensions = [
-  "docleaf.doxygen",
-  "sphinx.ext.linkcode",
-  ]
-
-linkcode_resolve = docleaf.doxygen.GitHubLinkResolver(
-    root="../../../", user="docleaf-labs", repo="docleaf", branch="main"
-)
-```
-
-Where:
-- `root` is the relative path to the root of your repository.
-- `user` is the user or organisation name for your GitHub repository.
-- `repo` is the name of your GitHub repository.
-- `tag` is the git tag that you would like the generated link URLs to target.
-- `branch` is the git branch that you would like the generated link URLs to target.
-- `commit` is the git commit SHA that you would like the generated link URLs to target.
-
-Only one of `tag`, `branch` and `commit` is necessary.
-
-
-## Performance
-
-When doing a clean build of the Zephyr RTOS documentation suite, Docleaf is 2.1x faster than Breathe.
-
-```
-Benchmark: docleaf
-  Time (mean ± σ):     180.383 s ±  3.213 s    [User: 448.242 s, System: 12.908 s]
-  Range (min … max):   175.695 s … 185.187 s    10 runs
-```
-
-```
-Benchmark: breathe
-  Time (mean ± σ):     389.658 s ±  5.271 s    [User: 1839.366 s, System: 24.895 s]
-  Range (min … max):   379.093 s … 394.315 s    10 runs
-```
-
-## History
-
-Docleaf is written and maintained by the creator of the [Breathe](https://github.com/breathe-doc/breathe) project.
-It was created to resolve some of the performance and memory consumption issues with Breathe by rewriting the code
-base to use Rust. The user experience is designed to match and improve on Breathe.
+<h1 align="center">
+  Docleaf
+</h1>
+
+<p align="center">
+   Your technical docs, beautifully integrated
+</p>
+
+Docleaf smoothly integrates your technical and long-form documentation. It is a Sphinx extension which reads Doxygen
+XML output and formats the information seamlessly with your user documentation.
+
+## License
+
+Docleaf is licensed under the [Parity Public License](./LICENSE.md). The Parity license allows permissive use of 
+Docleaf to help document open source projects. If you have a closed source project that you would like to document with
+Docleaf then you must purchase a commercial license.
+
+For further information please email: [support@docleaf.io](mailto:support@docleaf.io)
+
+## Features
+
+- Custom directives allowing you to target various parts of C and C++ code bases.
+- Integration with Sphinx C and C++ domains to support easily linking to your generated output.
+- Hash-based content checks, as well as timestamp checks, to minimize incremental build times after a Doxygen run.
+- Integration with the `sphinx.ext.linkcode` extension to support links to source code locations in a GitHub
+  repository.
+
+## Installation
+
+Docleaf can be installed from [PyPI](https://pypi.org/project/docleaf/):
+
+```
+pip install docleaf
+```
+
+## Usage
+
+Include `docleaf.doxygen` as an extension in your Sphinx `conf.py` file:
+
+```python
+extensions = ["docleaf.doxygen"]
+```
+
+Configure the extension to know where your source code is stored and the Doxygen XML output has been generated for
+your project. Optionally set the default project:
+
+```python
+docleaf_projects = {
+  "my_project": {
+    "root": "../src",
+    "xml": "../doxygen/xml"
+  }
+
+}
+docleaf_default_project = "my_project"
+```
+
+The use the provided directives in your reStructuredText files:
+
+```rst
+.. doxygenstruct:: ExampleStruct
+```
+
+See below for available directives.
+
+### Directives
+
+Generate documentation for a C++ class.
+
+```rst
+.. doxygenclass:: ClassName
+```
+
+Generate documentation for a C or C++ struct.
+
+```rst
+.. doxygenstruct:: StructName
+```
+
+Generate documentation for a C or C++ function.
+
+```rst
+.. doxygenfunction:: function_name
+```
+
+Generate documentation for a C or C++ enum.
+
+```rst
+.. doxygenenum:: EnumName
+```
+
+Generate documentation for specific group as specified within your Doxygen set up and code comments.
+
+```rst
+.. doxygengroup:: group_name
+```
+
+All directives take a `:project:` option to specify the project to use from your `conf.py` if you don't want to use
+the default project.
+
+### Settings
+
+- `docleaf_projects` 
+
+  A Python dictionary mapping each project name to the folders where its source code and Doxygen XML output are stored.
+
+- `docleaf_default_project`
+
+  The default project to use when none is specified on the directive itself.
+  
+- `docleaf_domain_by_extension`
+
+  A Python dictionary mapping from file extension to Sphinx domain. Docleaf uses Doxygen's language classifications
+  where possible but for optimal control of how source files are classified it is useful to use this setting. For
+  example:
+
+  ```python
+  docleaf_domain_by_extension = {"hpp": "cpp", "h": "c"}
+  ```
+
+  Will make sure that all files that end in `.hpp` will be considered as C++ files and processed using the C++ Sphinx
+  domain whilst files that end in `.h` will be considered C files and processed with the C Sphinx domain.
+
+- `docleaf_doxygen_skip`
+
+  A list of instructions describing any parts of the Doxygen XML to skip when generating the output documentation.
+  Supported entries are:
+
+  - `members:all_caps` - Skips any function or variable members (as defined as a 'memberdef' by Doxygen) which have 
+    names which are all capital letters and underscores. This is to allow users to filter our unprocessed C/C++ macros
+    if desirable.
+  - `xml-nodes:<node name>` - Skips reading and process of the given XML node and its children in the Doxygen XML 
+    output. Support is limited to the `htmlonly` node.
+
+### Integration with `sphinx.ext.linkcode`
+
+Docleaf can integrate with the `sphinx.ext.linkcode` extension in order to add `[source]` links next to various
+supported entries in your documentation. Linking to GitHub based repositories is supported.
+
+In order to use it, add the `sphinx.ext.linkcode` extension to the `extensions` list in your Sphinx `conf.py` and use
+the `docleaf.doxygen.GitHubLinkResolver` with appropriate parameters for your repository.
+
+```python
+extensions = [
+  "docleaf.doxygen",
+  "sphinx.ext.linkcode",
+  ]
+
+linkcode_resolve = docleaf.doxygen.GitHubLinkResolver(
+    root="../../../", user="docleaf-labs", repo="docleaf", branch="main"
+)
+```
+
+Where:
+- `root` is the relative path to the root of your repository.
+- `user` is the user or organisation name for your GitHub repository.
+- `repo` is the name of your GitHub repository.
+- `tag` is the git tag that you would like the generated link URLs to target.
+- `branch` is the git branch that you would like the generated link URLs to target.
+- `commit` is the git commit SHA that you would like the generated link URLs to target.
+
+Only one of `tag`, `branch` and `commit` is necessary.
+
+
+## Performance
+
+When doing a clean build of the Zephyr RTOS documentation suite, Docleaf is 2.1x faster than Breathe.
+
+```
+Benchmark: docleaf
+  Time (mean ± σ):     180.383 s ±  3.213 s    [User: 448.242 s, System: 12.908 s]
+  Range (min … max):   175.695 s … 185.187 s    10 runs
+```
+
+```
+Benchmark: breathe
+  Time (mean ± σ):     389.658 s ±  5.271 s    [User: 1839.366 s, System: 24.895 s]
+  Range (min … max):   379.093 s … 394.315 s    10 runs
+```
+
+## History
+
+Docleaf is written and maintained by the creator of the [Breathe](https://github.com/breathe-doc/breathe) project.
+It was created to resolve some of the performance and memory consumption issues with Breathe by rewriting the code
+base to use Rust. The user experience is designed to match and improve on Breathe.
```

## Comparing `docleaf-0.8.1.dist-info/license_files/LICENSE.md` & `docleaf-0.8.2.dist-info/license_files/LICENSE.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# The Parity Public License 7.0.0
-
-Contributor: Michael Jones
-
-Source Code: https://github.com/docleaf-labs/docleaf
-
-## Purpose
-
-This license allows you to use and share this software for free, but you have to share software that builds on it alike.
-
-## Agreement
-
-In order to receive this license, you have to agree to its rules.  Those rules are both obligations under that agreement and conditions to your license.  Don't do anything with this software that triggers a rule you can't or won't follow.
-
-## Notices
-
-Make sure everyone who gets a copy of any part of this software from you, with or without changes, also gets the text of this license and the contributor and source code lines above.
-
-## Copyleft
-
-[Contribute](#contribute) software you develop, operate, or analyze with this software, including changes or additions to this software.  When in doubt, [contribute](#contribute).
-
-## Prototypes
-
-You don't have to [contribute](#contribute) any change, addition, or other software that meets all these criteria:
-
-1.  You don't use it for more than thirty days.
-
-2.  You don't share it outside the team developing it, other than for non-production user testing.
-
-3.  You don't develop, operate, or analyze other software with it for anyone outside the team developing it.
-
-## Reverse Engineering
-
-You may use this software to operate and analyze software you can't [contribute](#contribute) in order to develop alternatives you can and do [contribute](#contribute).
-
-## Contribute
-
-To [contribute](#contribute) software:
-
-1.  Publish all source code for the software in the preferred form for making changes through a freely accessible distribution system widely used for similar source code so the contributor and others can find and copy it.
-
-2.  Make sure every part of the source code is available under this license or another license that allows everything this license does, such as [the Blue Oak Model License 1.0.0](https://blueoakcouncil.org/license/1.0.0), [the Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html), [the MIT license](https://spdx.org/licenses/MIT.html), or [the two-clause BSD license](https://spdx.org/licenses/BSD-2-Clause.html).
-
-3.  Take these steps within thirty days.
-
-4.  Note that this license does _not_ allow you to change the license terms for this software.  You must follow [Notices](#notices).
-
-## Excuse
-
-You're excused for unknowingly breaking [Copyleft](#copyleft) if you [contribute](#contribute) as required, or stop doing anything requiring this license, within thirty days of learning you broke the rule.  You're excused for unknowingly breaking [Notices](#notices) if you take all practical steps to comply within thirty days of learning you broke the rule.
-
-## Defense
-
-Don't make any legal claim against anyone accusing this software, with or without changes, alone or with other technology, of infringing any patent.
-
-## Copyright
-
-The contributor licenses you to do everything with this software that would otherwise infringe their copyright in it.
-
-## Patent
-
-The contributor licenses you to do everything with this software that would otherwise infringe any patents they can license or become able to license.
-
-## Reliability
-
-The contributor can't revoke this license.
-
-## No Liability
-
-***As far as the law allows, this software comes as is, without any warranty or condition, and the contributor won't be liable to anyone for any damages related to this software or this license, under any kind of legal claim.***
+# The Parity Public License 7.0.0
+
+Contributor: Michael Jones
+
+Source Code: https://github.com/docleaf-labs/docleaf
+
+## Purpose
+
+This license allows you to use and share this software for free, but you have to share software that builds on it alike.
+
+## Agreement
+
+In order to receive this license, you have to agree to its rules.  Those rules are both obligations under that agreement and conditions to your license.  Don't do anything with this software that triggers a rule you can't or won't follow.
+
+## Notices
+
+Make sure everyone who gets a copy of any part of this software from you, with or without changes, also gets the text of this license and the contributor and source code lines above.
+
+## Copyleft
+
+[Contribute](#contribute) software you develop, operate, or analyze with this software, including changes or additions to this software.  When in doubt, [contribute](#contribute).
+
+## Prototypes
+
+You don't have to [contribute](#contribute) any change, addition, or other software that meets all these criteria:
+
+1.  You don't use it for more than thirty days.
+
+2.  You don't share it outside the team developing it, other than for non-production user testing.
+
+3.  You don't develop, operate, or analyze other software with it for anyone outside the team developing it.
+
+## Reverse Engineering
+
+You may use this software to operate and analyze software you can't [contribute](#contribute) in order to develop alternatives you can and do [contribute](#contribute).
+
+## Contribute
+
+To [contribute](#contribute) software:
+
+1.  Publish all source code for the software in the preferred form for making changes through a freely accessible distribution system widely used for similar source code so the contributor and others can find and copy it.
+
+2.  Make sure every part of the source code is available under this license or another license that allows everything this license does, such as [the Blue Oak Model License 1.0.0](https://blueoakcouncil.org/license/1.0.0), [the Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html), [the MIT license](https://spdx.org/licenses/MIT.html), or [the two-clause BSD license](https://spdx.org/licenses/BSD-2-Clause.html).
+
+3.  Take these steps within thirty days.
+
+4.  Note that this license does _not_ allow you to change the license terms for this software.  You must follow [Notices](#notices).
+
+## Excuse
+
+You're excused for unknowingly breaking [Copyleft](#copyleft) if you [contribute](#contribute) as required, or stop doing anything requiring this license, within thirty days of learning you broke the rule.  You're excused for unknowingly breaking [Notices](#notices) if you take all practical steps to comply within thirty days of learning you broke the rule.
+
+## Defense
+
+Don't make any legal claim against anyone accusing this software, with or without changes, alone or with other technology, of infringing any patent.
+
+## Copyright
+
+The contributor licenses you to do everything with this software that would otherwise infringe their copyright in it.
+
+## Patent
+
+The contributor licenses you to do everything with this software that would otherwise infringe any patents they can license or become able to license.
+
+## Reliability
+
+The contributor can't revoke this license.
+
+## No Liability
+
+***As far as the law allows, this software comes as is, without any warranty or condition, and the contributor won't be liable to anyone for any damages related to this software or this license, under any kind of legal claim.***
```

