# Comparing `tmp/rs_parsepatch-0.3.8.tar.gz` & `tmp/rs_parsepatch-0.3.9.tar.gz`

## Comparing `rs_parsepatch-0.3.8.tar` & `rs_parsepatch-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 rs_parsepatch-0.3.8/Cargo.toml
--rw-r--r--   0        0        0      647 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/README.md
--rw-r--r--   0        0        0      736 2023-03-06 21:54:28.000000 rs_parsepatch-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       46 2023-03-06 21:48:17.000000 rs_parsepatch-0.3.8/requirements-dev.txt
--rw-r--r--   0        0        0     4365 2020-11-12 17:30:01.000000 rs_parsepatch-0.3.8/src/common.rs
--rw-r--r--   0        0        0     2026 2020-11-05 12:29:36.000000 rs_parsepatch-0.3.8/src/counts.rs
--rw-r--r--   0        0        0     3123 2020-11-05 12:29:36.000000 rs_parsepatch-0.3.8/src/diffs.rs
--rw-r--r--   0        0        0     2923 2020-11-12 17:30:01.000000 rs_parsepatch-0.3.8/src/init.rs
--rw-r--r--   0        0        0      121 2021-07-22 12:49:09.000000 rs_parsepatch-0.3.8/src/lib.rs
--rw-r--r--   0        0        0     2074 2020-11-05 12:29:36.000000 rs_parsepatch-0.3.8/src/lines.rs
--rw-r--r--   0        0        0        0 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0   144528 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/77ec8a41ee73.patch
--rw-r--r--   0        0        0    10523 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/7dabae5e261a.patch
--rw-r--r--   0        0        0    11559 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/7e60ad275b73.patch
--rw-r--r--   0        0        0    35876 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/81d3e4a2f3f3.patch
--rw-r--r--   0        0        0    33381 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/b184c87f7606.patch
--rw-r--r--   0        0        0    41777 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/c4c0ad8b3eaa.patch
--rw-r--r--   0        0        0     2126 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/c58e9e70f971.patch
--rw-r--r--   0        0        0     3253 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/c6f9187b0b2e.patch
--rw-r--r--   0        0        0    13091 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/d4f80c4ba719.patch
--rw-r--r--   0        0        0   104682 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/d7a700707ddb.patch
--rw-r--r--   0        0        0    51155 2019-10-16 07:40:28.000000 rs_parsepatch-0.3.8/tests/patches/f045ac9f76cf.patch
--rw-r--r--   0        0        0     1977 2020-11-05 12:29:36.000000 rs_parsepatch-0.3.8/tests/patches/no_git_header.patch
--rw-r--r--   0        0        0     2902 2019-10-16 10:16:04.000000 rs_parsepatch-0.3.8/tests/test_parsepatch.py
--rw-r--r--   0        0        0     7399 2023-03-06 22:12:56.000000 rs_parsepatch-0.3.8/Cargo.lock
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 rs_parsepatch-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 rs_parsepatch-0.3.9/Cargo.toml
+-rw-r--r--   0        0        0      647 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/README.md
+-rw-r--r--   0        0        0      736 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-12 18:12:11.000000 rs_parsepatch-0.3.9/requirements-dev.txt
+-rw-r--r--   0        0        0     4365 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/common.rs
+-rw-r--r--   0        0        0     2026 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/counts.rs
+-rw-r--r--   0        0        0     3123 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/diffs.rs
+-rw-r--r--   0        0        0     2923 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/init.rs
+-rw-r--r--   0        0        0      121 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/lib.rs
+-rw-r--r--   0        0        0     2074 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/src/lines.rs
+-rw-r--r--   0        0        0        0 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0   144528 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/77ec8a41ee73.patch
+-rw-r--r--   0        0        0    10523 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/7dabae5e261a.patch
+-rw-r--r--   0        0        0    11559 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/7e60ad275b73.patch
+-rw-r--r--   0        0        0    35876 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/81d3e4a2f3f3.patch
+-rw-r--r--   0        0        0    33381 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/b184c87f7606.patch
+-rw-r--r--   0        0        0    41777 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/c4c0ad8b3eaa.patch
+-rw-r--r--   0        0        0     2126 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/c58e9e70f971.patch
+-rw-r--r--   0        0        0     3253 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/c6f9187b0b2e.patch
+-rw-r--r--   0        0        0    13091 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/d4f80c4ba719.patch
+-rw-r--r--   0        0        0   104682 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/d7a700707ddb.patch
+-rw-r--r--   0        0        0    51155 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/f045ac9f76cf.patch
+-rw-r--r--   0        0        0     1977 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/patches/no_git_header.patch
+-rw-r--r--   0        0        0     2902 2023-03-07 20:23:01.000000 rs_parsepatch-0.3.9/tests/test_parsepatch.py
+-rw-r--r--   0        0        0     7399 2023-04-12 18:12:13.000000 rs_parsepatch-0.3.9/Cargo.lock
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 rs_parsepatch-0.3.9/PKG-INFO
```

### Comparing `rs_parsepatch-0.3.8/README.md` & `rs_parsepatch-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/pyproject.toml` & `rs_parsepatch-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/src/common.rs` & `rs_parsepatch-0.3.9/src/common.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/src/counts.rs` & `rs_parsepatch-0.3.9/src/counts.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/src/diffs.rs` & `rs_parsepatch-0.3.9/src/diffs.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/src/init.rs` & `rs_parsepatch-0.3.9/src/init.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/src/lines.rs` & `rs_parsepatch-0.3.9/src/lines.rs`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/77ec8a41ee73.patch` & `rs_parsepatch-0.3.9/tests/patches/77ec8a41ee73.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/7dabae5e261a.patch` & `rs_parsepatch-0.3.9/tests/patches/7dabae5e261a.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/7e60ad275b73.patch` & `rs_parsepatch-0.3.9/tests/patches/7e60ad275b73.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/81d3e4a2f3f3.patch` & `rs_parsepatch-0.3.9/tests/patches/81d3e4a2f3f3.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/b184c87f7606.patch` & `rs_parsepatch-0.3.9/tests/patches/b184c87f7606.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/c4c0ad8b3eaa.patch` & `rs_parsepatch-0.3.9/tests/patches/c4c0ad8b3eaa.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/c58e9e70f971.patch` & `rs_parsepatch-0.3.9/tests/patches/c58e9e70f971.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/c6f9187b0b2e.patch` & `rs_parsepatch-0.3.9/tests/patches/c6f9187b0b2e.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/d4f80c4ba719.patch` & `rs_parsepatch-0.3.9/tests/patches/d4f80c4ba719.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/d7a700707ddb.patch` & `rs_parsepatch-0.3.9/tests/patches/d7a700707ddb.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/f045ac9f76cf.patch` & `rs_parsepatch-0.3.9/tests/patches/f045ac9f76cf.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/patches/no_git_header.patch` & `rs_parsepatch-0.3.9/tests/patches/no_git_header.patch`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/tests/test_parsepatch.py` & `rs_parsepatch-0.3.9/tests/test_parsepatch.py`

 * *Files identical despite different names*

### Comparing `rs_parsepatch-0.3.8/Cargo.lock` & `rs_parsepatch-0.3.9/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -87,17 +87,17 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "parsepatch"
-version = "0.2.9"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b82b65ac8bbacb8e8dec02d4d95e4246af4a6545cce91ca910da8eea9269afde"
+checksum = "5e4853d6c2baee52240ca7e6fe96938ed07981d304ab1a73b5b3e7d9dcd3cc48"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "proc-macro2"
 version = "1.0.42"
@@ -105,66 +105,66 @@
 checksum = "c278e965f1d8cf32d6e0e96de3d3e79712178ae67986d9cf9151f51e95aac89b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
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
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -183,15 +183,15 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rs_parsepatch"
-version = "0.3.8"
+version = "0.3.9"
 dependencies = [
  "parsepatch",
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
```

### Comparing `rs_parsepatch-0.3.8/PKG-INFO` & `rs_parsepatch-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs_parsepatch
-Version: 0.3.8
+Version: 0.3.9
 Home-Page: https://github.com/mozilla/pyo3-parsepatch
 Author: calixteman <cdenizet@mozilla.com>
 Author-email: calixteman <cdenizet@mozilla.com>
 License: MPL-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/mozilla/pyo3-parsepatch
```

