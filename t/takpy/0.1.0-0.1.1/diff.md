# Comparing `tmp/takpy-0.1.0.tar.gz` & `tmp/takpy-0.1.1.tar.gz`

## Comparing `takpy-0.1.0.tar` & `takpy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 takpy-0.1.0/Cargo.toml
--rw-r--r--   0        0        0      681 2023-07-13 12:49:07.000000 takpy-0.1.0/README.md
--rw-r--r--   0        0        0      379 2023-07-13 12:51:42.000000 takpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5870 2023-07-13 12:45:40.000000 takpy-0.1.0/src/lib.rs
--rw-r--r--   0        0        0     7848 2023-07-13 12:37:44.000000 takpy-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 takpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 takpy-0.1.1/Cargo.toml
+-rw-r--r--   0        0        0     5856 2023-07-13 13:00:30.000000 takpy-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       38 2023-07-13 13:28:26.000000 takpy-0.1.1/.gitignore
+-rw-r--r--   0        0        0      681 2023-07-13 12:49:07.000000 takpy-0.1.1/README.md
+-rw-r--r--   0        0        0      379 2023-07-13 12:51:42.000000 takpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6045 2023-07-13 13:27:13.000000 takpy-0.1.1/src/lib.rs
+-rw-r--r--   0        0        0     7848 2023-07-13 13:27:21.000000 takpy-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 takpy-0.1.1/PKG-INFO
```

### Comparing `takpy-0.1.0/README.md` & `takpy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `takpy-0.1.0/src/lib.rs` & `takpy-0.1.1/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,19 @@
                     self.0.ply
                 }
 
                 #[getter]
                 fn reversible_plies(&self) -> u16 {
                     self.0.reversible_plies
                 }
+
+                // TODO: Figure out if this is the right way to do it
+                fn clone(&self) -> Game {
+                    Clone::clone(self)
+                }
             }
         }
     };
 }
 
 game!(size_3, 3, 0);
 game!(size_4, 4, 0);
```

### Comparing `takpy-0.1.0/Cargo.lock` & `takpy-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 name = "takparse"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "616bf8626a329585beb63e0bb03a5d809318da9d41d7bfb694222ded8b0f4846"
 
 [[package]]
 name = "takpy"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "fast-tak",
  "pyo3",
 ]
 
 [[package]]
 name = "target-lexicon"
```

### Comparing `takpy-0.1.0/PKG-INFO` & `takpy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: takpy
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # takpy
```

