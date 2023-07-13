# Comparing `tmp/rs_parsepatch-0.3.9.tar.gz` & `tmp/rs_parsepatch-0.4.0.tar.gz`

## Comparing `rs_parsepatch-0.3.9.tar` & `rs_parsepatch-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 rs_parsepatch-0.3.9/Cargo.toml
--rw-r--r--   0        0        0      647 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/README.md
--rw-r--r--   0        0        0      736 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-12 18:12:11.000000 rs_parsepatch-0.3.9/requirements-dev.txt
--rw-r--r--   0        0        0     4365 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/common.rs
--rw-r--r--   0        0        0     2026 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/counts.rs
--rw-r--r--   0        0        0     3123 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/diffs.rs
--rw-r--r--   0        0        0     2923 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/init.rs
--rw-r--r--   0        0        0      121 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/lib.rs
--rw-r--r--   0        0        0     2074 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/lines.rs
--rw-r--r--   0        0        0        0 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/__init__.py
--rw-r--r--   0        0        0   144528 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/77ec8a41ee73.patch
--rw-r--r--   0        0        0    10523 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/7dabae5e261a.patch
--rw-r--r--   0        0        0    11559 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/7e60ad275b73.patch
--rw-r--r--   0        0        0    35876 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/81d3e4a2f3f3.patch
--rw-r--r--   0        0        0    33381 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/b184c87f7606.patch
--rw-r--r--   0        0        0    41777 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/c4c0ad8b3eaa.patch
--rw-r--r--   0        0        0     2126 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/c58e9e70f971.patch
--rw-r--r--   0        0        0     3253 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/c6f9187b0b2e.patch
--rw-r--r--   0        0        0    13091 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/d4f80c4ba719.patch
--rw-r--r--   0        0        0   104682 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/d7a700707ddb.patch
--rw-r--r--   0        0        0    51155 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/f045ac9f76cf.patch
--rw-r--r--   0        0        0     1977 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/no_git_header.patch
--rw-r--r--   0        0        0     2902 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/test_parsepatch.py
--rw-r--r--   0        0        0     7399 2023-04-12 18:12:13.000000 rs_parsepatch-0.3.9/Cargo.lock
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 rs_parsepatch-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 rs_parsepatch-0.4.0/Cargo.toml
+-rw-r--r--   0        0        0      647 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/README.md
+-rw-r--r--   0        0        0      736 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-07-13 12:16:47.000000 rs_parsepatch-0.4.0/requirements-dev.txt
+-rw-r--r--   0        0        0     4365 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/src/common.rs
+-rw-r--r--   0        0        0     2026 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/src/counts.rs
+-rw-r--r--   0        0        0     3123 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/src/diffs.rs
+-rw-r--r--   0        0        0     2947 2023-07-13 12:30:27.000000 rs_parsepatch-0.4.0/src/init.rs
+-rw-r--r--   0        0        0      121 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/src/lib.rs
+-rw-r--r--   0        0        0     2074 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/src/lines.rs
+-rw-r--r--   0        0        0        0 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0   144528 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/77ec8a41ee73.patch
+-rw-r--r--   0        0        0    10523 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/7dabae5e261a.patch
+-rw-r--r--   0        0        0    11559 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/7e60ad275b73.patch
+-rw-r--r--   0        0        0    35876 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/81d3e4a2f3f3.patch
+-rw-r--r--   0        0        0    33381 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/b184c87f7606.patch
+-rw-r--r--   0        0        0    41777 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/c4c0ad8b3eaa.patch
+-rw-r--r--   0        0        0     2126 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/c58e9e70f971.patch
+-rw-r--r--   0        0        0     3253 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/c6f9187b0b2e.patch
+-rw-r--r--   0        0        0    13091 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/d4f80c4ba719.patch
+-rw-r--r--   0        0        0   104682 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/d7a700707ddb.patch
+-rw-r--r--   0        0        0    51155 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/f045ac9f76cf.patch
+-rw-r--r--   0        0        0     1977 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/patches/no_git_header.patch
+-rw-r--r--   0        0        0     2902 2023-03-07 08:29:14.000000 rs_parsepatch-0.4.0/tests/test_parsepatch.py
+-rw-r--r--   0        0        0     7851 2023-07-13 14:16:12.000000 rs_parsepatch-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 rs_parsepatch-0.4.0/PKG-INFO
```

### Comparing `rs_parsepatch-0.3.9/README.md` & `rs_parsepatch-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/pyproject.toml` & `rs_parsepatch-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/src/common.rs` & `rs_parsepatch-0.4.0/src/common.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/src/counts.rs` & `rs_parsepatch-0.4.0/src/counts.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/src/diffs.rs` & `rs_parsepatch-0.4.0/src/diffs.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/src/init.rs` & `rs_parsepatch-0.4.0/src/init.rs`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
             return Err(PyTypeError::new_err("Invalid patch type"));
         };
 
         patch.get_result()
     }};
 }
 
-#[pyfunction(kwargs = "**")]
+#[pyfunction]
+#[pyo3(signature = (bytes, **kwargs))]
 /// Get the added/deleted/moved lines for each file in the patch.
 /// Each line is a tuple (old_line_no, new_line_no, line_bytes).
 /// If the line is added then old_line_no is None.
 /// If the line is deleted then new_line_no is None.
 /// If the hunks=True is passed as argument then the lines are gathered by hunk
 fn get_diffs(py: Python, bytes: PyObject, kwargs: Option<&PyDict>) -> PyResult<PyObject> {
     let hunks = if let Some(kwargs) = kwargs {
```

### Comparing `rs_parsepatch-0.3.9/src/lines.rs` & `rs_parsepatch-0.4.0/src/lines.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/77ec8a41ee73.patch` & `rs_parsepatch-0.4.0/tests/patches/77ec8a41ee73.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/7dabae5e261a.patch` & `rs_parsepatch-0.4.0/tests/patches/7dabae5e261a.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/7e60ad275b73.patch` & `rs_parsepatch-0.4.0/tests/patches/7e60ad275b73.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/81d3e4a2f3f3.patch` & `rs_parsepatch-0.4.0/tests/patches/81d3e4a2f3f3.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/b184c87f7606.patch` & `rs_parsepatch-0.4.0/tests/patches/b184c87f7606.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/c4c0ad8b3eaa.patch` & `rs_parsepatch-0.4.0/tests/patches/c4c0ad8b3eaa.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/c58e9e70f971.patch` & `rs_parsepatch-0.4.0/tests/patches/c58e9e70f971.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/c6f9187b0b2e.patch` & `rs_parsepatch-0.4.0/tests/patches/c6f9187b0b2e.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/d4f80c4ba719.patch` & `rs_parsepatch-0.4.0/tests/patches/d4f80c4ba719.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/d7a700707ddb.patch` & `rs_parsepatch-0.4.0/tests/patches/d7a700707ddb.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/f045ac9f76cf.patch` & `rs_parsepatch-0.4.0/tests/patches/f045ac9f76cf.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/patches/no_git_header.patch` & `rs_parsepatch-0.4.0/tests/patches/no_git_header.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/tests/test_parsepatch.py` & `rs_parsepatch-0.4.0/tests/test_parsepatch.py`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.9/Cargo.lock` & `rs_parsepatch-0.4.0/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -18,261 +18,272 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "indoc"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05a0bd019339e5d968b37855180087b7b9d512c5046fbd244cf8c95687927d6e"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.126"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "349d5a591cd28b49e1d1037471617a32ddcda5731b99419008085f72d5a53836"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.7"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327fa5b6a6940e4699ec49a9beae1ea4845c6bab9314e4f84ac68742139d8c53"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.13.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18a6dbe30758c9f83eb00cbea4ac95966305f5a7772f3f42ebfc7fc7eddbd8e1"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.3"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a279cbf25cb0757810394fbc1e359949b59e348145c643a939a525692e6929"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "parsepatch"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e4853d6c2baee52240ca7e6fe96938ed07981d304ab1a73b5b3e7d9dcd3cc48"
+checksum = "46c056f107e40038b8a19e5ff78ae6308ff0704dd36aaf4d1b1e0ec568f39543"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.42"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c278e965f1d8cf32d6e0e96de3d3e79712178ae67986d9cf9151f51e95aac89b"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.20"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bcdf212e9776fbcb2d23ab029360416bb1706b1aea2d1a5ba002727cbcab804"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rs_parsepatch"
-version = "0.3.9"
+version = "0.4.0"
 dependencies = [
  "parsepatch",
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.9.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
-version = "1.0.98"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c50aef8a904de4c23c788f104b7dddc7d6f79c647c7c8ce4cc8f73eb0ca773dd"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.4"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.2"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15c61ba63f9235225a22310255a29b806b907c9b8c964bcbd0a2c70f3f2deea7"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unindent"
-version = "0.1.9"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52fee519a3e570f7df377a06a1a7775cdbfb7aa460be7e08de2b1f0e69973a44"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "windows-sys"
-version = "0.36.1"
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
+ "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `rs_parsepatch-0.3.9/PKG-INFO` & `rs_parsepatch-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs_parsepatch
-Version: 0.3.9
+Version: 0.4.0
 Home-Page: https://github.com/mozilla/pyo3-parsepatch
 Author: calixteman <cdenizet@mozilla.com>
 Author-email: calixteman <cdenizet@mozilla.com>
 License: MPL-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/mozilla/pyo3-parsepatch
```

