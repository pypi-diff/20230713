# Comparing `tmp/windows_control-0.0.8.tar.gz` & `tmp/windows_control-0.0.9.tar.gz`

## Comparing `windows_control-0.0.8.tar` & `windows_control-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 windows_control-0.0.8/Cargo.toml
--rw-r--r--   0        0        0     2807 2023-06-28 03:33:37.000000 windows_control-0.0.8/.github/workflows/CI.yml
--rw-r--r--   0        0        0      756 2023-06-28 03:33:37.000000 windows_control-0.0.8/.gitignore
--rw-r--r--   0        0        0     2753 2023-07-02 15:41:49.000000 windows_control-0.0.8/README.md
--rw-r--r--   0        0        0      469 2023-06-28 09:07:29.000000 windows_control-0.0.8/README_PUB.md
--rw-r--r--   0        0        0      679 2023-06-28 09:02:28.000000 windows_control-0.0.8/justfile
--rw-r--r--   0        0        0      820 2023-07-06 02:49:26.000000 windows_control-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      585 2023-07-03 08:24:56.000000 windows_control-0.0.8/src/clean_up.rs
--rw-r--r--   0        0        0    14532 2023-07-03 03:45:51.000000 windows_control-0.0.8/src/keyboard/key_map.rs
--rw-r--r--   0        0        0     3495 2023-07-03 08:17:50.000000 windows_control-0.0.8/src/keyboard/mod.rs
--rw-r--r--   0        0        0     2318 2023-07-06 02:48:40.000000 windows_control-0.0.8/src/lib.rs
--rw-r--r--   0        0        0      840 2023-07-03 07:25:23.000000 windows_control-0.0.8/src/mouse/mod.rs
--rw-r--r--   0        0        0     5609 2023-07-06 02:42:06.000000 windows_control-0.0.8/src/window/mod.rs
--rw-r--r--   0        0        0     2844 2023-07-06 02:41:24.000000 windows_control-0.0.8/src/window/private.rs
--rw-r--r--   0        0        0     4254 2023-07-06 02:39:35.000000 windows_control-0.0.8/test.py
--rw-r--r--   0        0        0    65561 2023-07-06 02:39:21.000000 windows_control-0.0.8/Cargo.lock
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 windows_control-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 windows_control-0.0.9/Cargo.toml
+-rw-r--r--   0        0        0     2807 2023-06-28 03:33:37.000000 windows_control-0.0.9/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      756 2023-06-28 03:33:37.000000 windows_control-0.0.9/.gitignore
+-rw-r--r--   0        0        0     2753 2023-07-02 15:41:49.000000 windows_control-0.0.9/README.md
+-rw-r--r--   0        0        0      469 2023-06-28 09:07:29.000000 windows_control-0.0.9/README_PUB.md
+-rw-r--r--   0        0        0      679 2023-06-28 09:02:28.000000 windows_control-0.0.9/justfile
+-rw-r--r--   0        0        0      820 2023-07-13 13:33:58.000000 windows_control-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      585 2023-07-03 08:24:56.000000 windows_control-0.0.9/src/clean_up.rs
+-rw-r--r--   0        0        0    14532 2023-07-03 03:45:51.000000 windows_control-0.0.9/src/keyboard/key_map.rs
+-rw-r--r--   0        0        0     3495 2023-07-03 08:17:50.000000 windows_control-0.0.9/src/keyboard/mod.rs
+-rw-r--r--   0        0        0     1605 2023-07-13 13:33:41.000000 windows_control-0.0.9/src/lib.rs
+-rw-r--r--   0        0        0      840 2023-07-03 07:25:23.000000 windows_control-0.0.9/src/mouse/mod.rs
+-rw-r--r--   0        0        0     5609 2023-07-06 02:42:06.000000 windows_control-0.0.9/src/window/mod.rs
+-rw-r--r--   0        0        0     2844 2023-07-06 02:41:24.000000 windows_control-0.0.9/src/window/private.rs
+-rw-r--r--   0        0        0     4361 2023-07-06 03:08:55.000000 windows_control-0.0.9/test.py
+-rw-r--r--   0        0        0    62461 2023-07-13 13:33:11.000000 windows_control-0.0.9/Cargo.lock
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 windows_control-0.0.9/PKG-INFO
```

### Comparing `windows_control-0.0.8/Cargo.toml` & `windows_control-0.0.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 crate-type = ["cdylib"] # "cdylib" is necessary to produce a shared library for Python to import from.
 
 [dependencies]
 enigo = "0.1.2"
 phf = {version="0.11.2",features=["macros"]}
 winapi = { version = "0.3.9", features = ["winuser","libloaderapi","shellapi","winerror","dwmapi","shellscalingapi"] }
 # windows = "0.48.0"
-opencv = {version = "0.82.1"}
+# opencv = {version = "0.82.1"}
 image = "0.24.6"
 show-image = "0.13.1"
 screenshots = "0.6.0"
 lazy_static = "1.4"
 
 [dependencies.pyo3]
 version = "0.19.0"
```

### Comparing `windows_control-0.0.8/.github/workflows/CI.yml` & `windows_control-0.0.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/.gitignore` & `windows_control-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/README.md` & `windows_control-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/justfile` & `windows_control-0.0.9/justfile`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/pyproject.toml` & `windows_control-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "windows_control"
-version = "0.0.8"
+version = "0.0.9"
 description = "It is used to do some control with keyboard/mouse on windows (especially on win10)."
 readme = "README_PUB.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

### Comparing `windows_control-0.0.8/src/clean_up.rs` & `windows_control-0.0.9/src/clean_up.rs`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/src/keyboard/key_map.rs` & `windows_control-0.0.9/src/keyboard/key_map.rs`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/src/keyboard/mod.rs` & `windows_control-0.0.9/src/keyboard/mod.rs`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/src/mouse/mod.rs` & `windows_control-0.0.9/src/mouse/mod.rs`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/src/window/mod.rs` & `windows_control-0.0.9/src/window/mod.rs`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/src/window/private.rs` & `windows_control-0.0.9/src/window/private.rs`

 * *Files identical despite different names*

### Comparing `windows_control-0.0.8/test.py` & `windows_control-0.0.9/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from time import sleep
 
 # Add the path to the Rust library to the sys.path list
 rust_lib_path = os.path.abspath(r'C:\Users\Administrator\Desktop\rust_lib\target\debug')
 sys.path.append(rust_lib_path)
 
 # Import the Rust library for testing
+opencv_lib_path = os.path.abspath(r'C:\tools\opencv\build\x64\vc16\bin')
+sys.path.append(opencv_lib_path)
+
 import windows_control
 from windows_control import keyboard, mouse, window
 
 
 def test_keyboard(input_key):
     # Test press_key
     keyboard.press(input_key)
```

### Comparing `windows_control-0.0.8/Cargo.lock` & `windows_control-0.0.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,14 @@
 dependencies = [
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
-name = "aho-corasick"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -142,51 +133,28 @@
 ]
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
-dependencies = [
- "jobserver",
-]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cfg_aliases"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
 
 [[package]]
-name = "clang"
-version = "2.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c044c781163c001b913cd018fc95a628c50d0d2dfea8bca77dad71edb16e37"
-dependencies = [
- "clang-sys",
- "libc",
-]
-
-[[package]]
-name = "clang-sys"
-version = "1.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c688fc74432808e3eb684cae8830a86be1d66a2bd58e1f248ed0960a590baf6f"
-dependencies = [
- "glob",
- "libc",
-]
-
-[[package]]
 name = "cmake"
 version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
  "cc",
 ]
@@ -472,20 +440,14 @@
 [[package]]
 name = "downcast-rs"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
 
 [[package]]
-name = "dunce"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
-
-[[package]]
 name = "dwrote"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439a1c2ba5611ad3ed731280541d36d2e9c4ac5e7fb818a27b604bdc5a6aa65b"
 dependencies = [
  "lazy_static",
  "libc",
@@ -766,20 +728,14 @@
 [[package]]
 name = "glam"
 version = "0.21.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "518faa5064866338b013ff9b2350dc318e14cc4fcd6cb8206d7e7c9886c98815"
 
 [[package]]
-name = "glob"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
-
-[[package]]
 name = "glow"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8bd5877156a19b8ac83a29b2306fe20537429d318f3ff0a1a2119f8d9c61919"
 dependencies = [
  "js-sys",
  "slotmap",
@@ -934,23 +890,14 @@
 [[package]]
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
-name = "jobserver"
-version = "0.1.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "jpeg-decoder"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
 dependencies = [
  "rayon",
 ]
@@ -1329,47 +1276,14 @@
 [[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
-name = "opencv"
-version = "0.82.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79290f5f138b26637cae0ae243d77de871a096e334d3fca22f5ddf31ab6f4cc5"
-dependencies = [
- "cc",
- "dunce",
- "jobserver",
- "libc",
- "num-traits",
- "once_cell",
- "opencv-binding-generator",
- "pkg-config",
- "semver",
- "shlex",
- "vcpkg",
-]
-
-[[package]]
-name = "opencv-binding-generator"
-version = "0.66.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be5f640bda28b478629f525e8525601586a2a2b9403a4b8f2264fa5fcfebe6be"
-dependencies = [
- "clang",
- "clang-sys",
- "dunce",
- "once_cell",
- "percent-encoding",
- "regex",
-]
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1673,43 +1587,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "regex"
-version = "1.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89089e897c013b3deb627116ae56a6955a72b8bed395c9526af31c9fe528b484"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-automata",
- "regex-syntax",
-]
-
-[[package]]
-name = "regex-automata"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa250384981ea14565685dea16a9ccc4d1c541a13f82b9c168572264d1df8c56"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-syntax",
-]
-
-[[package]]
-name = "regex-syntax"
-version = "0.7.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ab07dc67230e4a4718e70fd5c20055a4334b121f1f9db8fe63ef39ce9b8c846"
-
-[[package]]
 name = "renderdoc-sys"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1382d1f0a252c4bf97dc20d979a2fdd05b024acd7c2ed0f7595d7817666a157"
 
 [[package]]
 name = "rustc-hash"
@@ -1817,20 +1702,14 @@
 dependencies = [
  "expat-sys",
  "freetype-sys",
  "pkg-config",
 ]
 
 [[package]]
-name = "shlex"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
-
-[[package]]
 name = "show-image"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b8a66a2f47667d404f77403a68263263b52af6c1136bccdad448bb1c38ac215"
 dependencies = [
  "futures",
  "glam",
@@ -2063,20 +1942,14 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "vcpkg"
-version = "0.2.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
-
-[[package]]
 name = "vec_map"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
 
 [[package]]
 name = "version_check"
@@ -2443,15 +2316,14 @@
 [[package]]
 name = "windows_control_python"
 version = "0.1.0"
 dependencies = [
  "enigo",
  "image",
  "lazy_static",
- "opencv",
  "phf",
  "pyo3",
  "screenshots",
  "show-image",
  "winapi",
 ]
```

### Comparing `windows_control-0.0.8/PKG-INFO` & `windows_control-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windows_control
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: It is used to do some control with keyboard/mouse on windows (especially on win10).
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/dbsxdbsx/windows_control
```

