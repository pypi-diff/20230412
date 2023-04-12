# Comparing `tmp/typst-0.1.4.tar.gz` & `tmp/typst-0.2.0.tar.gz`

## Comparing `typst-0.1.4.tar` & `typst-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 typst-0.1.4/Cargo.toml
--rw-r--r--   0     1001      123     2752 2023-04-07 08:16:41.000000 typst-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-07 08:16:41.000000 typst-0.1.4/.gitignore
--rw-r--r--   0     1001      123     9723 2023-04-07 08:16:41.000000 typst-0.1.4/LICENSE
--rw-r--r--   0     1001      123      766 2023-04-07 08:16:41.000000 typst-0.1.4/README.md
--rw-r--r--   0     1001      123      421 2023-04-07 08:16:41.000000 typst-0.1.4/pyproject.toml
--rw-r--r--   0     1001      123       74 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/__init__.py
--rw-r--r--   0     1001      123      483 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/__init__.pyi
--rw-r--r--   0     1001      123   331992 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/DejaVuSansMono-Bold.ttf
--rw-r--r--   0     1001      123   253580 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
--rw-r--r--   0     1001      123   251932 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/DejaVuSansMono-Oblique.ttf
--rw-r--r--   0     1001      123   340712 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/DejaVuSansMono.ttf
--rw-r--r--   0     1001      123   806856 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/LinLibertine_R.ttf
--rw-r--r--   0     1001      123   748600 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/LinLibertine_RB.ttf
--rw-r--r--   0     1001      123   533532 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/LinLibertine_RBI.ttf
--rw-r--r--   0     1001      123   721340 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/LinLibertine_RI.ttf
--rw-r--r--   0     1001      123   499128 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/NewCM10-Bold.otf
--rw-r--r--   0     1001      123   445800 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/NewCM10-BoldItalic.otf
--rw-r--r--   0     1001      123   464808 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/NewCM10-Italic.otf
--rw-r--r--   0     1001      123   547508 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/NewCM10-Regular.otf
--rw-r--r--   0     1001      123  2161432 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/NewCMMath-Book.otf
--rw-r--r--   0     1001      123  1229208 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/fonts/NewCMMath-Regular.otf
--rw-r--r--   0     1001      123        1 2023-04-07 08:16:41.000000 typst-0.1.4/python/typst/py.typed
--rw-r--r--   0     1001      123     9415 2023-04-07 08:16:41.000000 typst-0.1.4/src/compiler.rs
--rw-r--r--   0     1001      123     3946 2023-04-07 08:16:41.000000 typst-0.1.4/src/lib.rs
--rw-r--r--   0     1001      123    38849 2023-04-07 08:16:41.000000 typst-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 typst-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 typst-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2752 2023-04-12 02:23:06.000000 typst-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-12 02:23:06.000000 typst-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     9723 2023-04-12 02:23:06.000000 typst-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      766 2023-04-12 02:23:06.000000 typst-0.2.0/README.md
+-rw-r--r--   0     1001      123      421 2023-04-12 02:23:06.000000 typst-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123       74 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/__init__.py
+-rw-r--r--   0     1001      123      483 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/__init__.pyi
+-rw-r--r--   0     1001      123   331992 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0     1001      123   253580 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
+-rw-r--r--   0     1001      123   251932 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
+-rw-r--r--   0     1001      123   340712 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0     1001      123   806856 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_R.ttf
+-rw-r--r--   0     1001      123   748600 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_RB.ttf
+-rw-r--r--   0     1001      123   533532 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_RBI.ttf
+-rw-r--r--   0     1001      123   721340 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/LinLibertine_RI.ttf
+-rw-r--r--   0     1001      123   499128 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-Bold.otf
+-rw-r--r--   0     1001      123   445800 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-BoldItalic.otf
+-rw-r--r--   0     1001      123   464808 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-Italic.otf
+-rw-r--r--   0     1001      123   547508 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCM10-Regular.otf
+-rw-r--r--   0     1001      123  2161432 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCMMath-Book.otf
+-rw-r--r--   0     1001      123  1229208 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/fonts/NewCMMath-Regular.otf
+-rw-r--r--   0     1001      123        1 2023-04-12 02:23:06.000000 typst-0.2.0/python/typst/py.typed
+-rw-r--r--   0     1001      123     9415 2023-04-12 02:23:06.000000 typst-0.2.0/src/compiler.rs
+-rw-r--r--   0     1001      123     3946 2023-04-12 02:23:06.000000 typst-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123    41249 2023-04-12 02:23:06.000000 typst-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 typst-0.2.0/PKG-INFO
```

### Comparing `typst-0.1.4/Cargo.toml` & `typst-0.2.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "typst-py"
-version = "0.1.4"
+version = "0.2.0"
 edition = "2021"
 description = "Python binding to typst"
 license = "Apache-2.0"
 repository = "https://github.com/messense/typst-py"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.18.1", features = ["abi3-py37"] }
-typst = { git = "https://github.com/typst/typst.git", tag = "v0.1.0" }
-typst-library = { git = "https://github.com/typst/typst.git", tag = "v0.1.0" }
+typst = { git = "https://github.com/typst/typst.git", tag = "v0.2.0" }
+typst-library = { git = "https://github.com/typst/typst.git", tag = "v0.2.0" }
 comemo = "0.2"
 dirs = "5"
 elsa = "1.7"
 memmap2 = "0.5"
 once_cell = "1"
 same-file = "1"
 siphasher = "0.3"
```

### Comparing `typst-0.1.4/.github/workflows/CI.yml` & `typst-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/.gitignore` & `typst-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/LICENSE` & `typst-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/README.md` & `typst-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/DejaVuSansMono-Bold.ttf` & `typst-0.2.0/python/typst/fonts/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf` & `typst-0.2.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/DejaVuSansMono-Oblique.ttf` & `typst-0.2.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/DejaVuSansMono.ttf` & `typst-0.2.0/python/typst/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/LinLibertine_R.ttf` & `typst-0.2.0/python/typst/fonts/LinLibertine_R.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/LinLibertine_RB.ttf` & `typst-0.2.0/python/typst/fonts/LinLibertine_RB.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/LinLibertine_RBI.ttf` & `typst-0.2.0/python/typst/fonts/LinLibertine_RBI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/LinLibertine_RI.ttf` & `typst-0.2.0/python/typst/fonts/LinLibertine_RI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/NewCM10-Bold.otf` & `typst-0.2.0/python/typst/fonts/NewCM10-Bold.otf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/NewCM10-BoldItalic.otf` & `typst-0.2.0/python/typst/fonts/NewCM10-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/NewCM10-Italic.otf` & `typst-0.2.0/python/typst/fonts/NewCM10-Italic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/NewCM10-Regular.otf` & `typst-0.2.0/python/typst/fonts/NewCM10-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/NewCMMath-Book.otf` & `typst-0.2.0/python/typst/fonts/NewCMMath-Book.otf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/python/typst/fonts/NewCMMath-Regular.otf` & `typst-0.2.0/python/typst/fonts/NewCMMath-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/src/compiler.rs` & `typst-0.2.0/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/src/lib.rs` & `typst-0.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typst-0.1.4/Cargo.lock` & `typst-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,39 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chinese-number"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "365a2e504d6cb41e85fba5d01a6baf7f13cad4424102859193c4674e7fdff933"
+dependencies = [
+ "chinese-numerals",
+ "chinese-variant",
+ "enum-ordinalize",
+ "num-bigint",
+ "num-traits",
+]
+
+[[package]]
+name = "chinese-numerals"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76a5a40575256b55eebe3e39fa41e53bdaea5d67ac5a7092fa8756020c798d1e"
+
+[[package]]
+name = "chinese-variant"
+version = "1.0.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aeea139b89efab957972956e5d3e4efb66a6c261f726abf6911040cc8ef700f7"
+
+[[package]]
 name = "chrono"
 version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
  "num-integer",
  "num-traits",
@@ -228,24 +253,47 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e0aca8dce8856e420195bd13b6a64de3334235ccc9214e824b86b12bf26283"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
+name = "enum-ordinalize"
+version = "3.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a62bb1df8b45ecb7ffa78dca1c17a438fb193eb083db0b1b494d2a61bcb5096a"
+dependencies = [
+ "num-bigint",
+ "num-traits",
+ "proc-macro2",
+ "quote",
+ "rustc_version",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "fancy-regex"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d6b8560a05112eb52f04b00e5d3790c0dd75d9d980eb8a122fb23b92a623ccf"
 dependencies = [
  "bit-set",
  "regex",
 ]
 
 [[package]]
+name = "fdeflate"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
+dependencies = [
+ "simd-adler32",
+]
+
+[[package]]
 name = "flate2"
 version = "1.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
 dependencies = [
  "crc32fast",
  "miniz_oxide 0.6.2",
@@ -518,14 +566,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+ "simd-adler32",
+]
+
+[[package]]
+name = "num-bigint"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
@@ -640,22 +709,23 @@
 checksum = "9eefadd393715fe315c8cdcd587f893b818a6dfe4f6f9faeb44b764c7c38fd8b"
 dependencies = [
  "ttf-parser 0.18.1",
 ]
 
 [[package]]
 name = "png"
-version = "0.17.7"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d708eaf860a19b19ce538740d2b4bdeeb8337fa53f7738455e706623ad5c638"
+checksum = "aaeebc51f9e7d2c150d3f3bfeb667f2aa985db5ef1e3d212847bdedb488beeaa"
 dependencies = [
  "bitflags",
  "crc32fast",
+ "fdeflate",
  "flate2",
- "miniz_oxide 0.6.2",
+ "miniz_oxide 0.7.1",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
@@ -838,14 +908,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "921904a62e410e37e215c40381b7117f830d9d89ba60ab5236170541dd25646b"
 dependencies = [
  "xmlparser",
 ]
 
 [[package]]
+name = "rustc_version"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver",
+]
+
+[[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "rustybuzz"
@@ -890,31 +969,37 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "semver"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+
+[[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.14",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
@@ -933,14 +1018,20 @@
  "indexmap",
  "ryu",
  "serde",
  "yaml-rust",
 ]
 
 [[package]]
+name = "simd-adler32"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "238abfbb77c1915110ad968465608b68e869e0772622c9656714e73e5a1a522f"
+
+[[package]]
 name = "simplecss"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a11be7c62927d9427e9f40f3444d5499d868648e2edbc4e2116de69e7ec0e89d"
 dependencies = [
  "log",
 ]
@@ -1021,17 +1112,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "fcf316d5356ed6847742d036f8a39c3b8435cac10bd528a4bd461928a6ab34d5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1080,15 +1171,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.14",
 ]
 
 [[package]]
 name = "tiny-skia"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d049bfef0eaa2521e75d9ffb5ce86ad54480932ae19b85f78bec6f52c4d30d78"
@@ -1141,24 +1232,25 @@
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typst"
-version = "0.1.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.1.0#b3faef4b80a674294091066e20501e3a5d0f6103"
+version = "0.2.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.2.0#fe2640c55268f167d8749f77b37e52b7b17f21dd"
 dependencies = [
  "bitflags",
  "bytemuck",
  "comemo",
  "ecow",
  "flate2",
  "if_chain",
  "image",
+ "indexmap",
  "log",
  "miniz_oxide 0.5.4",
  "once_cell",
  "pdf-writer",
  "pixglyph",
  "regex",
  "resvg",
@@ -1178,17 +1270,18 @@
  "unscanny",
  "usvg",
  "xmp-writer",
 ]
 
 [[package]]
 name = "typst-library"
-version = "0.1.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.1.0#b3faef4b80a674294091066e20501e3a5d0f6103"
+version = "0.2.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.2.0#fe2640c55268f167d8749f77b37e52b7b17f21dd"
 dependencies = [
+ "chinese-number",
  "comemo",
  "csv",
  "ecow",
  "hayagriva",
  "hypher",
  "kurbo",
  "lipsum",
@@ -1208,27 +1301,27 @@
  "unicode-script",
  "unicode-segmentation",
  "xi-unicode",
 ]
 
 [[package]]
 name = "typst-macros"
-version = "0.1.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.1.0#b3faef4b80a674294091066e20501e3a5d0f6103"
+version = "0.2.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.2.0#fe2640c55268f167d8749f77b37e52b7b17f21dd"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "unscanny",
 ]
 
 [[package]]
 name = "typst-py"
-version = "0.1.4"
+version = "0.2.0"
 dependencies = [
  "comemo",
  "dirs",
  "elsa",
  "memmap2",
  "once_cell",
  "pyo3",
```

### Comparing `typst-0.1.4/PKG-INFO` & `typst-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst
-Version: 0.1.4
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python binding to typst
 License: Apache-2.0
 Requires-Python: >=3.7
```

