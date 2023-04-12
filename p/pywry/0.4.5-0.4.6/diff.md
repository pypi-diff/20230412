# Comparing `tmp/pywry-0.4.5.tar.gz` & `tmp/pywry-0.4.6.tar.gz`

## Comparing `pywry-0.4.5.tar` & `pywry-0.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 pywry-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 pywry-0.4.5/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     2367 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     2149 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/src/websocket.rs
--rw-r--r--   0     1001      123    19797 2023-04-02 18:22:30.000000 pywry-0.4.5/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    62168 2023-04-02 18:22:30.000000 pywry-0.4.5/Cargo.lock
--rw-r--r--   0     1001      123      180 2023-04-02 18:22:30.000000 pywry-0.4.5/python/pywry/__init__.py
--rw-r--r--   0     1001      123    10581 2023-04-02 18:22:30.000000 pywry-0.4.5/python/pywry/core.py
--rw-r--r--   0     1001      123      370 2023-04-02 18:22:30.000000 pywry-0.4.5/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      832 2023-04-02 18:22:30.000000 pywry-0.4.5/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-04-02 18:22:30.000000 pywry-0.4.5/python/pywry/py.typed
--rw-r--r--   0     1001      123      777 2023-04-02 18:22:30.000000 pywry-0.4.5/Cargo.toml
--rw-r--r--   0     1001      123     2149 2023-04-02 18:22:30.000000 pywry-0.4.5/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-02 18:22:30.000000 pywry-0.4.5/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-02 18:22:30.000000 pywry-0.4.5/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-02 18:22:30.000000 pywry-0.4.5/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-02 18:22:30.000000 pywry-0.4.5/src/websocket.rs
--rw-r--r--   0     1001      123    19797 2023-04-02 18:22:30.000000 pywry-0.4.5/src/window.rs
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 pywry-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 pywry-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 pywry-0.4.6/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     2585 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     2149 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/websocket.rs
+-rw-r--r--   0     1001      123    19854 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    60685 2023-04-12 13:45:08.000000 pywry-0.4.6/Cargo.lock
+-rw-r--r--   0     1001      123    10581 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/core.py
+-rw-r--r--   0     1001      123      832 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/backend.py
+-rw-r--r--   0     1001      123      370 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      180 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/py.typed
+-rw-r--r--   0     1001      123      778 2023-04-12 13:45:08.000000 pywry-0.4.6/Cargo.toml
+-rw-r--r--   0     1001      123     2149 2023-04-12 13:45:08.000000 pywry-0.4.6/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-04-12 13:45:08.000000 pywry-0.4.6/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-04-12 13:45:08.000000 pywry-0.4.6/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-04-12 13:45:08.000000 pywry-0.4.6/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-04-12 13:45:08.000000 pywry-0.4.6/src/websocket.rs
+-rw-r--r--   0     1001      123    19854 2023-04-12 13:45:08.000000 pywry-0.4.6/src/window.rs
+-rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 pywry-0.4.6/PKG-INFO
```

### Comparing `pywry-0.4.5/pyproject.toml` & `pywry-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywry"
-version = "0.4.5"
+version = "0.4.6"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `pywry-0.4.5/rust_src/pywry/Cargo.toml` & `pywry-0.4.6/rust_src/pywry/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.4.5"
+version = "0.4.6"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
@@ -13,15 +13,15 @@
 
 
 [dependencies]
 pyo3 = { version = "0.18.0", features = [
     "extension-module",
     "generate-import-lib",
 ] }
-wry = { version = "0.23", features = ["devtools"] }
+wry = { version = "^0.27", features = ["devtools"] }
 image = { version = "^0.24.5", default-features = false, features = ["png"] }
 tokio-tungstenite = "^0.18"
 tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread"] }
 futures-util = { version = "^0.3.25" }
 serde = { version = "^1.0", features = ["derive"] }
 serde_json = "^1.0"
 mime_guess = "^2.0"
```

### Comparing `pywry-0.4.5/rust_src/pywry/LICENSE` & `pywry-0.4.6/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/rust_src/pywry/README.md` & `pywry-0.4.6/rust_src/pywry/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -49,29 +49,38 @@
 ### Linux
 
 Tao uses [gtk-rs](https://gtk-rs.org/) and its related libraries for window creation and wry also needs [WebKitGTK](https://webkitgtk.org/) for WebView. So please make sure the following packages are installed:
 
 #### Arch Linux / Manjaro
 
 ```bash
-sudo pacman -S webkit2gtk-4.0
+sudo pacman -S webkit2gtk
 ```
 
 #### Debian / Ubuntu
 
 ```bash
 sudo apt install libwebkit2gtk-4.0-dev
 ```
 
 #### Fedora / CentOS / AlmaLinux
 
 ```bash
-sudo dnf install gtk3-devel webkit2gtk4.0-devel
+sudo dnf install gtk3-devel webkit2gtk3-devel
 ```
 
 ### macOS
 
 WebKit is native to macOS, so no additional dependencies are needed.
 
 ### Windows
 
 WebView2 provided by Microsoft Edge Chromium is used. So wry supports Windows 7, 8, 10 and 11.
+
+
+## Troubleshooting
+
+### Linux
+
+#### `"/lib/x86_64-linux-gnu/libgio-2.0.so.0: undefined symbol: g_module_open_full"`
+
+This is a known issue with the `gio` library. You can fix it by installing the `libglib2.0-dev` package.
```

### Comparing `pywry-0.4.5/rust_src/pywry/src/constants.rs` & `pywry-0.4.6/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/rust_src/pywry/src/lib.rs` & `pywry-0.4.6/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/rust_src/pywry/src/structs.rs` & `pywry-0.4.6/rust_src/pywry/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/rust_src/pywry/src/websocket.rs` & `pywry-0.4.6/rust_src/pywry/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/rust_src/pywry/src/window.rs` & `pywry-0.4.6/rust_src/pywry/src/window.rs`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     } else {
         content
     };
 
     let mut pre_window = WindowBuilder::new()
         .with_title(to_show.title)
         .with_window_icon(get_icon(&window_icon))
+        .with_min_inner_size(LogicalSize::new(800, 450))
         .with_theme(Some(Theme::Dark));
 
     if to_show.height.is_some() && to_show.width.is_some() {
         pre_window = pre_window.with_inner_size(LogicalSize::new(
             to_show.width.unwrap_or(800) + 80,
             to_show.height.unwrap_or(600) + 80,
         ));
```

### Comparing `pywry-0.4.5/Cargo.lock` & `pywry-0.4.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -21,34 +21,34 @@
 name = "anyhow"
 version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
 
 [[package]]
 name = "atk"
-version = "0.15.1"
+version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c3d816ce6f0e2909a96830d6911c2aff044370b1ef92d7f267b43bae5addedd"
+checksum = "39991bc421ddf72f70159011b323ff49b0f783cc676a7287c59453da2e2531cf"
 dependencies = [
  "atk-sys",
  "bitflags",
  "glib",
  "libc",
 ]
 
 [[package]]
 name = "atk-sys"
-version = "0.15.1"
+version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58aeb089fb698e06db8089971c7ee317ab9644bade33383f63631437b03aafb6"
+checksum = "11ad703eb64dc058024f0e57ccfa069e15a413b98dbd50a1a950e743b7f11148"
 dependencies = [
  "glib-sys",
  "gobject-sys",
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -96,34 +96,35 @@
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cairo-rs"
-version = "0.15.12"
+version = "0.16.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c76ee391b03d35510d9fa917357c7f1855bd9a6659c95a1b392e33f49b3369bc"
+checksum = "f3125b15ec28b84c238f6f476c6034016a5f6cc0221cb514ca46c532139fc97d"
 dependencies = [
  "bitflags",
  "cairo-sys-rs",
  "glib",
  "libc",
+ "once_cell",
  "thiserror",
 ]
 
 [[package]]
 name = "cairo-sys-rs"
-version = "0.15.1"
+version = "0.16.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c55d429bef56ac9172d25fecb85dc8068307d17acd74b377866b7a1ef25d3c8"
+checksum = "7c48f4af05fabdcfa9658178e1326efa061853f040ce7d72e33af6885196f421"
 dependencies = [
  "glib-sys",
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
 ]
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
@@ -132,23 +133,14 @@
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
 
 [[package]]
 name = "cfg-expr"
-version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3431df59f28accaf4cb4eed4a9acc66bea3f3c3753aa6cdc2f024174ef232af7"
-dependencies = [
- "smallvec",
-]
-
-[[package]]
-name = "cfg-expr"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0357a6402b295ca3a86bc148e84df46c02e41f41fef186bda662557ef6328aa"
 dependencies = [
  "smallvec",
 ]
 
@@ -513,81 +505,95 @@
 checksum = "c31b6d751ae2c7f11320402d34e41349dd1016f8d5d45e48c4312bc8625af50c"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "gdk"
-version = "0.15.4"
+version = "0.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6e05c1f572ab0e1f15be94217f0dc29088c248b14f792a5ff0af0d84bcda9e8"
+checksum = "aa9cb33da481c6c040404a11f8212d193889e9b435db2c14fd86987f630d3ce1"
 dependencies = [
  "bitflags",
  "cairo-rs",
  "gdk-pixbuf",
  "gdk-sys",
  "gio",
  "glib",
  "libc",
  "pango",
 ]
 
 [[package]]
 name = "gdk-pixbuf"
-version = "0.15.11"
+version = "0.16.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad38dd9cc8b099cceecdf41375bb6d481b1b5a7cd5cd603e10a69a9383f8619a"
+checksum = "c3578c60dee9d029ad86593ed88cb40f35c1b83360e12498d055022385dd9a05"
 dependencies = [
  "bitflags",
  "gdk-pixbuf-sys",
  "gio",
  "glib",
  "libc",
 ]
 
 [[package]]
 name = "gdk-pixbuf-sys"
-version = "0.15.10"
+version = "0.16.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "140b2f5378256527150350a8346dbdb08fadc13453a7a2d73aecd5fab3c402a7"
+checksum = "3092cf797a5f1210479ea38070d9ae8a5b8e9f8f1be9f32f4643c529c7d70016"
 dependencies = [
  "gio-sys",
  "glib-sys",
  "gobject-sys",
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
 ]
 
 [[package]]
 name = "gdk-sys"
-version = "0.15.1"
+version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32e7a08c1e8f06f4177fb7e51a777b8c1689f743a7bc11ea91d44d2226073a88"
+checksum = "d76354f97a913e55b984759a997b693aa7dc71068c9e98bcce51aa167a0a5c5a"
 dependencies = [
  "cairo-sys-rs",
  "gdk-pixbuf-sys",
  "gio-sys",
  "glib-sys",
  "gobject-sys",
  "libc",
  "pango-sys",
  "pkg-config",
- "system-deps 6.0.3",
+ "system-deps",
+]
+
+[[package]]
+name = "gdkwayland-sys"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4511710212ed3020b61a8622a37aa6f0dd2a84516575da92e9b96928dcbe83ba"
+dependencies = [
+ "gdk-sys",
+ "glib-sys",
+ "gobject-sys",
+ "libc",
+ "pkg-config",
+ "system-deps",
 ]
 
 [[package]]
 name = "gdkx11-sys"
-version = "0.15.1"
+version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4b7f8c7a84b407aa9b143877e267e848ff34106578b64d1e0a24bf550716178"
+checksum = "9fa2bf8b5b8c414bc5d05e48b271896d0fd3ddb57464a3108438082da61de6af"
 dependencies = [
  "gdk-sys",
  "glib-sys",
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
  "x11",
 ]
 
 [[package]]
 name = "generic-array"
 version = "0.14.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -617,103 +623,108 @@
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "gio"
-version = "0.15.12"
+version = "0.16.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68fdbc90312d462781a395f7a16d96a2b379bb6ef8cd6310a2df272771c4283b"
+checksum = "2a1c84b4534a290a29160ef5c6eff2a9c95833111472e824fc5cb78b513dd092"
 dependencies = [
  "bitflags",
  "futures-channel",
  "futures-core",
  "futures-io",
+ "futures-util",
  "gio-sys",
  "glib",
  "libc",
  "once_cell",
+ "pin-project-lite",
+ "smallvec",
  "thiserror",
 ]
 
 [[package]]
 name = "gio-sys"
-version = "0.15.10"
+version = "0.16.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32157a475271e2c4a023382e9cab31c4584ee30a97da41d3c4e9fdd605abcf8d"
+checksum = "e9b693b8e39d042a95547fc258a7b07349b1f0b48f4b2fa3108ba3c51c0b5229"
 dependencies = [
  "glib-sys",
  "gobject-sys",
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
  "winapi",
 ]
 
 [[package]]
 name = "glib"
-version = "0.15.12"
+version = "0.16.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edb0306fbad0ab5428b0ca674a23893db909a98582969c9b537be4ced78c505d"
+checksum = "ddd4df61a866ed7259d6189b8bcb1464989a77f1d85d25d002279bbe9dd38b2f"
 dependencies = [
  "bitflags",
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-task",
+ "futures-util",
+ "gio-sys",
  "glib-macros",
  "glib-sys",
  "gobject-sys",
  "libc",
  "once_cell",
  "smallvec",
  "thiserror",
 ]
 
 [[package]]
 name = "glib-macros"
-version = "0.15.13"
+version = "0.16.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10c6ae9f6fa26f4fb2ac16b528d138d971ead56141de489f8111e259b9df3c4a"
+checksum = "fb1a9325847aa46f1e96ffea37611b9d51fc4827e67f79e7de502a297560a67b"
 dependencies = [
  "anyhow",
- "heck 0.4.1",
+ "heck",
  "proc-macro-crate",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "glib-sys"
-version = "0.15.10"
+version = "0.16.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef4b192f8e65e9cf76cbf4ea71fa8e3be4a0e18ffe3d68b8da6836974cc5bad4"
+checksum = "c61a4f46316d06bfa33a7ac22df6f0524c8be58e3db2d9ca99ccb1f357b62a65"
 dependencies = [
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
 ]
 
 [[package]]
 name = "gobject-sys"
-version = "0.15.10"
+version = "0.16.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d57ce44246becd17153bd035ab4d32cfee096a657fc01f2231c9278378d1e0a"
+checksum = "3520bb9c07ae2a12c7f2fbb24d4efc11231c8146a86956413fb1a79bb760a0f1"
 dependencies = [
  "glib-sys",
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
 ]
 
 [[package]]
 name = "gtk"
-version = "0.15.5"
+version = "0.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92e3004a2d5d6d8b5057d2b57b3712c9529b62e82c77f25c1fecde1fd5c23bd0"
+checksum = "e4d3507d43908c866c805f74c9dd593c0ce7ba5c38e576e41846639cdcd4bee6"
 dependencies = [
  "atk",
  "bitflags",
  "cairo-rs",
  "field-offset",
  "futures-channel",
  "gdk",
@@ -726,35 +737,35 @@
  "once_cell",
  "pango",
  "pkg-config",
 ]
 
 [[package]]
 name = "gtk-sys"
-version = "0.15.3"
+version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5bc2f0587cba247f60246a0ca11fe25fb733eabc3de12d1965fc07efab87c84"
+checksum = "89b5f8946685d5fe44497007786600c2f368ff6b1e61a16251c89f72a97520a3"
 dependencies = [
  "atk-sys",
  "cairo-sys-rs",
  "gdk-pixbuf-sys",
  "gdk-sys",
  "gio-sys",
  "glib-sys",
  "gobject-sys",
  "libc",
  "pango-sys",
- "system-deps 6.0.3",
+ "system-deps",
 ]
 
 [[package]]
 name = "gtk3-macros"
-version = "0.15.6"
+version = "0.16.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "684c0456c086e8e7e9af73ec5b84e35938df394712054550e81558d21c44ab0d"
+checksum = "096eb63c6fedf03bafe65e5924595785eaf1bcb7200dac0f2cbe9c9738f05ad8"
 dependencies = [
  "anyhow",
  "proc-macro-crate",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
@@ -764,23 +775,14 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "heck"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
-dependencies = [
- "unicode-segmentation",
-]
-
-[[package]]
-name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
 version = "0.2.6"
@@ -880,33 +882,33 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "javascriptcore-rs"
-version = "0.16.0"
+version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf053e7843f2812ff03ef5afe34bb9c06ffee120385caad4f6b9967fcd37d41c"
+checksum = "110b9902c80c12bf113c432d0b71c7a94490b294a8234f326fd0abca2fac0b00"
 dependencies = [
  "bitflags",
  "glib",
  "javascriptcore-rs-sys",
 ]
 
 [[package]]
 name = "javascriptcore-rs-sys"
-version = "0.4.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "905fbb87419c5cde6e3269537e4ea7d46431f3008c5d057e915ef3f115e7793c"
+checksum = "98a216519a52cd941a733a0ad3f1023cfdb1cd47f3955e8e863ed56f558f916c"
 dependencies = [
  "glib-sys",
  "gobject-sys",
  "libc",
- "system-deps 5.0.0",
+ "system-deps",
 ]
 
 [[package]]
 name = "jni"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "039022cdf4d7b1cf548d31f60ae783138e5fd42013f6271049d7df7afadef96c"
@@ -1188,35 +1190,36 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "pango"
-version = "0.15.10"
+version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22e4045548659aee5313bde6c582b0d83a627b7904dd20dc2d9ef0895d414e4f"
+checksum = "cdff66b271861037b89d028656184059e03b0b6ccb36003820be19f7200b1e94"
 dependencies = [
  "bitflags",
+ "gio",
  "glib",
  "libc",
  "once_cell",
  "pango-sys",
 ]
 
 [[package]]
 name = "pango-sys"
-version = "0.15.10"
+version = "0.16.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2a00081cde4661982ed91d80ef437c20eacaf6aa1a5962c0279ae194662c3aa"
+checksum = "9e134909a9a293e04d2cc31928aa95679c5e4df954d0b85483159bd20d8f047f"
 dependencies = [
  "glib-sys",
  "gobject-sys",
  "libc",
- "system-deps 6.0.3",
+ "system-deps",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
@@ -1235,20 +1238,14 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
-name = "paste"
-version = "1.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
-
-[[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "phf"
@@ -1482,15 +1479,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.4.5"
+version = "0.4.6"
 dependencies = [
  "futures-util",
  "image",
  "mime_guess",
  "pyo3",
  "serde",
  "serde_json",
@@ -1769,39 +1766,39 @@
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
-name = "soup2"
-version = "0.2.1"
+name = "soup3"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2b4d76501d8ba387cf0fefbe055c3e0a59891d09f0f995ae4e4b16f6b60f3c0"
+checksum = "82bc46048125fefd69d30b32b9d263d6556c9ffe82a7a7df181a86d912da5616"
 dependencies = [
  "bitflags",
+ "futures-channel",
  "gio",
  "glib",
  "libc",
  "once_cell",
- "soup2-sys",
+ "soup3-sys",
 ]
 
 [[package]]
-name = "soup2-sys"
-version = "0.2.0"
+name = "soup3-sys"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "009ef427103fcb17f802871647a7fa6c60cbb654b4c4e4c0ac60a31c5f6dc9cf"
+checksum = "014bbeb1c4cdb30739dc181e8d98b7908f124d9555843afa89b5570aaf4ec62b"
 dependencies = [
- "bitflags",
  "gio-sys",
  "glib-sys",
  "gobject-sys",
  "libc",
- "system-deps 5.0.0",
+ "system-deps",
 ]
 
 [[package]]
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
@@ -1852,55 +1849,43 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "system-deps"
-version = "5.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18db855554db7bd0e73e06cf7ba3df39f97812cb11d3f75e71c39bf45171797e"
-dependencies = [
- "cfg-expr 0.9.1",
- "heck 0.3.3",
- "pkg-config",
- "toml",
- "version-compare 0.0.11",
-]
-
-[[package]]
-name = "system-deps"
 version = "6.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2955b1fe31e1fa2fbd1976b71cc69a606d7d4da16f6de3333d0c92d51419aeff"
 dependencies = [
- "cfg-expr 0.11.0",
- "heck 0.4.1",
+ "cfg-expr",
+ "heck",
  "pkg-config",
  "toml",
- "version-compare 0.1.1",
+ "version-compare",
 ]
 
 [[package]]
 name = "tao"
-version = "0.15.8"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac8e6399427c8494f9849b58694754d7cc741293348a6836b6c8d2c5aa82d8e6"
+checksum = "8f2340617d383561b0ea25358b97ec2c2ba04db48c458ce71dd1b38d7fd09ac5"
 dependencies = [
  "bitflags",
  "cairo-rs",
  "cc",
  "cocoa",
  "core-foundation",
  "core-graphics",
  "crossbeam-channel",
  "dispatch",
  "gdk",
  "gdk-pixbuf",
  "gdk-sys",
+ "gdkwayland-sys",
  "gdkx11-sys",
  "gio",
  "glib",
  "glib-sys",
  "gtk",
  "image",
  "instant",
@@ -1910,27 +1895,38 @@
  "log",
  "ndk",
  "ndk-context",
  "ndk-sys",
  "objc",
  "once_cell",
  "parking_lot",
- "paste",
  "png",
  "raw-window-handle",
  "scopeguard",
  "serde",
+ "tao-macros",
  "unicode-segmentation",
  "uuid",
  "windows",
  "windows-implement",
  "x11-dl",
 ]
 
 [[package]]
+name = "tao-macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b27a4bcc5eb524658234589bdffc7e7bfb996dbae6ce9393bfd39cb4159b445"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "tendril"
@@ -2136,20 +2132,14 @@
 checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
 dependencies = [
  "getrandom 0.2.8",
 ]
 
 [[package]]
 name = "version-compare"
-version = "0.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c18c859eead79d8b95d09e4678566e8d70105c4e7b251f707a03df32442661b"
-
-[[package]]
-name = "version-compare"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "579a42fc0b8e0c63b76519a339be31bed574929511fa53c1a3acae26eb258f29"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
@@ -2176,17 +2166,17 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "webkit2gtk"
-version = "0.18.2"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8f859735e4a452aeb28c6c56a852967a8a76c8eb1cc32dbf931ad28a13d6370"
+checksum = "d8eea819afe15eb8dcdff4f19d8bfda540bae84d874c10e6f4b8faf2d6704bd1"
 dependencies = [
  "bitflags",
  "cairo-rs",
  "gdk",
  "gdk-sys",
  "gio",
  "gio-sys",
@@ -2194,46 +2184,43 @@
  "glib-sys",
  "gobject-sys",
  "gtk",
  "gtk-sys",
  "javascriptcore-rs",
  "libc",
  "once_cell",
- "soup2",
+ "soup3",
  "webkit2gtk-sys",
 ]
 
 [[package]]
 name = "webkit2gtk-sys"
-version = "0.18.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d76ca6ecc47aeba01ec61e480139dda143796abcae6f83bcddf50d6b5b1dcf3"
+checksum = "d0ac7a95ddd3fdfcaf83d8e513b4b1ad101b95b413b6aa6662ed95f284fc3d5b"
 dependencies = [
- "atk-sys",
  "bitflags",
  "cairo-sys-rs",
- "gdk-pixbuf-sys",
  "gdk-sys",
  "gio-sys",
  "glib-sys",
  "gobject-sys",
  "gtk-sys",
  "javascriptcore-rs-sys",
  "libc",
- "pango-sys",
  "pkg-config",
- "soup2-sys",
- "system-deps 6.0.3",
+ "soup3-sys",
+ "system-deps",
 ]
 
 [[package]]
 name = "webview2-com"
-version = "0.19.1"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4a769c9f1a64a8734bde70caafac2b96cada12cd4aefa49196b3a386b8b4178"
+checksum = "11296e5daf3a653b79bf47d66c380e4143d5b9c975818871179a3bda79499562"
 dependencies = [
  "webview2-com-macros",
  "webview2-com-sys",
  "windows",
  "windows-implement",
 ]
 
@@ -2246,17 +2233,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "webview2-com-sys"
-version = "0.19.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aac48ef20ddf657755fdcda8dfed2a7b4fc7e4581acce6fe9b88c3d64f29dee7"
+checksum = "cde542bed28058a5b028d459689ee57f1d06685bb6c266da3b91b1be6703952f"
 dependencies = [
  "regex",
  "serde",
  "serde_json",
  "thiserror",
  "windows",
  "windows-bindgen",
@@ -2292,51 +2279,60 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.39.0"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1c4bd0a50ac6020f65184721f758dba47bb9fbc2133df715ec74a237b26794a"
+checksum = "9e745dab35a0c4c77aa3ce42d595e13d2003d6902d6b08c9ef5fc326d08da12b"
 dependencies = [
  "windows-implement",
- "windows_aarch64_msvc 0.39.0",
- "windows_i686_gnu 0.39.0",
- "windows_i686_msvc 0.39.0",
- "windows_x86_64_gnu 0.39.0",
- "windows_x86_64_msvc 0.39.0",
+ "windows-interface",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-bindgen"
-version = "0.39.0"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68003dbd0e38abc0fb85b939240f4bce37c43a5981d3df37ccbaaa981b47cb41"
+checksum = "222204ecf46521382a4d88b4a1bbefca9f8855697b4ab7d20803901425e061a3"
 dependencies = [
  "windows-metadata",
  "windows-tokens",
 ]
 
 [[package]]
 name = "windows-implement"
-version = "0.39.0"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba01f98f509cb5dc05f4e5fc95e535f78260f15fea8fe1a8abdd08f774f1cee7"
+checksum = "6ce87ca8e3417b02dc2a8a22769306658670ec92d78f1bd420d6310a67c245c6"
 dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "windows-interface"
+version = "0.44.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "853f69a591ecd4f810d29f17e902d40e349fb05b0b11fff63b08b826bfe39c7f"
+dependencies = [
+ "proc-macro2",
+ "quote",
  "syn 1.0.109",
- "windows-tokens",
 ]
 
 [[package]]
 name = "windows-metadata"
-version = "0.39.0"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ee5e275231f07c6e240d14f34e1b635bf1faa1c76c57cfd59a5cdb9848e4278"
+checksum = "ee78911e3f4ce32c1ad9d3c7b0bd95389662ad8d8f1a3155688fed70bd96e2b6"
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
@@ -2346,96 +2342,66 @@
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
- "windows_x86_64_msvc 0.42.2",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows-tokens"
-version = "0.39.0"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f838de2fe15fe6bac988e74b798f26499a8b21a9d97edec321e79b28d1d7f597"
+checksum = "fa4251900975a0d10841c5d4bde79c56681543367ef811f3fabb8d1803b0959b"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.39.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec7711666096bd4096ffa835238905bb33fb87267910e154b18b44eaabb340f2"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.39.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "763fc57100a5f7042e3057e7e8d9bdd7860d330070251a73d003563a3bb49e1b"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.39.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7bc7cbfe58828921e10a9f446fcaaf649204dcfe6c1ddd712c5eebae6bda1106"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.39.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6868c165637d653ae1e8dc4d82c25d4f97dd6605eaa8d784b5c6e0ab2a252b65"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.39.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e4d40883ae9cae962787ca76ba76390ffa29214667a111db9e0a1ad8377e809"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "winnow"
 version = "0.3.6"
@@ -2443,40 +2409,41 @@
 checksum = "23d020b441f92996c80d94ae9166e8501e59c7bb56121189dc9eab3bd8216966"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "wry"
-version = "0.23.4"
+version = "0.27.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c1ad8e2424f554cc5bdebe8aa374ef5b433feff817aebabca0389961fc7ef98"
+checksum = "b958a84f347bf8ec2e882b3f767bdb3f7797e89867bb9d6f0d1fe3df26754fe9"
 dependencies = [
  "base64",
  "block",
  "cocoa",
  "core-graphics",
  "crossbeam-channel",
  "dunce",
  "gdk",
  "gio",
  "glib",
  "gtk",
  "html5ever",
  "http",
+ "javascriptcore-rs",
  "kuchiki",
  "libc",
  "log",
  "objc",
  "objc_id",
  "once_cell",
  "serde",
  "serde_json",
  "sha2",
- "soup2",
+ "soup3",
  "tao",
  "thiserror",
  "url",
  "webkit2gtk",
  "webkit2gtk-sys",
  "webview2-com",
  "windows",
```

### Comparing `pywry-0.4.5/python/pywry/core.py` & `pywry-0.4.6/python/pywry/core.py`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/python/pywry/backend.py` & `pywry-0.4.6/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/Cargo.toml` & `pywry-0.4.6/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.4.5"
+version = "0.4.6"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
@@ -13,15 +13,15 @@
 
 
 [dependencies]
 pyo3 = { version = "0.18.0", features = [
     "extension-module",
     "generate-import-lib",
 ] }
-wry = { version = "0.23", features = ["devtools"] }
+wry = { version = "^0.27", features = ["devtools"] }
 image = { version = "^0.24.5", default-features = false, features = ["png"] }
 tokio-tungstenite = "^0.18"
 tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread"] }
 futures-util = { version = "^0.3.25" }
 serde = { version = "^1.0", features = ["derive"] }
 serde_json = "^1.0"
 mime_guess = "^2.0"
```

### Comparing `pywry-0.4.5/src/constants.rs` & `pywry-0.4.6/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/src/lib.rs` & `pywry-0.4.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/src/structs.rs` & `pywry-0.4.6/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/src/websocket.rs` & `pywry-0.4.6/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.5/src/window.rs` & `pywry-0.4.6/src/window.rs`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     } else {
         content
     };
 
     let mut pre_window = WindowBuilder::new()
         .with_title(to_show.title)
         .with_window_icon(get_icon(&window_icon))
+        .with_min_inner_size(LogicalSize::new(800, 450))
         .with_theme(Some(Theme::Dark));
 
     if to_show.height.is_some() && to_show.width.is_some() {
         pre_window = pre_window.with_inner_size(LogicalSize::new(
             to_show.width.unwrap_or(800) + 80,
             to_show.height.unwrap_or(600) + 80,
         ));
```

### Comparing `pywry-0.4.5/PKG-INFO` & `pywry-0.4.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.4.5
+Version: 0.4.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: websockets>=5.0.1
@@ -67,30 +67,39 @@
 ### Linux
 
 Tao uses [gtk-rs](https://gtk-rs.org/) and its related libraries for window creation and wry also needs [WebKitGTK](https://webkitgtk.org/) for WebView. So please make sure the following packages are installed:
 
 #### Arch Linux / Manjaro
 
 ```bash
-sudo pacman -S webkit2gtk-4.0
+sudo pacman -S webkit2gtk
 ```
 
 #### Debian / Ubuntu
 
 ```bash
 sudo apt install libwebkit2gtk-4.0-dev
 ```
 
 #### Fedora / CentOS / AlmaLinux
 
 ```bash
-sudo dnf install gtk3-devel webkit2gtk4.0-devel
+sudo dnf install gtk3-devel webkit2gtk3-devel
 ```
 
 ### macOS
 
 WebKit is native to macOS, so no additional dependencies are needed.
 
 ### Windows
 
 WebView2 provided by Microsoft Edge Chromium is used. So wry supports Windows 7, 8, 10 and 11.
 
+
+## Troubleshooting
+
+### Linux
+
+#### `"/lib/x86_64-linux-gnu/libgio-2.0.so.0: undefined symbol: g_module_open_full"`
+
+This is a known issue with the `gio` library. You can fix it by installing the `libglib2.0-dev` package.
+
```

