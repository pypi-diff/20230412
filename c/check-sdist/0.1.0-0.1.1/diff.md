# Comparing `tmp/check_sdist-0.1.0.tar.gz` & `tmp/check_sdist-0.1.1.tar.gz`

## Comparing `check_sdist-0.1.0.tar` & `check_sdist-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 check_sdist-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 check_sdist-0.1.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 check_sdist-0.1.0/noxfile.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 check_sdist-0.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 check_sdist-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 check_sdist-0.1.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 check_sdist-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 check_sdist-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 check_sdist-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/__init__.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/__main__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/git.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/inject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/py.typed
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/sdist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/_compat/__init__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/_compat/importlib.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/_compat/tomllib.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/resources/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/resources/default-ignore.txt
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 check_sdist-0.1.0/src/check_sdist/resources/junk-paths.txt
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 check_sdist-0.1.0/tests/test_inject.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 check_sdist-0.1.0/tests/test_package.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 check_sdist-0.1.0/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 check_sdist-0.1.0/LICENSE
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 check_sdist-0.1.0/README.md
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 check_sdist-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 check_sdist-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 check_sdist-0.1.1/noxfile.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 check_sdist-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 check_sdist-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/__init__.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/__main__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/git.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/inject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/py.typed
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/sdist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/_compat/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/_compat/importlib.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/_compat/tomllib.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/resources/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/resources/default-ignore.txt
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 check_sdist-0.1.1/src/check_sdist/resources/junk-paths.txt
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/downstream.toml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/test_downstream.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/test_inject.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 check_sdist-0.1.1/tests/test_package.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 check_sdist-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 check_sdist-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 check_sdist-0.1.1/README.md
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 check_sdist-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 check_sdist-0.1.1/PKG-INFO
```

### Comparing `check_sdist-0.1.0/.pre-commit-config.yaml` & `check_sdist-0.1.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,26 @@
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.1.1"
     hooks:
       - id: mypy
-        files: src
+        files: src|tests
         args: []
-        additional_dependencies: ["tomli", "pathspec", "importlib-resources"]
+        additional_dependencies:
+          ["tomli", "pathspec", "importlib-resources", "pytest"]
+
+  - repo: https://github.com/henryiii/check-sdist
+    rev: "v0.1.0"
+    hooks:
+      - id: check-sdist
+        args: [--inject-junk]
+        additional_dependencies:
+          - hatchling
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
```

### Comparing `check_sdist-0.1.0/noxfile.py` & `check_sdist-0.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/.github/CONTRIBUTING.md` & `check_sdist-0.1.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/.github/matchers/pylint.json` & `check_sdist-0.1.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/.github/workflows/ci.yml` & `check_sdist-0.1.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -86,11 +86,11 @@
       - uses: actions/upload-artifact@v3
         with:
           path: dist
 
       - name: Check products
         run: pipx run twine check dist/*
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.3
+      - uses: pypa/gh-action-pypi-publish@v1.8.5
         if: github.event_name == 'release' && github.event.action == 'published'
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `check_sdist-0.1.0/docs/conf.py` & `check_sdist-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/src/check_sdist/__main__.py` & `check_sdist-0.1.1/src/check_sdist/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ._compat import tomllib
 from .git import git_files
 from .inject import inject_junk_files
 from .resources import resources
 from .sdist import sdist_files
 
 
-def compare(source_dir: Path, isolated: bool, verbose: bool = False) -> int:
+def compare(source_dir: Path, *, isolated: bool, verbose: bool = False) -> int:
     """
     Compare the files in the SDist with the files tracked by git.
 
     Takes the source directory and a flag indicating whether the SDist should
     be built in an isolated environment.
 
     Return 0 if they match, 1 if the SDist has files that are not tracked by
@@ -37,14 +37,15 @@
     sdist_only_patterns = config.get("sdist-only", [])
     git_only_patterns = config.get("git-only", [])
     default_ignore = config.get("default-ignore", True)
 
     if default_ignore:
         with resources.joinpath("default-ignore.txt").open("r", encoding="utf-8") as f:
             git_only_patterns.extend(f.read().splitlines())
+        sdist_only_patterns.extend("*.dist-info")
 
     sdist_spec = pathspec.GitIgnoreSpec.from_lines(sdist_only_patterns)
     git_spec = pathspec.GitIgnoreSpec.from_lines(git_only_patterns)
 
     sdist_only = frozenset(p for p in sdist - git if not sdist_spec.match_file(p))
     git_only = frozenset(p for p in git - sdist if not git_spec.match_file(p))
 
@@ -95,12 +96,14 @@
     )
     args = parser.parse_args()
 
     with contextlib.ExitStack() as stack:
         if args.inject_junk:
             stack.enter_context(inject_junk_files(args.source_dir))
 
-    raise SystemExit(compare(args.source_dir, not args.no_isolation, args.verbose))
+    raise SystemExit(
+        compare(args.source_dir, isolated=not args.no_isolation, verbose=args.verbose)
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `check_sdist-0.1.0/src/check_sdist/git.py` & `check_sdist-0.1.1/src/check_sdist/git.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/src/check_sdist/inject.py` & `check_sdist-0.1.1/src/check_sdist/inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/src/check_sdist/sdist.py` & `check_sdist-0.1.1/src/check_sdist/sdist.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,12 +19,14 @@
         (outpath,) = Path(outdir).glob("*.tar.gz")
 
         with tarfile.open(outpath) as tar:
             prefixes = {n.split("/", maxsplit=1)[0] for n in tar.getnames()}
             if len(prefixes) != 1:
                 msg = f"malformted SDist, contains multiple packages {prefixes}"
                 raise AssertionError(msg)
-            return frozenset(n.split("/", maxsplit=1)[1] for n in tar.getnames())
+            return frozenset(
+                t.name.split("/", maxsplit=1)[1] for t in tar.getmembers() if t.isfile()
+            )
 
 
 if __name__ == "__main__":
     print(*sorted(sdist_files(Path.cwd(), True)), sep="\n")
```

### Comparing `check_sdist-0.1.0/tests/test_inject.py` & `check_sdist-0.1.1/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/tests/test_package.py` & `check_sdist-0.1.1/tests/test_package.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 def get_all_files(path: Path) -> frozenset[str]:
     with os.scandir(path) as it:
         return frozenset(it.name for it in it if not it.name.startswith(".coverage"))
 
 
 def test_self_dir():
     start = get_all_files(DIR.parent)
-    assert compare(DIR.parent, True) == 0
+    assert compare(DIR.parent, isolated=True) == 0
     end = get_all_files(DIR.parent)
     assert start == end
 
 
 def test_self_dir_injected():
     start = get_all_files(DIR.parent)
     with inject_junk_files(DIR.parent):
-        assert compare(DIR.parent, True) == 0
+        assert compare(DIR.parent, isolated=True) == 0
     end = get_all_files(DIR.parent)
     assert start == end
```

### Comparing `check_sdist-0.1.0/.gitignore` & `check_sdist-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/LICENSE` & `check_sdist-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.0/pyproject.toml` & `check_sdist-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -67,21 +67,28 @@
 log_cli_level = "INFO"
 testpaths = [
   "tests",
 ]
 
 
 [tool.mypy]
-files = "src"
+files = ["src", "tests"]
 python_version = "3.8"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
+disallow_untyped_defs = false
+disallow_incomplete_defs = false
+
+[[tool.mypy.overrides]]
+module = "check_sdist.*"
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
   "B",           # flake8-bugbear
   "I",           # isort
```

### Comparing `check_sdist-0.1.0/PKG-INFO` & `check_sdist-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-sdist
-Version: 0.1.0
+Version: 0.1.1
 Summary: Check the contents of an SDist vs. git
 Project-URL: Homepage, https://github.com/henryiii/check-sdist
 Project-URL: Bug Tracker, https://github.com/henryiii/check-sdist/issues
 Project-URL: Changelog, https://github.com/henryiii/check-sdist/releases
 Author-email: Henry Schreiner <henryschreineriii@gmail.com>
 License-File: LICENSE
 Keywords: lint,packaging,sdist
@@ -44,56 +44,86 @@
 [actions-link]:             https://github.com/henryiii/check-sdist/actions
 [pypi-link]:                https://pypi.org/project/check-sdist/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/check-sdist
 [pypi-version]:             https://img.shields.io/pypi/v/check-sdist
 
 <!-- prettier-ignore-end -->
 
+Have you ever shipped broken SDists with missing files or possibly dirty SDists
+with files that shouldn't have been there? Have you noticed that standards
+compliant tools aren't making the same SDist that `flit build` is? Is hatchling
+adding `.DSStore` files when you ship from your macOS? No matter what
+build-backend you use, check-sdist can help!
+
+Check-sdist builds an SDist and compares the contents with your Git repository
+contents. It can even temporarily inject common junk files (like pycache files
+or OS specific files) and help verify that those aren't getting bundled into
+your SDist. If you are getting files you didn't expect or missing files you did
+expect, consult your build backend's docs to see how to include or exclude
+files.
+
+### Quick start
+
 To run:
 
 ```console
 $ pipx run check-sdist
 ```
 
 You can add `--no-isolation` to disable build isolation (faster, but must
-preinstall build deps), `--source-dir` to select a different source dir to
-check, and `--inject-junk` to temporarily inject some common junk files while
-running.
+preinstall build dependencies), `--source-dir` to select a different source
+directory to check, and `--inject-junk` to temporarily inject some common junk
+files while running.
 
-To use the development version:
+If you need the latest development version:
 
 ```console
 $ pipx run --spec git+https://github.com/henryiii/check-sdist check-sdist
 ```
 
-To use the pre-commit integration, use this in your `.pre-commit-config.yaml`:
+### Pre-commit integration
+
+To use the [pre-commit](https://pre-commit.com) integration, put this in your
+`.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/henryiii/check-sdist
   rev: v0.1.0
   hooks:
     - id: check-sdist
       args: [--inject-junk]
       additional_dependencies: [] # list your build deps here
 ```
 
-Or, slower, but doesn't require build dependency listing:
+This requires your build dependencies, but in doing so, it can cache the
+environment, making it quite fast. If you don't mind slower runs and don't want
+to require build dependency listing:
 
 ```yaml
 - repo: https://github.com/henryiii/check-sdist
   rev: v0.1.0
   hooks:
     - id: check-sdist-isolated
       args: [--inject-junk]
 ```
 
-To configure, these options are provided for your pyproject.toml file:
+### Configuration
+
+To configure, these options are supported in your `pyproject.toml` file:
 
 ```toml
 [tool.check-sdist]
 sdist-only = []
 git-only = []
 default-ignore = true
 ```
 
-You can add .gitignore style lines here, and you can turn off the default ignore
-list, which adds some default `git-only` files.
+You can add `.gitignore` style lines here, and you can turn off the default
+ignore list, which adds some default git-only files.
+
+### See also
+
+- [check-manifest](https://github.com/mgedmin/check-manifest): A (currently)
+  setuptools specific checker that can suggest possible ways to include/exclude
+  files.
+- [scikit-hep developer pages](https://scikit-hep.org/developer): Guidelines on
+  which this package was designed.
```

