# Comparing `tmp/pywry-0.4.6.tar.gz` & `tmp/pywry-0.4.7.tar.gz`

## Comparing `pywry-0.4.6.tar` & `pywry-0.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 pywry-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 pywry-0.4.6/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     2585 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     2149 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/websocket.rs
--rw-r--r--   0     1001      123    19854 2023-04-12 13:45:08.000000 pywry-0.4.6/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    60685 2023-04-12 13:45:08.000000 pywry-0.4.6/Cargo.lock
--rw-r--r--   0     1001      123    10581 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/core.py
--rw-r--r--   0     1001      123      832 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/backend.py
--rw-r--r--   0     1001      123      370 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      180 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-12 13:45:08.000000 pywry-0.4.6/python/pywry/py.typed
--rw-r--r--   0     1001      123      778 2023-04-12 13:45:08.000000 pywry-0.4.6/Cargo.toml
--rw-r--r--   0     1001      123     2149 2023-04-12 13:45:08.000000 pywry-0.4.6/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-12 13:45:08.000000 pywry-0.4.6/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-12 13:45:08.000000 pywry-0.4.6/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-12 13:45:08.000000 pywry-0.4.6/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-12 13:45:08.000000 pywry-0.4.6/src/websocket.rs
--rw-r--r--   0     1001      123    19854 2023-04-12 13:45:08.000000 pywry-0.4.6/src/window.rs
--rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 pywry-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 pywry-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 pywry-0.4.7/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     2585 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     2149 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/src/websocket.rs
+-rw-r--r--   0     1001      123    20212 2023-04-12 20:54:05.000000 pywry-0.4.7/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    60685 2023-04-12 20:54:05.000000 pywry-0.4.7/Cargo.lock
+-rw-r--r--   0     1001      123    10581 2023-04-12 20:54:05.000000 pywry-0.4.7/python/pywry/core.py
+-rw-r--r--   0     1001      123      832 2023-04-12 20:54:05.000000 pywry-0.4.7/python/pywry/backend.py
+-rw-r--r--   0     1001      123      370 2023-04-12 20:54:05.000000 pywry-0.4.7/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      180 2023-04-12 20:54:05.000000 pywry-0.4.7/python/pywry/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-12 20:54:05.000000 pywry-0.4.7/python/pywry/py.typed
+-rw-r--r--   0     1001      123      778 2023-04-12 20:54:05.000000 pywry-0.4.7/Cargo.toml
+-rw-r--r--   0     1001      123     2149 2023-04-12 20:54:05.000000 pywry-0.4.7/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-04-12 20:54:05.000000 pywry-0.4.7/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-04-12 20:54:05.000000 pywry-0.4.7/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-04-12 20:54:05.000000 pywry-0.4.7/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-04-12 20:54:05.000000 pywry-0.4.7/src/websocket.rs
+-rw-r--r--   0     1001      123    20212 2023-04-12 20:54:05.000000 pywry-0.4.7/src/window.rs
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 pywry-0.4.7/PKG-INFO
```

### Comparing `pywry-0.4.6/pyproject.toml` & `pywry-0.4.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "pywry"
-version = "0.4.6"
+version = "0.4.7"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
 ]
 
-dependencies = ['websockets>=5.0.1', 'psutil>=5.8.0']
+dependencies = ['websockets>=11.0.1', 'psutil>=5.8.0,<5.9.4']
 
 [build-system]
 requires = [
     "setuptools>=58.0.0",
     "wheel",
     "maturin>=0.14,<0.15",
     "toml"
```

### Comparing `pywry-0.4.6/rust_src/pywry/Cargo.toml` & `pywry-0.4.7/rust_src/pywry/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.4.6"
+version = "0.4.7"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.4.6/rust_src/pywry/LICENSE` & `pywry-0.4.7/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/rust_src/pywry/README.md` & `pywry-0.4.7/rust_src/pywry/README.md`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/rust_src/pywry/src/constants.rs` & `pywry-0.4.7/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/rust_src/pywry/src/lib.rs` & `pywry-0.4.7/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/rust_src/pywry/src/structs.rs` & `pywry-0.4.7/rust_src/pywry/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/rust_src/pywry/src/websocket.rs` & `pywry-0.4.7/rust_src/pywry/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/rust_src/pywry/src/window.rs` & `pywry-0.4.7/rust_src/pywry/src/window.rs`

 * *Files 2% similar despite different names*

```diff
@@ -469,41 +469,48 @@
             }
             // WindowEvent::NewWindow
             #[cfg(not(target_os = "windows"))]
             Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
                 if debug {
                     println!("\nNew Window Requested: {}", uri);
                 }
-                let pre_window = WindowBuilder::new()
-                    .with_title(uri.to_string())
-                    .with_window_icon(window_icon)
-                    .with_inner_size(LogicalSize::new(1300, 900))
-                    .with_resizable(true)
-                    .with_theme(Some(Theme::Dark));
-
-                let window = match pre_window.build(event_loop) {
-                    Err(error) => {
-                        println!("Window Creation Error: {}", error);
-                        return;
-                    }
-                    Ok(item) => item,
-                };
+                if uri.starts_with("http://") || uri.starts_with("https://") {
+                    let pre_window = WindowBuilder::new()
+                        .with_title(uri.to_string())
+                        .with_window_icon(window_icon)
+                        .with_inner_size(LogicalSize::new(1300, 900))
+                        .with_resizable(true)
+                        .with_theme(Some(Theme::Dark));
 
-                let window_id = window.id();
+                    let window = match pre_window.build(event_loop) {
+                        Err(error) => {
+                            println!("Window Creation Error: {}", error);
+                            return;
+                        }
+                        Ok(item) => item,
+                    };
 
-                let webview = WebViewBuilder::new(window)
-                    .unwrap()
-                    .with_url(&uri)
-                    .unwrap()
-                    .build()
-                    .unwrap();
+                    let window_id = window.id();
 
-                webviews.insert(window_id, webview);
+                    let webview = WebViewBuilder::new(window)
+                        .unwrap()
+                        .with_url(&uri)
+                        .unwrap()
+                        .build()
+                        .unwrap();
 
-                if debug {
-                    println!("New Window Created");
+                    webviews.insert(window_id, webview);
+
+                    if debug {
+                        println!("New Window Created");
+                    }
+
+                } else {
+                    if debug {
+                        println!("Invalid URI tried to open in new window: {}", uri);
+                    }
                 }
             }
             _ => {}
         }
     });
 }
```

### Comparing `pywry-0.4.6/Cargo.lock` & `pywry-0.4.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1479,15 +1479,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.4.6"
+version = "0.4.7"
 dependencies = [
  "futures-util",
  "image",
  "mime_guess",
  "pyo3",
  "serde",
  "serde_json",
```

### Comparing `pywry-0.4.6/python/pywry/core.py` & `pywry-0.4.7/python/pywry/core.py`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/python/pywry/backend.py` & `pywry-0.4.7/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/Cargo.toml` & `pywry-0.4.7/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.4.6"
+version = "0.4.7"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.4.6/src/constants.rs` & `pywry-0.4.7/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/src/lib.rs` & `pywry-0.4.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/src/structs.rs` & `pywry-0.4.7/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/src/websocket.rs` & `pywry-0.4.7/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.4.6/src/window.rs` & `pywry-0.4.7/src/window.rs`

 * *Files 2% similar despite different names*

```diff
@@ -469,41 +469,48 @@
             }
             // WindowEvent::NewWindow
             #[cfg(not(target_os = "windows"))]
             Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
                 if debug {
                     println!("\nNew Window Requested: {}", uri);
                 }
-                let pre_window = WindowBuilder::new()
-                    .with_title(uri.to_string())
-                    .with_window_icon(window_icon)
-                    .with_inner_size(LogicalSize::new(1300, 900))
-                    .with_resizable(true)
-                    .with_theme(Some(Theme::Dark));
-
-                let window = match pre_window.build(event_loop) {
-                    Err(error) => {
-                        println!("Window Creation Error: {}", error);
-                        return;
-                    }
-                    Ok(item) => item,
-                };
+                if uri.starts_with("http://") || uri.starts_with("https://") {
+                    let pre_window = WindowBuilder::new()
+                        .with_title(uri.to_string())
+                        .with_window_icon(window_icon)
+                        .with_inner_size(LogicalSize::new(1300, 900))
+                        .with_resizable(true)
+                        .with_theme(Some(Theme::Dark));
 
-                let window_id = window.id();
+                    let window = match pre_window.build(event_loop) {
+                        Err(error) => {
+                            println!("Window Creation Error: {}", error);
+                            return;
+                        }
+                        Ok(item) => item,
+                    };
 
-                let webview = WebViewBuilder::new(window)
-                    .unwrap()
-                    .with_url(&uri)
-                    .unwrap()
-                    .build()
-                    .unwrap();
+                    let window_id = window.id();
 
-                webviews.insert(window_id, webview);
+                    let webview = WebViewBuilder::new(window)
+                        .unwrap()
+                        .with_url(&uri)
+                        .unwrap()
+                        .build()
+                        .unwrap();
 
-                if debug {
-                    println!("New Window Created");
+                    webviews.insert(window_id, webview);
+
+                    if debug {
+                        println!("New Window Created");
+                    }
+
+                } else {
+                    if debug {
+                        println!("Invalid URI tried to open in new window: {}", uri);
+                    }
                 }
             }
             _ => {}
         }
     });
 }
```

### Comparing `pywry-0.4.6/PKG-INFO` & `pywry-0.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.4.6
+Version: 0.4.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: websockets>=5.0.1
-Requires-Dist: psutil>=5.8.0
+Requires-Dist: websockets>=11.0.1
+Requires-Dist: psutil>=5.8.0,<5.9.4
 Requires-Dist: auditwheel; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

