# Comparing `tmp/casers-0.1.0.tar.gz` & `tmp/casers-0.2.0.tar.gz`

## Comparing `casers-0.1.0.tar` & `casers-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 casers-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123      932 2023-04-12 07:30:02.000000 casers-0.1.0/.github/ISSUE_TEMPLATE/issue.yaml
--rw-r--r--   0     1001      123      182 2023-04-12 07:30:02.000000 casers-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0     1001      123      411 2023-04-12 07:30:02.000000 casers-0.1.0/.github/workflows/bumpversion.yml
--rw-r--r--   0     1001      123      521 2023-04-12 07:30:02.000000 casers-0.1.0/.github/workflows/check.yml
--rw-r--r--   0     1001      123     2767 2023-04-12 07:30:02.000000 casers-0.1.0/.github/workflows/maturin.yml
--rw-r--r--   0     1001      123      302 2023-04-12 07:30:02.000000 casers-0.1.0/.github/workflows/pr.yml
--rw-r--r--   0     1001      123     1813 2023-04-12 07:30:02.000000 casers-0.1.0/.gitignore
--rw-r--r--   0     1001      123      293 2023-04-12 07:30:02.000000 casers-0.1.0/CHANGELOG.md
--rw-r--r--   0     1001      123      135 2023-04-12 07:30:02.000000 casers-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123     2847 2023-04-12 07:30:02.000000 casers-0.1.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1092 2023-04-12 07:30:02.000000 casers-0.1.0/LICENSE
--rw-r--r--   0     1001      123     1523 2023-04-12 07:30:02.000000 casers-0.1.0/Makefile
--rw-r--r--   0     1001      123      705 2023-04-12 07:30:02.000000 casers-0.1.0/README.md
--rw-r--r--   0     1001      123      103 2023-04-12 07:30:02.000000 casers-0.1.0/casers/__init__.py
--rw-r--r--   0     1001      123       32 2023-04-12 07:30:02.000000 casers-0.1.0/casers/__main__.py
--rw-r--r--   0     1001      123       33 2023-04-12 07:30:02.000000 casers-0.1.0/casers/_casers.pyi
--rw-r--r--   0     1001      123       22 2023-04-12 07:30:02.000000 casers-0.1.0/casers/_version.py
--rw-r--r--   0     1001      123        0 2023-04-12 07:30:02.000000 casers-0.1.0/casers/cli/__init__.py
--rw-r--r--   0     1001      123      360 2023-04-12 07:30:02.000000 casers-0.1.0/casers/cli/app.py
--rw-r--r--   0     1001      123        1 2023-04-12 07:30:02.000000 casers-0.1.0/casers/py.typed
--rw-r--r--   0     1001      123    58149 2023-04-12 07:30:02.000000 casers-0.1.0/poetry.lock
--rw-r--r--   0     1001      123     2836 2023-04-12 07:30:02.000000 casers-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      349 2023-04-12 07:30:02.000000 casers-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-04-12 07:30:02.000000 casers-0.1.0/tests/__init__.py
--rw-r--r--   0     1001      123      220 2023-04-12 07:30:02.000000 casers-0.1.0/tests/test_to_camel.py
--rw-r--r--   0     1001      123     8112 2023-04-12 07:30:37.000000 casers-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 casers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 casers-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      932 2023-04-12 11:35:41.000000 casers-0.2.0/.github/ISSUE_TEMPLATE/issue.yaml
+-rw-r--r--   0     1001      123      182 2023-04-12 11:35:41.000000 casers-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0     1001      123      411 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/bumpversion.yml
+-rw-r--r--   0     1001      123      578 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/check.yml
+-rw-r--r--   0     1001      123     2767 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      123      302 2023-04-12 11:35:41.000000 casers-0.2.0/.github/workflows/pr.yml
+-rw-r--r--   0     1001      123     1813 2023-04-12 11:35:41.000000 casers-0.2.0/.gitignore
+-rw-r--r--   0     1001      123      362 2023-04-12 11:35:41.000000 casers-0.2.0/CHANGELOG.md
+-rw-r--r--   0     1001      123      135 2023-04-12 11:35:41.000000 casers-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123     2847 2023-04-12 11:35:41.000000 casers-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1092 2023-04-12 11:35:41.000000 casers-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1637 2023-04-12 11:35:41.000000 casers-0.2.0/Makefile
+-rw-r--r--   0     1001      123      946 2023-04-12 11:35:41.000000 casers-0.2.0/README.md
+-rw-r--r--   0     1001      123        0 2023-04-12 11:35:41.000000 casers-0.2.0/benches/__init__.py
+-rw-r--r--   0     1001      123      601 2023-04-12 11:35:41.000000 casers-0.2.0/benches/main.py
+-rw-r--r--   0     1001      123      137 2023-04-12 11:35:41.000000 casers-0.2.0/casers/__init__.py
+-rw-r--r--   0     1001      123       32 2023-04-12 11:35:41.000000 casers-0.2.0/casers/__main__.py
+-rw-r--r--   0     1001      123       72 2023-04-12 11:35:41.000000 casers-0.2.0/casers/_casers.pyi
+-rw-r--r--   0     1001      123       22 2023-04-12 11:35:41.000000 casers-0.2.0/casers/_version.py
+-rw-r--r--   0     1001      123        0 2023-04-12 11:35:41.000000 casers-0.2.0/casers/cli/__init__.py
+-rw-r--r--   0     1001      123      360 2023-04-12 11:35:41.000000 casers-0.2.0/casers/cli/app.py
+-rw-r--r--   0     1001      123        1 2023-04-12 11:35:41.000000 casers-0.2.0/casers/py.typed
+-rw-r--r--   0     1001      123      213 2023-04-12 11:35:41.000000 casers-0.2.0/casers/pydantic.py
+-rw-r--r--   0     1001      123    64193 2023-04-12 11:35:41.000000 casers-0.2.0/poetry.lock
+-rw-r--r--   0     1001      123     2959 2023-04-12 11:35:41.000000 casers-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      550 2023-04-12 11:35:41.000000 casers-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-04-12 11:35:41.000000 casers-0.2.0/tests/__init__.py
+-rw-r--r--   0     1001      123      354 2023-04-12 11:35:41.000000 casers-0.2.0/tests/test_pydantic.py
+-rw-r--r--   0     1001      123      496 2023-04-12 11:35:41.000000 casers-0.2.0/tests/test_to_camel.py
+-rw-r--r--   0     1001      123     8112 2023-04-12 11:36:11.000000 casers-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 casers-0.2.0/PKG-INFO
```

### Comparing `casers-0.1.0/.github/ISSUE_TEMPLATE/issue.yaml` & `casers-0.2.0/.github/ISSUE_TEMPLATE/issue.yaml`

 * *Files identical despite different names*

### Comparing `casers-0.1.0/.github/workflows/check.yml` & `casers-0.2.0/.github/workflows/check.yml`

 * *Files 18% similar despite different names*

```diff
@@ -24,7 +24,10 @@
         run: make build-rs
 
       - name: Run linters
         run: make lint
 
       - name: Run test
         run: make test
+
+      - name: Run benchmark
+        run: make benchmark
```

### Comparing `casers-0.1.0/.github/workflows/maturin.yml` & `casers-0.2.0/.github/workflows/maturin.yml`

 * *Files identical despite different names*

### Comparing `casers-0.1.0/.gitignore` & `casers-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `casers-0.1.0/CONTRIBUTING.md` & `casers-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `casers-0.1.0/LICENSE` & `casers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casers-0.1.0/Makefile` & `casers-0.2.0/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .DEFAULT_GOAL := help
-CODE = casers tests
+CODE = casers tests benches
 POETRY_RUN = poetry run
 TEST = $(POETRY_RUN) pytest $(args)
 
 .PHONY: help
 help: ## Show help
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
@@ -12,27 +12,27 @@
 
 .PHONY: install-poetry
 install-poetry:  ## Install poetry
 	pip install poetry
 
 .PHONY: install
 install:  ## Install dependencies
-	poetry install
+	poetry install -E all
 
 .PHONY: install-docs
 install-docs:  ## Install docs dependencies
 	poetry install --only docs
 
 .PHONY: publish
 publish:  ## Publish package
-	@maturin upload
+	@$(POETRY_RUN) maturin upload
 
 .PHONY: build-rs
 build-rs:  ## maturin develop
-	poetry run maturin develop
+	$(POETRY_RUN) maturin develop
 
 .PHONY: test
 test:  ## Test with coverage
 	$(TEST) --cov=./
 
 .PHONY: test-fast
 test-fast:  ## Test until error
@@ -64,7 +64,11 @@
 	$(POETRY_RUN) cz bump
 
 .PHONY: clean
 clean:  ## Clean
 	rm -rf site || true
 	rm -rf dist || true
 	rm -rf htmlcov || true
+
+.PHONY: benchmark
+benchmark:  ## Benchmark
+	$(POETRY_RUN) python -m benches.main
```

### Comparing `casers-0.1.0/README.md` & `casers-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,28 @@
 ```
 poetry add casers
 ```
 
 ## Usage
 
 ```python
-from casers import __version__
+from casers import snake_to_camel
+
+snake_to_camel("some_text") == "someText"
+# True
+```
+
+```python
+from casers.pydantic import SnakeToCamelAliases
+
+class Model(SnakeToCamelAliases):
+    snake_case: str
+
+Model.parse_obj({"snakeCase": "value"}).snake_case == "value"
+# True
 ```
 
 ## License
 
 * [MIT LICENSE](LICENSE)
 
 ## Contribution
```

### Comparing `casers-0.1.0/poetry.lock` & `casers-0.2.0/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -507,14 +507,67 @@
     {file = "prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
 ]
 
 [package.dependencies]
 wcwidth = "*"
 
 [[package]]
+name = "pydantic"
+version = "1.10.7"
+description = "Data validation and settings management using python type hints"
+category = "main"
+optional = true
+python-versions = ">=3.7"
+files = [
+    {file = "pydantic-1.10.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e79e999e539872e903767c417c897e729e015872040e56b96e67968c3b918b2d"},
+    {file = "pydantic-1.10.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:01aea3a42c13f2602b7ecbbea484a98169fb568ebd9e247593ea05f01b884b2e"},
+    {file = "pydantic-1.10.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:516f1ed9bc2406a0467dd777afc636c7091d71f214d5e413d64fef45174cfc7a"},
+    {file = "pydantic-1.10.7-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ae150a63564929c675d7f2303008d88426a0add46efd76c3fc797cd71cb1b46f"},
+    {file = "pydantic-1.10.7-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:ecbbc51391248116c0a055899e6c3e7ffbb11fb5e2a4cd6f2d0b93272118a209"},
+    {file = "pydantic-1.10.7-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:f4a2b50e2b03d5776e7f21af73e2070e1b5c0d0df255a827e7c632962f8315af"},
+    {file = "pydantic-1.10.7-cp310-cp310-win_amd64.whl", hash = "sha256:a7cd2251439988b413cb0a985c4ed82b6c6aac382dbaff53ae03c4b23a70e80a"},
+    {file = "pydantic-1.10.7-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:68792151e174a4aa9e9fc1b4e653e65a354a2fa0fed169f7b3d09902ad2cb6f1"},
+    {file = "pydantic-1.10.7-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:dfe2507b8ef209da71b6fb5f4e597b50c5a34b78d7e857c4f8f3115effaef5fe"},
+    {file = "pydantic-1.10.7-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:10a86d8c8db68086f1e30a530f7d5f83eb0685e632e411dbbcf2d5c0150e8dcd"},
+    {file = "pydantic-1.10.7-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d75ae19d2a3dbb146b6f324031c24f8a3f52ff5d6a9f22f0683694b3afcb16fb"},
+    {file = "pydantic-1.10.7-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:464855a7ff7f2cc2cf537ecc421291b9132aa9c79aef44e917ad711b4a93163b"},
+    {file = "pydantic-1.10.7-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:193924c563fae6ddcb71d3f06fa153866423ac1b793a47936656e806b64e24ca"},
+    {file = "pydantic-1.10.7-cp311-cp311-win_amd64.whl", hash = "sha256:b4a849d10f211389502059c33332e91327bc154acc1845f375a99eca3afa802d"},
+    {file = "pydantic-1.10.7-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:cc1dde4e50a5fc1336ee0581c1612215bc64ed6d28d2c7c6f25d2fe3e7c3e918"},
+    {file = "pydantic-1.10.7-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e0cfe895a504c060e5d36b287ee696e2fdad02d89e0d895f83037245218a87fe"},
+    {file = "pydantic-1.10.7-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:670bb4683ad1e48b0ecb06f0cfe2178dcf74ff27921cdf1606e527d2617a81ee"},
+    {file = "pydantic-1.10.7-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:950ce33857841f9a337ce07ddf46bc84e1c4946d2a3bba18f8280297157a3fd1"},
+    {file = "pydantic-1.10.7-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:c15582f9055fbc1bfe50266a19771bbbef33dd28c45e78afbe1996fd70966c2a"},
+    {file = "pydantic-1.10.7-cp37-cp37m-win_amd64.whl", hash = "sha256:82dffb306dd20bd5268fd6379bc4bfe75242a9c2b79fec58e1041fbbdb1f7914"},
+    {file = "pydantic-1.10.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8c7f51861d73e8b9ddcb9916ae7ac39fb52761d9ea0df41128e81e2ba42886cd"},
+    {file = "pydantic-1.10.7-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:6434b49c0b03a51021ade5c4daa7d70c98f7a79e95b551201fff682fc1661245"},
+    {file = "pydantic-1.10.7-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:64d34ab766fa056df49013bb6e79921a0265204c071984e75a09cbceacbbdd5d"},
+    {file = "pydantic-1.10.7-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:701daea9ffe9d26f97b52f1d157e0d4121644f0fcf80b443248434958fd03dc3"},
+    {file = "pydantic-1.10.7-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:cf135c46099ff3f919d2150a948ce94b9ce545598ef2c6c7bf55dca98a304b52"},
+    {file = "pydantic-1.10.7-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b0f85904f73161817b80781cc150f8b906d521fa11e3cdabae19a581c3606209"},
+    {file = "pydantic-1.10.7-cp38-cp38-win_amd64.whl", hash = "sha256:9f6f0fd68d73257ad6685419478c5aece46432f4bdd8d32c7345f1986496171e"},
+    {file = "pydantic-1.10.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c230c0d8a322276d6e7b88c3f7ce885f9ed16e0910354510e0bae84d54991143"},
+    {file = "pydantic-1.10.7-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:976cae77ba6a49d80f461fd8bba183ff7ba79f44aa5cfa82f1346b5626542f8e"},
+    {file = "pydantic-1.10.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7d45fc99d64af9aaf7e308054a0067fdcd87ffe974f2442312372dfa66e1001d"},
+    {file = "pydantic-1.10.7-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d2a5ebb48958754d386195fe9e9c5106f11275867051bf017a8059410e9abf1f"},
+    {file = "pydantic-1.10.7-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:abfb7d4a7cd5cc4e1d1887c43503a7c5dd608eadf8bc615413fc498d3e4645cd"},
+    {file = "pydantic-1.10.7-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:80b1fab4deb08a8292d15e43a6edccdffa5377a36a4597bb545b93e79c5ff0a5"},
+    {file = "pydantic-1.10.7-cp39-cp39-win_amd64.whl", hash = "sha256:d71e69699498b020ea198468e2480a2f1e7433e32a3a99760058c6520e2bea7e"},
+    {file = "pydantic-1.10.7-py3-none-any.whl", hash = "sha256:0cd181f1d0b1d00e2b705f1bf1ac7799a2d938cce3376b8007df62b29be3c2c6"},
+    {file = "pydantic-1.10.7.tar.gz", hash = "sha256:cfc83c0678b6ba51b0532bea66860617c4cd4251ecf76e9846fa5a9f3454e97e"},
+]
+
+[package.dependencies]
+typing-extensions = ">=4.2.0"
+
+[package.extras]
+dotenv = ["python-dotenv (>=0.10.4)"]
+email = ["email-validator (>=1.0.3)"]
+
+[[package]]
 name = "pytest"
 version = "7.3.0"
 description = "pytest: simple powerful testing with Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -786,15 +839,15 @@
     {file = "typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
 ]
 
 [[package]]
 name = "typing-extensions"
 version = "4.5.0"
 description = "Backported and Experimental Type Hints for Python 3.7+"
-category = "dev"
+category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
     {file = "typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
 ]
 
@@ -822,11 +875,15 @@
     {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
+[extras]
+all = ["pydantic"]
+pydantic = ["pydantic"]
+
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.7"
-content-hash = "c3222020e5df4bb6b895b14a14e8dfebd718a77e6c8a25da502c7f969fa7bf28"
+content-hash = "2d8ea14ebe1151ac35b9546cf833be019a4aab51bbdc3c622a65b04191e634d9"
```

### Comparing `casers-0.1.0/pyproject.toml` & `casers-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.0"
+version = "0.2.0"
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
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/casers"
 homepage = "https://pypi.org/project/casers"
 keywords = []
 
 [tool.poetry.scripts]
 casers = 'casers.cli.app:run'
 
 [tool.poetry.dependencies]
 python = "^3.7"
+pydantic = {version = "^1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 maturin = "^0.14.17"
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
@@ -38,14 +39,18 @@
 pytest-mock = "^3.10.0"
 ruff = "^0.0.255"
 toml = "^0.10.2"
 
 [tool.poetry.group.git.dependencies]
 commitizen = "^2.42.1"
 
+[tool.poetry.extras]
+all = ["pydantic"]
+pydantic = ["pydantic"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "casers"
 requires-python = ">=3.7"
@@ -82,15 +87,15 @@
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 
 [tool.coverage.run]
-omit = ["tests/*", "**/__main__.py", "**/.venv/*", "**/site-packages/*", "casers/cli/*"]
+omit = ["tests/*", "**/__main__.py", "**/.venv/*", "**/site-packages/*", "casers/cli/*", "benches/*"]
 branch = true
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 fail_under = 100
```

### Comparing `casers-0.1.0/Cargo.lock` & `casers-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "casers"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "convert_case",
  "pyo3",
 ]
 
 [[package]]
 name = "cfg-if"
```

