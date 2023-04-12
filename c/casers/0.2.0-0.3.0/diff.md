# Comparing `tmp/casers-0.2.0.tar.gz` & `tmp/casers-0.3.0.tar.gz`

## Comparing `casers-0.2.0.tar` & `casers-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 casers-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      932 2023-04-12 11:35:41.000000 casers-0.2.0/.github/ISSUE_TEMPLATE/issue.yaml
--rw-r--r--   0     1001      123      182 2023-04-12 11:35:41.000000 casers-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0     1001      123      411 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/bumpversion.yml
--rw-r--r--   0     1001      123      578 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/check.yml
--rw-r--r--   0     1001      123     2767 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/maturin.yml
--rw-r--r--   0     1001      123      302 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/pr.yml
--rw-r--r--   0     1001      123     1813 2023-04-12 11:35:41.000000 casers-0.2.0/.gitignore
--rw-r--r--   0     1001      123      362 2023-04-12 11:35:41.000000 casers-0.2.0/CHANGELOG.md
--rw-r--r--   0     1001      123      135 2023-04-12 11:35:41.000000 casers-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123     2847 2023-04-12 11:35:41.000000 casers-0.2.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1092 2023-04-12 11:35:41.000000 casers-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1637 2023-04-12 11:35:41.000000 casers-0.2.0/Makefile
--rw-r--r--   0     1001      123      946 2023-04-12 11:35:41.000000 casers-0.2.0/README.md
--rw-r--r--   0     1001      123        0 2023-04-12 11:35:41.000000 casers-0.2.0/benches/__init__.py
--rw-r--r--   0     1001      123      601 2023-04-12 11:35:41.000000 casers-0.2.0/benches/main.py
--rw-r--r--   0     1001      123      137 2023-04-12 11:35:41.000000 casers-0.2.0/casers/__init__.py
--rw-r--r--   0     1001      123       32 2023-04-12 11:35:41.000000 casers-0.2.0/casers/__main__.py
--rw-r--r--   0     1001      123       72 2023-04-12 11:35:41.000000 casers-0.2.0/casers/_casers.pyi
--rw-r--r--   0     1001      123       22 2023-04-12 11:35:41.000000 casers-0.2.0/casers/_version.py
--rw-r--r--   0     1001      123        0 2023-04-12 11:35:41.000000 casers-0.2.0/casers/cli/__init__.py
--rw-r--r--   0     1001      123      360 2023-04-12 11:35:41.000000 casers-0.2.0/casers/cli/app.py
--rw-r--r--   0     1001      123        1 2023-04-12 11:35:41.000000 casers-0.2.0/casers/py.typed
--rw-r--r--   0     1001      123      213 2023-04-12 11:35:41.000000 casers-0.2.0/casers/pydantic.py
--rw-r--r--   0     1001      123    64193 2023-04-12 11:35:41.000000 casers-0.2.0/poetry.lock
--rw-r--r--   0     1001      123     2959 2023-04-12 11:35:41.000000 casers-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      550 2023-04-12 11:35:41.000000 casers-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-04-12 11:35:41.000000 casers-0.2.0/tests/__init__.py
--rw-r--r--   0     1001      123      354 2023-04-12 11:35:41.000000 casers-0.2.0/tests/test_pydantic.py
--rw-r--r--   0     1001      123      496 2023-04-12 11:35:41.000000 casers-0.2.0/tests/test_to_camel.py
--rw-r--r--   0     1001      123     8112 2023-04-12 11:36:11.000000 casers-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 casers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 casers-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      932 2023-04-12 15:40:32.000000 casers-0.3.0/.github/ISSUE_TEMPLATE/issue.yaml
+-rw-r--r--   0     1001      123      182 2023-04-12 15:40:32.000000 casers-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0     1001      123      411 2023-04-12 15:40:32.000000 casers-0.3.0/.github/workflows/bumpversion.yml
+-rw-r--r--   0     1001      123      586 2023-04-12 15:40:32.000000 casers-0.3.0/.github/workflows/check.yml
+-rw-r--r--   0     1001      123     2767 2023-04-12 15:40:32.000000 casers-0.3.0/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      123      302 2023-04-12 15:40:32.000000 casers-0.3.0/.github/workflows/pr.yml
+-rw-r--r--   0     1001      123     1813 2023-04-12 15:40:32.000000 casers-0.3.0/.gitignore
+-rw-r--r--   0     1001      123      420 2023-04-12 15:40:32.000000 casers-0.3.0/CHANGELOG.md
+-rw-r--r--   0     1001      123      135 2023-04-12 15:40:32.000000 casers-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123     2847 2023-04-12 15:40:32.000000 casers-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1092 2023-04-12 15:40:32.000000 casers-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     1758 2023-04-12 15:40:32.000000 casers-0.3.0/Makefile
+-rw-r--r--   0     1001      123      946 2023-04-12 15:40:32.000000 casers-0.3.0/README.md
+-rw-r--r--   0     1001      123        0 2023-04-12 15:40:32.000000 casers-0.3.0/benches/__init__.py
+-rw-r--r--   0     1001      123      607 2023-04-12 15:40:32.000000 casers-0.3.0/benches/main.py
+-rw-r--r--   0     1001      123      137 2023-04-12 15:40:32.000000 casers-0.3.0/casers/__init__.py
+-rw-r--r--   0     1001      123       32 2023-04-12 15:40:32.000000 casers-0.3.0/casers/__main__.py
+-rw-r--r--   0     1001      123       72 2023-04-12 15:40:32.000000 casers-0.3.0/casers/_casers.pyi
+-rw-r--r--   0     1001      123       22 2023-04-12 15:40:32.000000 casers-0.3.0/casers/_version.py
+-rw-r--r--   0     1001      123        0 2023-04-12 15:40:32.000000 casers-0.3.0/casers/cli/__init__.py
+-rw-r--r--   0     1001      123      360 2023-04-12 15:40:32.000000 casers-0.3.0/casers/cli/app.py
+-rw-r--r--   0     1001      123        1 2023-04-12 15:40:32.000000 casers-0.3.0/casers/py.typed
+-rw-r--r--   0     1001      123      213 2023-04-12 15:40:32.000000 casers-0.3.0/casers/pydantic.py
+-rw-r--r--   0     1001      123    64193 2023-04-12 15:40:32.000000 casers-0.3.0/poetry.lock
+-rw-r--r--   0     1001      123     2959 2023-04-12 15:40:32.000000 casers-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     1270 2023-04-12 15:40:32.000000 casers-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-04-12 15:40:32.000000 casers-0.3.0/tests/__init__.py
+-rw-r--r--   0     1001      123      354 2023-04-12 15:40:32.000000 casers-0.3.0/tests/test_pydantic.py
+-rw-r--r--   0     1001      123      602 2023-04-12 15:40:32.000000 casers-0.3.0/tests/test_to_camel.py
+-rw-r--r--   0     1001      123     7650 2023-04-12 15:41:01.000000 casers-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 casers-0.3.0/PKG-INFO
```

### Comparing `casers-0.2.0/.github/ISSUE_TEMPLATE/issue.yaml` & `casers-0.3.0/.github/ISSUE_TEMPLATE/issue.yaml`

 * *Files identical despite different names*

### Comparing `casers-0.2.0/.github/workflows/check.yml` & `casers-0.3.0/.github/workflows/check.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,14 @@
       - name: Install python dependencies
         run: make install-poetry install
 
       - name: Maturin
         run: make build-rs
 
       - name: Run linters
-        run: make lint
+        run: make lint lint-rs
 
       - name: Run test
         run: make test
 
       - name: Run benchmark
         run: make benchmark
```

### Comparing `casers-0.2.0/.github/workflows/maturin.yml` & `casers-0.3.0/.github/workflows/maturin.yml`

 * *Files identical despite different names*

### Comparing `casers-0.2.0/.gitignore` & `casers-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `casers-0.2.0/CONTRIBUTING.md` & `casers-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `casers-0.2.0/LICENSE` & `casers-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casers-0.2.0/Makefile` & `casers-0.3.0/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -23,17 +23,25 @@
 	poetry install --only docs
 
 .PHONY: publish
 publish:  ## Publish package
 	@$(POETRY_RUN) maturin upload
 
 .PHONY: build-rs
-build-rs:  ## maturin develop
+build-rs:  ## Build .so files
 	$(POETRY_RUN) maturin develop
 
+.PHONY: format-rs
+format-rs:  ## Formatting rs code
+	cargo fmt
+
+.PHONY: lint-rs
+lint-rs:  ## Check rs code
+	cargo check
+
 .PHONY: test
 test:  ## Test with coverage
 	$(TEST) --cov=./
 
 .PHONY: test-fast
 test-fast:  ## Test until error
 	$(TEST) --exitfirst
```

### Comparing `casers-0.2.0/README.md` & `casers-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `casers-0.2.0/benches/main.py` & `casers-0.3.0/benches/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 
 def py_snake_to_camel(string: str) -> str:
     components = string.split("_")
     return components[0] + "".join(word.title() for word in components[1:])
 
 
 if __name__ == "__main__":
-    text = "hello_world"
+    text = "hello_world" * 100
     echo(timeit(lambda: snake_to_camel(text), number=10000), "casers.snake_to_camel")
     echo(timeit(lambda: to_camel(text), number=10000), "casers.to_camel")
     echo(timeit(lambda: py_snake_to_camel(text), number=10000), "python")
```

### Comparing `casers-0.2.0/poetry.lock` & `casers-0.3.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `casers-0.2.0/pyproject.toml` & `casers-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0"
+version = "0.3.0"
 tag_format = "$version"
 version_files = [
     "casers/_version.py",
     "Cargo.toml:version",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "casers"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/casers"
 homepage = "https://pypi.org/project/casers"
 keywords = []
```

### Comparing `casers-0.2.0/Cargo.lock` & `casers-0.3.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -12,36 +12,26 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "casers"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
- "convert_case",
  "pyo3",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "convert_case"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
-dependencies = [
- "unicode-segmentation",
-]
-
-[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
@@ -216,20 +206,14 @@
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
-name = "unicode-segmentation"
-version = "1.10.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
-
-[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "windows-sys"
```

### Comparing `casers-0.2.0/PKG-INFO` & `casers-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casers
-Version: 0.2.0
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.7
```

