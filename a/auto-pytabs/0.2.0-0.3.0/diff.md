# Comparing `tmp/auto_pytabs-0.2.0.tar.gz` & `tmp/auto_pytabs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_pytabs-0.2.0.tar", max compression
+gzip compressed data, was "auto_pytabs-0.3.0.tar", max compression
```

## Comparing `auto_pytabs-0.2.0.tar` & `auto_pytabs-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-01-29 14:02:18.611305 auto_pytabs-0.2.0/LICENSE
--rw-r--r--   0        0        0    12100 2023-01-29 14:02:18.611305 auto_pytabs-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-01-29 14:02:18.611305 auto_pytabs-0.2.0/auto_pytabs/__init__.py
--rw-r--r--   0        0        0     5344 2023-01-29 14:02:18.611305 auto_pytabs-0.2.0/auto_pytabs/core.py
--rw-r--r--   0        0        0     6358 2023-01-29 14:02:18.611305 auto_pytabs-0.2.0/auto_pytabs/markdown_ext.py
--rw-r--r--   0        0        0     1530 2023-01-29 14:02:18.611305 auto_pytabs-0.2.0/auto_pytabs/mkdocs_plugin.py
--rw-r--r--   0        0        0     6066 2023-01-29 14:02:18.611305 auto_pytabs-0.2.0/auto_pytabs/sphinx_ext.py
--rw-r--r--   0        0        0     1449 2023-01-29 14:02:18.615305 auto_pytabs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    13671 1970-01-01 00:00:00.000000 auto_pytabs-0.2.0/setup.py
--rw-r--r--   0        0        0    13025 1970-01-01 00:00:00.000000 auto_pytabs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/LICENSE
+-rw-r--r--   0        0        0    12172 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/__init__.py
+-rw-r--r--   0        0        0     5391 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/core.py
+-rw-r--r--   0        0        0     6364 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/markdown_ext.py
+-rw-r--r--   0        0        0     1556 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/mkdocs_plugin.py
+-rw-r--r--   0        0        0     6915 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/auto_pytabs/sphinx_ext.py
+-rw-r--r--   0        0        0     2089 2023-04-12 11:02:22.166577 auto_pytabs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 auto_pytabs-0.3.0/PKG-INFO
```

### Comparing `auto_pytabs-0.2.0/LICENSE` & `auto_pytabs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_pytabs-0.2.0/README.md` & `auto_pytabs-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 
 1. Maintaining multiple versions of a single example is tedious and error-prone as they can easily
    become out of sync
 2. Figuring out which examples need to be changed for which specific Python version is a labour intensive task
 3. Dropping or adding support for Python versions requires revisiting every example in the documentation
 4. Checking potentially ~4 versions of a single example into VCS creates unnecessary noise
 
-Given those, it's no surprise that the current standard is to only show examples for the lowest  supported version of Python.
+Given those, it's no surprise that the current standard is to only show examples for the lowest supported version of Python.
 
 ### The solution
 
-**AutoPyTabs** aims to solve all of these problems by automatically generating versions of code examples, targeting different
-Python versions **at build-time**, based on a base version (the lowest supported Python version).
+**AutoPyTabs** aims to solve all of these problems by automatically generating versions (using the awsome
+[ruff](https://github.com/charliermarsh/ruff) project) of code examples, targeting different Python versions
+**at build-time**, based on a base version (the lowest supported Python version).
 This means that:
 
 1. There exists only one version of each example: The lowest supported version becomes the source of truth,
    therefore preventing out-of-sync examples and reducing maintenance burden
 2. Dropping or adding support for Python versions can be done via a simple change in a configuration file
 
 <hr>
```

### Comparing `auto_pytabs-0.2.0/auto_pytabs/core.py` & `auto_pytabs-0.3.0/auto_pytabs/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 from __future__ import annotations
 
 import shutil
+import subprocess
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from hashlib import sha1
 from pathlib import Path
-from typing import Any, Dict, List, NamedTuple, Optional, Set
+from typing import Any, Dict, NamedTuple
 
-import autoflake  # type: ignore
-from pyupgrade._data import Settings as PyUpgradeSettings  # type: ignore
-from pyupgrade._main import _fix_plugins  # type: ignore
+RUFF_BASE_ARGS = [
+    "ruff",
+    "--no-cache",
+    "--fix",
+    "--quiet",
+    "--select",
+    "UP",
+    "--select",
+    "F401",
+    "--isolated",
+    "-",
+    "--target-version",
+]
 
 
 class VersionTuple(NamedTuple):
     major: int
     minor: int
 
     @classmethod
@@ -21,26 +32,25 @@
         return VersionTuple(major=int(major), minor=int(minor))
 
 
 VersionedCode = Dict[VersionTuple, str]
 
 
 class Cache:
-    """
-    Simple hybrid file system / memory cache.
+    """Simple hybrid file system / memory cache.
 
     Follows the
     `Cache Directory Tagging Specification http://www.brynosaurus.com/cachedir/>`_.
     """
 
     def __init__(self) -> None:
         self.cache_dir = Path(".auto_pytabs_cache")
         self.cache_content_dir = self.cache_dir / "content"
-        self._cache: Dict[str, str] = {}
-        self._touched: Set[str] = set()
+        self._cache: dict[str, str] = {}
+        self._touched: set[str] = set()
         self._load()
 
     def _init_cache_dir(self) -> None:
         self.cache_content_dir.mkdir(exist_ok=True, parents=True)
         cachedir_tag = self.cache_dir / "CACHEDIR.TAG"
         gitignore_file = self.cache_dir / ".gitignore"
         if not cachedir_tag.exists():
@@ -52,111 +62,113 @@
             )
         if not gitignore_file.exists():
             gitignore_file.write_text("*\n")
 
     def _load(self) -> None:
         self._init_cache_dir()
 
-        cache: Dict[str, str] = {}
+        cache: dict[str, str] = {}
         with ThreadPoolExecutor() as executor:
             futures = {
                 executor.submit(file.read_text): file.name
                 for file in self.cache_content_dir.iterdir()
             }
             for future in as_completed(futures):
                 cache[futures[future]] = future.result()
         self._cache.update(cache)
 
     @staticmethod
     def make_cache_key(*parts: Any) -> str:
-        """Create a cache key using an md5 hash of ``parts``"""
+        """Create a cache key using an md5 hash of ``parts``."""
         return sha1("".join(map(str, parts)).encode()).hexdigest()
 
-    def get(self, key: str) -> Optional[str]:
-        """Get an item specified by ``key`` the cache"""
+    def get(self, key: str) -> str | None:
+        """Get an item specified by ``key`` the cache."""
         self._touched.add(key)
         return self._cache.get(key)
 
     def set(self, key: str, content: str) -> None:
-        """Store an ``content``"""
+        """Store an ``content``."""
         self._cache[key] = content
         self._touched.add(key)
 
     def persist(self, evict: bool = True) -> None:
         """
-        Persist internal cache to disk. If ``evict`` is ``True``, evict unused items
+        Persist internal cache to disk. If ``evict`` is ``True``, evict unused items.
         """
         with ThreadPoolExecutor() as executor:
             for key, content in self._cache.items():
                 if key in self._touched:
                     executor.submit(
                         self.cache_content_dir.joinpath(key).write_text, content
                     )
                 elif evict:
                     executor.submit(
                         self.cache_content_dir.joinpath(key).unlink, missing_ok=True
                     )
 
     def clear_all(self) -> None:
-        """Clear all cached items from memory and disk"""
+        """Clear all cached items from memory and disk."""
         self._cache = {}
         self._touched = set()
 
         if not self.cache_dir.exists():
             return
 
         shutil.rmtree(self.cache_dir)
 
 
 def get_version_requirements(
     min_version: VersionTuple, max_version: VersionTuple
-) -> List[VersionTuple]:
-    """Given a min and max version, generate all versions in between"""
+) -> list[VersionTuple]:
+    """Given a min and max version, generate all versions in between."""
     min_major, min_minor = min_version
     max_major, max_minor = max_version
     return [
         VersionTuple(major=major, minor=minor)
         for major in range(min_major, max_major + 1)
         for minor in range(min_minor, max_minor + 1)
     ]
 
 
+def _run_ruff(source: str, target_version: str) -> str:
+    with subprocess.Popen(
+        [*RUFF_BASE_ARGS, target_version],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        stdin=subprocess.PIPE,
+        encoding="utf-8",
+    ) as process:
+        return process.communicate(input=source)[0]
+
+
 def _upgrade_code(
-    code: str, min_version: VersionTuple, cache: Optional[Cache] = None
+    code: str, min_version: VersionTuple, cache: Cache | None = None
 ) -> str:
-    cache_key: Optional[str] = None
+    cache_key: str | None = None
     if cache:
         cache_key = cache.make_cache_key(code, min_version)
 
         if cached_code := cache.get(cache_key):
             return cached_code
 
-    upgraded_code = _fix_plugins(
-        code,
-        settings=PyUpgradeSettings(
-            min_version=min_version,
-            keep_percent_format=True,
-            keep_mock=True,
-            keep_runtime_typing=True,
-        ),
-    )
-    if upgraded_code != code:
-        code = autoflake.fix_code(upgraded_code, remove_all_unused_imports=True)
+    code = _run_ruff(code, target_version=f"py3{min_version.minor}")
 
     if cache_key and cache:
         cache.set(cache_key, code)
 
     return code
 
 
 def version_code(
-    code: str, version_requirements: List[VersionTuple], cache: Optional[Cache] = None
+    code: str, version_requirements: list[VersionTuple], cache: Cache | None = None
 ) -> VersionedCode:
     """Create versions of ``code`` for all python versions specified in
-    ``version_requirements`` and return a dictionary of version-tuples/code"""
+    ``version_requirements`` and return a dictionary of version-tuples/code.
+    """
     latest_code = code
     versioned_code: VersionedCode = {version_requirements[0]: code}
 
     for version in version_requirements:
         upgraded_code = _upgrade_code(latest_code, version, cache=cache)
         if upgraded_code != latest_code:
             versioned_code[version] = upgraded_code
```

### Comparing `auto_pytabs-0.2.0/auto_pytabs/markdown_ext.py` & `auto_pytabs-0.3.0/auto_pytabs/markdown_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 
 import re
-from typing import Any, Dict, List, Literal, Optional, Set, Tuple, cast
+from typing import TYPE_CHECKING, Any, Literal, cast
 
-import markdown
 from markdown import Extension
 from markdown.preprocessors import Preprocessor
 
 from auto_pytabs.core import (
     Cache,
-    VersionTuple,
     VersionedCode,
+    VersionTuple,
     get_version_requirements,
     version_code,
 )
 
+if TYPE_CHECKING:
+    from markdown import Markdown
+
+
 RGX_BLOCK_TOKENS = re.compile(r"(.*```py[\w\W]*)|(.*```)")
 RGX_PYTABS_DIRECTIVE = re.compile(r"<!-- ?autopytabs: ?(.*)-->")
 
 PyTabDirective = Literal["disable", "enable", "disable-block"]
-PYTAB_DIRECTIVES: Set[PyTabDirective] = {"disable", "enable", "disable-block"}
+PYTAB_DIRECTIVES: set[PyTabDirective] = {"disable", "enable", "disable-block"}
 
 
-def _strip_indentation(lines: List[str]) -> Tuple[List[str], str]:
+def _strip_indentation(lines: list[str]) -> tuple[list[str], str]:
     if not lines:
         return [], ""
     first_line = lines[0]
     indent_char = ""
     if first_line[0] in [" ", "\t"]:
         indent_char = first_line[0]
     indent = indent_char * (len(first_line) - len(first_line.lstrip(indent_char)))
@@ -45,18 +48,18 @@
         matched_directive = match.group(1).strip()
         if matched_directive in PYTAB_DIRECTIVES:
             return cast(PyTabDirective, matched_directive)
         raise RuntimeError(f"Invalid AutoPytabs directive: {matched_directive!r}")
     return None
 
 
-def _extract_code_blocks(lines: List[str]) -> Tuple[List[str], Dict[int, List[str]]]:
+def _extract_code_blocks(lines: list[str]) -> tuple[list[str], dict[int, list[str]]]:
     in_block = False
     enabled = True
-    new_lines: List[str] = []
+    new_lines: list[str] = []
 
     to_transform = {}
 
     start = 0
     for i, line in enumerate(lines):
         is_comment_line = False
         directive = _get_pytabs_directive(line)
@@ -100,16 +103,16 @@
         tab_title = tab_title_template.format(min_version=version_string)
         out.append(f'=== "{tab_title}"\n{code}\n')
     return "\n".join(out)
 
 
 def _convert_block(
     *,
-    block: List[str],
-    versions: List[VersionTuple],
+    block: list[str],
+    versions: list[VersionTuple],
     tab_title_template: str,
     cache: Cache | None,
 ) -> str:
     block, indentation = _strip_indentation(block)
     head, *code_lines, tail = block
     code = "\n".join(code_lines)
     versioned_code = version_code(code, versions, cache=cache)
@@ -142,15 +145,15 @@
         self.min_version = VersionTuple.from_string(min_version)
         self.max_version = VersionTuple.from_string(max_version)
         self.versions = get_version_requirements(self.min_version, self.max_version)
         self.tab_title_template = tab_title_template or "Python {min_version}+"
         self.cache = cache
         super().__init__(*args, **kwargs)
 
-    def run(self, lines: List[str]) -> List[str]:
+    def run(self, lines: list[str]) -> list[str]:
         new_lines, to_transform = _extract_code_blocks(lines)
 
         output_lines = []
         for i, line in enumerate(new_lines):
             block_to_transform = to_transform.get(i)
             if block_to_transform:
                 transformed_block = _convert_block(
@@ -163,26 +166,25 @@
             else:
                 output_lines.append(line)
 
         return output_lines
 
 
 class AutoPyTabsExtension(Extension):
-    def __init__(self, *args: Any, cache: Optional[Cache], **kwargs: Any):
+    def __init__(self, *args: Any, cache: Cache | None, **kwargs: Any):
         self.config = {
             "min_version": ["3.7", "minimum version"],
             "max_version": ["3.11", "maximum version"],
             "tab_title_template": ["", "tab title format-string"],
         }
         self.cache = cache
         super().__init__(*args, **kwargs)
 
-    def extendMarkdown(self, md: markdown.Markdown) -> None:
+    def extendMarkdown(self, md: Markdown) -> None:
         """Register the extension."""
-
         self.md = md
         md.registerExtension(self)
         config = self.getConfigs()
 
         md.preprocessors.register(
             UpgradePreprocessor(
                 min_version=config["min_version"],
```

### Comparing `auto_pytabs-0.2.0/auto_pytabs/mkdocs_plugin.py` & `auto_pytabs-0.3.0/auto_pytabs/mkdocs_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from mkdocs.config.defaults import MkDocsConfig
+
 
 from mkdocs.config import Config, config_options
-from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 
 from auto_pytabs.core import Cache
 
 
 class PluginConfig(Config):  # type: ignore[no-untyped-call]
     min_version = config_options.Type(str, default="3.7")
     max_version = config_options.Type(str, default="3.11")
     tab_title_template = config_options.Type(str, default="Python {min_version}+")
     no_cache = config_options.Type(bool, default=False)
 
 
 class AutoPyTabsPlugin(BasePlugin[PluginConfig]):  # type: ignore[no-untyped-call]
     def __init__(self) -> None:
-        self.cache: Optional[Cache] = None
+        self.cache: Cache | None = None
 
     def on_config(self, config: MkDocsConfig) -> Config | None:
         if not self.config.no_cache:
             self.cache = Cache()
 
         config.markdown_extensions.append("auto_pytabs")
         config["mdx_configs"].update(
```

### Comparing `auto_pytabs-0.2.0/auto_pytabs/sphinx_ext.py` & `auto_pytabs-0.3.0/auto_pytabs/sphinx_ext.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Iterable, List, TYPE_CHECKING, cast
+import importlib
+import importlib.metadata
+from collections.abc import Iterable
+from typing import TYPE_CHECKING, Any, cast
 
 from docutils.nodes import Node, container, section
 from docutils.parsers.rst import directives
 from docutils.statemachine import ViewList
-from sphinx.config import Config
 from sphinx.directives.code import CodeBlock, LiteralInclude
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.nodes import nested_parse_with_titles
 
 from auto_pytabs.core import (
     Cache,
     VersionedCode,
     get_version_requirements,
     version_code,
 )
 
 if TYPE_CHECKING:
     from sphinx.application import Sphinx
+    from sphinx.config import Config
+    from sphinx.environment import BuildEnvironment
 
 
-def indent(string: str, indent_char: str = " ", level: int = 4) -> List[str]:
+def indent(string: str, indent_char: str = " ", level: int = 4) -> list[str]:
     return list((indent_char * level) + line for line in string.splitlines())
 
 
 class UpgradeMixin(SphinxDirective):
     compat: bool = False
 
     def _render_directive_options(self) -> str:
         ret = ""
-        options: Dict[str, Any] = {
+        options: dict[str, Any] = {
             k: v for k, v in self.options.items() if k in CodeBlock.option_spec
         }
         if not self.compat:
             options["no-upgrade"] = True
         for option, value in options.items():
             if self.option_spec[option] is directives.flag:
                 value = None
@@ -43,15 +47,15 @@
             ret += f":{option}: {value if value is not None else ''}\n"
         return ret
 
     def _create_tabs(
         self,
         versioned_code: VersionedCode,
         tab_title_template: str,
-    ) -> List[str]:
+    ) -> list[str]:
         if len(versioned_code) == 1:
             return [
                 ".. code-block:: python",
                 *indent(self._render_directive_options()),
                 "",
                 *indent(versioned_code.popitem()[1]),
                 "",
@@ -70,19 +74,21 @@
                     "",
                     *indent(code, level=12),
                     "",
                 ]
             )
         return out
 
-    def _create_py_tab_nodes(self, code: str) -> List[Node]:
+    @property
+    def cache(self) -> Cache | None:
+        return getattr(self.env, "auto_pytabs_cache", None)
+
+    def _create_py_tab_nodes(self, code: str) -> list[Node]:
         version_requirements = self.config["auto_pytabs_versions"]
-        versioned_code = version_code(
-            code, version_requirements, cache=self.config["auto_pytabs_cache"]
-        )
+        versioned_code = version_code(code, version_requirements, cache=self.cache)
         tabs = self._create_tabs(
             versioned_code, self.env.config["auto_pytabs_tab_title_template"]
         )
 
         rst = ViewList()
         source, lineno = self.get_source_info()
         for line in tabs:
@@ -90,15 +96,15 @@
 
         node = section()
         node.document = self.state.document
 
         nested_parse_with_titles(self.state, rst, node)
         nodes = node.children
 
-        return cast(List[Node], nodes)
+        return cast("list[Node]", nodes)
 
 
 class PyTabsCodeBlock(CodeBlock, UpgradeMixin):
     compat = True
 
     def run(self) -> list[Node]:
         if not self.arguments or self.arguments[0] != "python":
@@ -107,78 +113,93 @@
         self.assert_has_content()
         return self._create_py_tab_nodes("\n".join(self.content))
 
 
 class PyTabsLiteralInclude(LiteralInclude, UpgradeMixin):
     compat = True
 
-    def run(self) -> List[Node]:
+    def run(self) -> list[Node]:
         base_node = super().run()[0]
         if self.options.get("language") != "python":
             return [base_node]
         if isinstance(base_node, container):
             base_node = base_node.children[1]
         return self._create_py_tab_nodes(base_node.rawsource)  # type: ignore[attr-defined]  # noqa: E501
 
 
 class CodeBlockOverride(PyTabsCodeBlock):
     compat = False
     option_spec = {**CodeBlock.option_spec, "no-upgrade": directives.flag}
 
-    def run(self) -> List[Node]:
+    def run(self) -> list[Node]:
         if "no-upgrade" in self.options:
             return CodeBlock.run(self)
 
         return super().run()
 
 
 class LiteralIncludeOverride(PyTabsLiteralInclude):
     compat = False
     option_spec = {**LiteralInclude.option_spec, "no-upgrade": directives.flag}
 
-    def run(self) -> List[Node]:
+    def run(self) -> list[Node]:
         if "no-upgrade" in self.options:
             return LiteralInclude.run(self)
         return super().run()
 
 
 def on_config_inited(app: Sphinx, config: Config) -> None:
     config["auto_pytabs_versions"] = get_version_requirements(
         config["auto_pytabs_min_version"], config["auto_pytabs_max_version"]
     )
-    app.config["auto_pytabs_cache"] = (
-        Cache() if not config["auto_pytabs_no_cache"] else None
-    )
 
     if not config["auto_pytabs_compat_mode"]:
         app.add_directive("code-block", CodeBlockOverride, override=True)
         app.add_directive("literalinclude", LiteralIncludeOverride, override=True)
 
 
 def on_build_finished(app: Sphinx, exception: Exception | None) -> None:
-    if cache := app.config["auto_pytabs_cache"]:
+    if cache := getattr(app.env, "auto_pytabs_cache", None):
         cache.persist()
 
 
-def setup(app: Sphinx) -> Dict[str, bool | str]:
+def on_env_before_read_docs(
+    app: Sphinx, env: BuildEnvironment, docnames: list[str]
+) -> None:
+    if not app.config["auto_pytabs_no_cache"]:
+        env.auto_pytabs_cache = Cache()  # type: ignore[attr-defined]
+
+
+def on_env_merge_info(
+    app: Sphinx, env: BuildEnvironment, docnames: list[str], other: BuildEnvironment
+) -> None:
+    cache: Cache | None = getattr(env, "auto_pytabs_cache", None)
+    other_cache: Cache | None = getattr(other, "auto_pytabs_cache", None)
+    if cache and other_cache:
+        cache._touched.update(other_cache._touched)
+        cache._cache.update(other_cache._cache)
+
+
+def setup(app: Sphinx) -> dict[str, bool | str]:
     app.add_directive("pytabs-code-block", PyTabsCodeBlock)
     app.add_directive("pytabs-literalinclude", PyTabsLiteralInclude)
 
     app.add_config_value(
         "auto_pytabs_tab_title_template",
         default="Python {min_version}+",
         rebuild="html",
     )
     app.add_config_value("auto_pytabs_min_version", default=(3, 7), rebuild="html")
     app.add_config_value("auto_pytabs_max_version", default=(3, 11), rebuild="html")
     app.add_config_value("auto_pytabs_no_cache", default=False, rebuild="html")
     app.add_config_value("auto_pytabs_compat_mode", default=False, rebuild="html")
 
     app.connect("config-inited", on_config_inited)
-
     app.connect("build-finished", on_build_finished)
+    app.connect("env-before-read-docs", on_env_before_read_docs)
+    app.connect("env-merge-info", on_env_merge_info)
 
     return {
-        "version": "0.1",
+        "version": importlib.metadata.version("auto_pytabs"),
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `auto_pytabs-0.2.0/pyproject.toml` & `auto_pytabs-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "auto-pytabs"
-version = "0.2.0"
+version = "0.3.0"
 description = "Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations"
 authors = ["Janek Nouvertné <provinzkraut@posteo.de>"]
 readme = "README.md"
 packages = [{ include = "auto_pytabs" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pyupgrade = "^3.3.1"
-autoflake = "^2.0.0"
-sphinx = { version = ">=4,<6", optional = true }
-markdown = {version = ">=3.2.1,<3.4", optional = true }
+sphinx = { version = ">=4", optional = true }
+markdown = {version = ">=3.2.1", optional = true }
 mkdocs = {version = "^1.4.2", optional = true}
-pytest-mock = "^3.10.0"
+ruff = "^0.0.260"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 mypy = "^0.990"
 types-markdown = "^3.4.2.1"
 pytest = "^7.2.0"
 pymdown-extensions = "^9.9"
 sphinx-design = "^0.3.0"
 pytest-regressions = "^2.4.2"
 types-docutils = "^0.19.1.1"
 mkdocs = "^1.4.2"
 pyyaml = "^6.0"
+pytest-mock = "^3.10.0"
+pre-commit = "^3.2.1"
 
 
 [tool.poetry.extras]
 sphinx = ["sphinx"]
 markdown = ["markdown"]
 mkdocs = ["mkdocs"]
 
@@ -52,7 +52,38 @@
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning:sphinx_design.*:",
     "ignore::DeprecationWarning:sphinx.util.images:4",
     "ignore::DeprecationWarning:importlib.resources._legacy:80",
 ]
+
+
+[tool.ruff]
+select = [
+    "DTZ", # flake8-datetimez
+    "E", # pycodestyle errors
+    "ERA", # eradicate
+    "F", # pyflakes
+    "I", # isort
+    "ICN", # flake8-import-conventions
+    "PLE",
+    "PTH", # flake8-use-pathlib
+    "Q", # flake8-quotes
+    "RET", # flake8-return
+    "RUF", # Ruff-specific rules
+    "SIM", # flake8-simplify
+    "T10", # flake8-debugger
+    "T20", # flake8-print
+    "TCH", # flake8-type-checking
+    "TID", # flake8-tidy-imports
+    "UP", # pyupgrade
+    "W", # pycodestyle - warning
+    "YTT", # flake8-2020
+]
+
+src = ["auto_pytabs", "test"]
+target-version = "py38"
+
+
+[tool.ruff.per-file-ignores]
+"test*" = ["S101"]
```

### Comparing `auto_pytabs-0.2.0/setup.py` & `auto_pytabs-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,405 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: auto-pytabs
+Version: 0.3.0
+Summary: Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations
+Author: Janek Nouvertné
+Author-email: provinzkraut@posteo.de
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: markdown
+Provides-Extra: mkdocs
+Provides-Extra: sphinx
+Requires-Dist: markdown (>=3.2.1) ; extra == "markdown"
+Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "mkdocs"
+Requires-Dist: ruff (>=0.0.260,<0.0.261)
+Requires-Dist: sphinx (>=4) ; extra == "sphinx"
+Description-Content-Type: text/markdown
 
-packages = \
-['auto_pytabs']
+# AutoPyTabs
 
-package_data = \
-{'': ['*']}
+Automatically generate code examples for different Python versions in
+[mkdocs](https://www.mkdocs.org) or [Sphinx](https://www.sphinx-doc.org) based documentations, or a plain
+[markdown](https://python-markdown.github.io/) workflow, making use of the
+[pymdown "tabbed"](https://facelessuser.github.io/pymdown-extensions/extensions/tabbed/) markdown extension for markdown,
+and [sphinx{design} tabs](https://sphinx-design.readthedocs.io/en/latest/tabs.html) for Sphinx.
 
-install_requires = \
-['autoflake>=2.0.0,<3.0.0',
- 'pytest-mock>=3.10.0,<4.0.0',
- 'pyupgrade>=3.3.1,<4.0.0']
-
-extras_require = \
-{'markdown': ['markdown>=3.2.1,<3.4'],
- 'mkdocs': ['mkdocs>=1.4.2,<2.0.0'],
- 'sphinx': ['sphinx>=4,<6']}
-
-entry_points = \
-{'markdown.extensions': ['auto_pytabs = '
-                         'auto_pytabs.markdown_ext:AutoPyTabsExtension'],
- 'mkdocs.plugins': ['auto_pytabs = auto_pytabs.mkdocs_plugin:AutoPyTabsPlugin']}
-
-setup_kwargs = {
-    'name': 'auto-pytabs',
-    'version': '0.2.0',
-    'description': 'Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations',
-    'long_description': '# AutoPyTabs\n\nAutomatically generate code examples for different Python versions in\n[mkdocs](https://www.mkdocs.org) or [Sphinx](https://www.sphinx-doc.org) based documentations, or a plain\n[markdown](https://python-markdown.github.io/) workflow, making use of the\n[pymdown "tabbed"](https://facelessuser.github.io/pymdown-extensions/extensions/tabbed/) markdown extension for markdown,\nand [sphinx{design} tabs](https://sphinx-design.readthedocs.io/en/latest/tabs.html) for Sphinx.\n\n## Rationale\n\n### The problem\n\nPython project documentation typically include code examples. Given that most of the time, a project will support\nmultiple versions of Python, it would be ideal to showcase the adjustments that can or need to be made for different\nPython versions. This can be achieved by including several versions of the example code, conveniently displayed using\nthe [pymdown "tabbed"](https://facelessuser.github.io/pymdown-extensions/extensions/tabbed/) extension for markdown, or\n[sphinx{design} tabs](https://sphinx-design.readthedocs.io/en/latest/tabs.html) for Sphinx.\n\nThis, however, raises several problems:\n\n1. Maintaining multiple versions of a single example is tedious and error-prone as they can easily\n   become out of sync\n2. Figuring out which examples need to be changed for which specific Python version is a labour intensive task\n3. Dropping or adding support for Python versions requires revisiting every example in the documentation\n4. Checking potentially ~4 versions of a single example into VCS creates unnecessary noise\n\nGiven those, it\'s no surprise that the current standard is to only show examples for the lowest  supported version of Python.\n\n### The solution\n\n**AutoPyTabs** aims to solve all of these problems by automatically generating versions of code examples, targeting different\nPython versions **at build-time**, based on a base version (the lowest supported Python version).\nThis means that:\n\n1. There exists only one version of each example: The lowest supported version becomes the source of truth,\n   therefore preventing out-of-sync examples and reducing maintenance burden\n2. Dropping or adding support for Python versions can be done via a simple change in a configuration file\n\n<hr>\n\n## Table of contents\n\n1. [Usage with mkdocs / markdown](#usage-markdown)\n   1. [Configuration](#markdown-config)\n   2. [Differences between the mkdocs plugin vs markdown extension](#differences-between-the-mkdocs-plugin-and-markdown-extension)\n   3. [Examples](#markdown-examples)\n   4. [Selectively disable](#selectively-disable)\n   5. [Compatibility with `pymdownx.snippets`](#compatibility-with-pymdownxsnippets)\n2. [Usage with Sphinx](#usage-with-sphinx)\n   1. [Configuration](#sphinx-config)\n   2. [Directives](#directives)\n   3. [Examples](#sphinx-examples)\n   4. [Compatibility with other extensions](#compatibility-with-other-extensions)\n\n<hr> \n\n## Installation\n\nFor mkdocs: `pip install auto-pytabs[mkdocs]`\nFor markdown: `pip install auto-pytabs[markdown]`\nFor sphinx: `pip install auto-pytabs[sphinx]`\n\n<h2 id="usage-markdown">Usage with mkdocs / markdown</h2>\n\n<h3 id="markdown-config">Configuration</h3>\n\n#### Mkdocs plugin\n\n```yaml\nsite_name: My Docs\nmarkdown_extensions:\n  - pymdownx.tabbed:\nplugins:\n  - auto_pytabs:\n      min_version: "3.7"  # optional\n      max_version: "3.11" # optional\n      tab_title_template: "Python {min_version}+"  # optional\n      no_cache: false  # optional\n```\n\n*Available configuration options*\n\n| Name                 | Default                   | Description                 |\n| -------------------- | ------------------------- | --------------------------- |\n| `min_version`        | `(3, 7)`                  | Minimum python version      |\n| `max_version`        | `(3, 7)`                  | Maximum python version      |\n| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles     |\n| `no_cache`           | `False`                   | Disable file system caching |\n\n#### Markdown extension\n\n```python\nimport markdown\n\nmd = markdown.Markdown(\n    extensions=["auto_pytabs"],\n    extension_configs={\n        "auto_pytabs": {\n            "min_version": "3.7",  # optional\n            "max_version": "3.11",  # optional\n            "tab_title_template": "Python {min_version}+",  # optional\n        }\n    },\n)\n```\n\n*Available configuration options*\n\n| Name                 | Default                   | Description                                 |\n| -------------------- | ------------------------- | ------------------------------------------- |\n| `min_version`        | `(3, 7)`                  | Minimum python version to generate code for |\n| `max_version`        | `(3, 7)`                  | Maximum python version to generate code for |\n| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                     |\n\n### Differences between the mkdocs plugin and markdown extension\n\nAutoPyTabs ships as a markdown extension and an mkdocs plugin, both of which can be used in mkdocs. The only difference\nbetween them is that the mkdocs plugin supports caching, which can make subsequent builds faster (i.e. when using `mkdocs serve`).\nThe reason why the markdown extension does not support caching is that `markdown` does not have clearly defined build\nsteps with wich an extension could interact (like mkdocs [plugin events](https://www.mkdocs.org/dev-guide/plugins/#events)),\nmaking it impossible to know when to persist cached items to disk / evict unused items.\n\n**If you are using mkdocs, the mkdocs plugin is recommended**. If you have caching disabled, there will be no difference either way.\n\nShould you wish to integrate the markdown extension into a build process where you can manually persist the cache after the build,\nyou can explicitly pass it a cache:\n\n```python\nimport markdown\nfrom auto_pytabs.core import Cache\n\ncache = Cache()\n\nmd = markdown.Markdown(\n    extensions=["auto_pytabs"],\n    extension_configs={\n        "auto_pytabs": {\n           "cache": cache\n        }\n    },\n)\n\n\ndef build_markdown() -> None:\n    md.convertFile("document.md", "document.html")\n    cache.persist()\n```\n\n<h3 id="markdown-examples">Examples</h3>\n\n**Input**\n\n<pre>\n```python\nfrom typing import Optional, Dict\n\ndef foo(bar: Optional[str]) -> Dict[str, str]:\n    ...\n```\n</pre>\n\n**Equivalent markdown**\n\n<pre>\n=== "Python 3.7+"\n    ```python\n    from typing import Optional, Dict\n\n    def foo(bar: Optional[str]) -> Dict[str, str]:\n        ...\n    ```\n\n=== "Python 3.9+"\n    ```python\n    from typing import Optional\n    \n    \n    def foo(bar: Optional[str]) -> dict[str, str]:\n        ...\n    ```\n\n==== "Python 3.10+"\n    ```python\n    def foo(bar: str | None) -> dict[str, str]:\n        ...\n    ```\n</pre>\n\n#### Nested blocks\n\nNested tabs are supported as well:\n\n**Input**\n\n<pre>\n=== "Level 1-1"\n\n    === "Level 2-1"\n\n        ```python\n        from typing import List\n        x: List[str]\n        ```\n\n    === "Level 2-2"\n    \n        Hello, world!\n\n=== "Level 1-2"\n\n    Goodbye, world!\n</pre>\n\n**Equivalent markdown**\n\n<pre>\n=== "Level 1-1"\n\n    === "Level 2-1"\n\n        === "Python 3.7+"\n            ```python\n            from typing import List\n            x: List[str]\n            ```\n        \n        === "Python 3.9+"\n            ```python\n            x: list[str]\n            ```\n\n    === "Level 2-2"\n\n        Goodbye, world!\n\n=== "Level 1-2"\n    Hello, world!\n    \n</pre>\n\n### Selectively disable\n\nYou can disable conversion for a single code block:\n\n````\n<!-- autopytabs: disable-block -->\n```python\nfrom typing import Set, Optional\n\ndef bar(baz: Optional[str]) -> Set[str]:\n    ...\n```\n````\n\nOr for whole sections / files\n\n```\n<!-- autopytabs: disable -->\neverything after this will be ignored\n<!-- autopytabs: enable -->\nre-enables conversion again\n```\n\n### Compatibility with `pymdownx.snippets`\n\nIf the `pymdownx.snippets` extension is used, make sure that it runs **before** AutoPyTab\n\n<hr>\n\n## Usage with Sphinx\n\nAutPyTabs provides a Sphinx extension `auto_pytabs.sphinx_ext`, enabling its functionality\nfor the `.. code-block` and `.. literalinclude` directives.\n\n<h3 id="sphinx-config">Configuration</h3>\n\n#### Example configuration\n\n```python\nextensions = ["auto_pytabs.sphinx_ext", "sphinx_design"]\n\nauto_pytabs_min_version = (3, 7)  # optional\nauto_pytabs_max_version = (3, 11)  # optional\nauto_pytabs_tab_title_template = "Python {min_version}+"  # optional \n# auto_pytabs_no_cache = True  # disabled file system caching\n# auto_pytabs_compat_mode = True  # enable compatibility mode\n```\n\n#### Available configuration options\n\n| Name                             | Default                   | Description                                      |\n| -------------------------------- | ------------------------- | ------------------------------------------------ |\n| `auto_pytabs_min_version`        | `(3, 7)`                  | Minimum python version to generate code for      |\n| `auto_pytabs_max_version`        | `(3, 7)`                  | Maximum python version to generate code for      |\n| `auto_pytabs_tab_title_template` | `"Python {min_version}+"` | Template for tab titles                          |\n| `auto_pytabs_no_cache`           | `False`                   | Disable file system caching                      |\n| `auto_pytabs_compat_mode`        | `False`                   | Enable [compatibility mode](#compatibility-mode) |\n\n<h3 id="sphinx-examples">Examples</h3>\n\n**Input**\n\n```rst\n.. code-block:: python\n\n   from typing import Optional, Dict\n   \n   def foo(bar: Optional[str]) -> Dict[str, str]:\n       ...\n```\n\n**Equivalent ReST**\n\n```rst\n.. tab-set::\n\n   .. tab-item:: Python 3.7+\n   \n       .. code-block:: python\n       \n          from typing import Optional, Dict\n      \n          def foo(bar: Optional[str]) -> Dict[str, str]:\n              ...\n\n   .. tab-item:: Python 3.9+\n   \n      .. code-block:: python\n      \n          from typing import Optional\n          \n          \n          def foo(bar: Optional[str]) -> dict[str, str]:\n              ...\n\n   .. tab-item:: Python 3.10+\n   \n      .. code-block:: python\n      \n          def foo(bar: str | None) -> dict[str, str]:\n              ...\n\n```\n\n### Directives\n\nAutoPyTabs overrides the built-in `code-block` and `literal-include` directives,\nextending them with auto-upgrade and tabbing functionality, which means no special\ndirectives, and therefore changes to existing documents are needed.\n\nAdditionally, a `:no-upgrade:` option is added to the directives, which can be used to\nselectively fall back the default behaviour.\n\nTwo new directives are provided as well:\n\n- `.. pytabs-code-block::`\n- `.. pytabs-literalinclude::`\n\nwhich by default act exactly like `.. code-block` and `.. literalinclude` respectively,\nand are mainly to provide AutoPyTab\'s functionality in [compatibility mode](#compatibility-mode).\n\n### Compatibility mode\n\nIf you don\'t want the default behaviour of directive overrides, and instead wish to use the\n`.. pytabs-` directives manually (e.g. because of compatibility issues with other extensions\nor because you only want to apply it to select code blocks) you can make use AutoPyTabs\' compatibility\nmode. To enable it, simply use the `auto_pytabs_compat_mode = True` in `conf.py`. Now, only content within `.. pytabs-`\ndirectives will be upgraded.\n\n### Compatibility with other extensions\n\nNormally the directive overrides don\'t cause any problems and are very convenient,\nsince no changes to existing documents have to be made. However, if other extensions are included,\nwhich themselves override one of those directives, one of them will inadvertently override the other,\ndepending on the order they\'re defined in `extensions`.\n\nTo combat this, you can use the [compatibility mode](#compatibility-mode) extension instead, which\nonly includes the new directives.\n\nIf you control the conflicting overrides, you can alternatively inherit from\n`auto_py_tabs.sphinx_ext.CodeBlockOverride` and `auto_py_tabs.sphinx_ext.LiteralIncludeOverride`\ninstead of `sphinx.directives.code.CodeBlock` and `sphinx.directives.code.LiteralInclude` respectively.\n',
-    'author': 'Janek Nouvertné',
-    'author_email': 'provinzkraut@posteo.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Rationale
 
+### The problem
+
+Python project documentation typically include code examples. Given that most of the time, a project will support
+multiple versions of Python, it would be ideal to showcase the adjustments that can or need to be made for different
+Python versions. This can be achieved by including several versions of the example code, conveniently displayed using
+the [pymdown "tabbed"](https://facelessuser.github.io/pymdown-extensions/extensions/tabbed/) extension for markdown, or
+[sphinx{design} tabs](https://sphinx-design.readthedocs.io/en/latest/tabs.html) for Sphinx.
+
+This, however, raises several problems:
+
+1. Maintaining multiple versions of a single example is tedious and error-prone as they can easily
+   become out of sync
+2. Figuring out which examples need to be changed for which specific Python version is a labour intensive task
+3. Dropping or adding support for Python versions requires revisiting every example in the documentation
+4. Checking potentially ~4 versions of a single example into VCS creates unnecessary noise
+
+Given those, it's no surprise that the current standard is to only show examples for the lowest supported version of Python.
+
+### The solution
+
+**AutoPyTabs** aims to solve all of these problems by automatically generating versions (using the awsome
+[ruff](https://github.com/charliermarsh/ruff) project) of code examples, targeting different Python versions
+**at build-time**, based on a base version (the lowest supported Python version).
+This means that:
+
+1. There exists only one version of each example: The lowest supported version becomes the source of truth,
+   therefore preventing out-of-sync examples and reducing maintenance burden
+2. Dropping or adding support for Python versions can be done via a simple change in a configuration file
+
+<hr>
+
+## Table of contents
+
+1. [Usage with mkdocs / markdown](#usage-markdown)
+   1. [Configuration](#markdown-config)
+   2. [Differences between the mkdocs plugin vs markdown extension](#differences-between-the-mkdocs-plugin-and-markdown-extension)
+   3. [Examples](#markdown-examples)
+   4. [Selectively disable](#selectively-disable)
+   5. [Compatibility with `pymdownx.snippets`](#compatibility-with-pymdownxsnippets)
+2. [Usage with Sphinx](#usage-with-sphinx)
+   1. [Configuration](#sphinx-config)
+   2. [Directives](#directives)
+   3. [Examples](#sphinx-examples)
+   4. [Compatibility with other extensions](#compatibility-with-other-extensions)
+
+<hr> 
+
+## Installation
+
+For mkdocs: `pip install auto-pytabs[mkdocs]`
+For markdown: `pip install auto-pytabs[markdown]`
+For sphinx: `pip install auto-pytabs[sphinx]`
+
+<h2 id="usage-markdown">Usage with mkdocs / markdown</h2>
+
+<h3 id="markdown-config">Configuration</h3>
+
+#### Mkdocs plugin
+
+```yaml
+site_name: My Docs
+markdown_extensions:
+  - pymdownx.tabbed:
+plugins:
+  - auto_pytabs:
+      min_version: "3.7"  # optional
+      max_version: "3.11" # optional
+      tab_title_template: "Python {min_version}+"  # optional
+      no_cache: false  # optional
+```
+
+*Available configuration options*
+
+| Name                 | Default                   | Description                 |
+| -------------------- | ------------------------- | --------------------------- |
+| `min_version`        | `(3, 7)`                  | Minimum python version      |
+| `max_version`        | `(3, 7)`                  | Maximum python version      |
+| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles     |
+| `no_cache`           | `False`                   | Disable file system caching |
+
+#### Markdown extension
+
+```python
+import markdown
+
+md = markdown.Markdown(
+    extensions=["auto_pytabs"],
+    extension_configs={
+        "auto_pytabs": {
+            "min_version": "3.7",  # optional
+            "max_version": "3.11",  # optional
+            "tab_title_template": "Python {min_version}+",  # optional
+        }
+    },
+)
+```
+
+*Available configuration options*
+
+| Name                 | Default                   | Description                                 |
+| -------------------- | ------------------------- | ------------------------------------------- |
+| `min_version`        | `(3, 7)`                  | Minimum python version to generate code for |
+| `max_version`        | `(3, 7)`                  | Maximum python version to generate code for |
+| `tab_title_template` | `"Python {min_version}+"` | Template for tab titles                     |
+
+### Differences between the mkdocs plugin and markdown extension
+
+AutoPyTabs ships as a markdown extension and an mkdocs plugin, both of which can be used in mkdocs. The only difference
+between them is that the mkdocs plugin supports caching, which can make subsequent builds faster (i.e. when using `mkdocs serve`).
+The reason why the markdown extension does not support caching is that `markdown` does not have clearly defined build
+steps with wich an extension could interact (like mkdocs [plugin events](https://www.mkdocs.org/dev-guide/plugins/#events)),
+making it impossible to know when to persist cached items to disk / evict unused items.
+
+**If you are using mkdocs, the mkdocs plugin is recommended**. If you have caching disabled, there will be no difference either way.
+
+Should you wish to integrate the markdown extension into a build process where you can manually persist the cache after the build,
+you can explicitly pass it a cache:
+
+```python
+import markdown
+from auto_pytabs.core import Cache
+
+cache = Cache()
+
+md = markdown.Markdown(
+    extensions=["auto_pytabs"],
+    extension_configs={
+        "auto_pytabs": {
+           "cache": cache
+        }
+    },
+)
+
+
+def build_markdown() -> None:
+    md.convertFile("document.md", "document.html")
+    cache.persist()
+```
+
+<h3 id="markdown-examples">Examples</h3>
+
+**Input**
+
+<pre>
+```python
+from typing import Optional, Dict
+
+def foo(bar: Optional[str]) -> Dict[str, str]:
+    ...
+```
+</pre>
+
+**Equivalent markdown**
+
+<pre>
+=== "Python 3.7+"
+    ```python
+    from typing import Optional, Dict
+
+    def foo(bar: Optional[str]) -> Dict[str, str]:
+        ...
+    ```
+
+=== "Python 3.9+"
+    ```python
+    from typing import Optional
+    
+    
+    def foo(bar: Optional[str]) -> dict[str, str]:
+        ...
+    ```
+
+==== "Python 3.10+"
+    ```python
+    def foo(bar: str | None) -> dict[str, str]:
+        ...
+    ```
+</pre>
+
+#### Nested blocks
+
+Nested tabs are supported as well:
+
+**Input**
+
+<pre>
+=== "Level 1-1"
+
+    === "Level 2-1"
+
+        ```python
+        from typing import List
+        x: List[str]
+        ```
+
+    === "Level 2-2"
+    
+        Hello, world!
+
+=== "Level 1-2"
+
+    Goodbye, world!
+</pre>
+
+**Equivalent markdown**
+
+<pre>
+=== "Level 1-1"
+
+    === "Level 2-1"
+
+        === "Python 3.7+"
+            ```python
+            from typing import List
+            x: List[str]
+            ```
+        
+        === "Python 3.9+"
+            ```python
+            x: list[str]
+            ```
+
+    === "Level 2-2"
+
+        Goodbye, world!
+
+=== "Level 1-2"
+    Hello, world!
+    
+</pre>
+
+### Selectively disable
+
+You can disable conversion for a single code block:
+
+````
+<!-- autopytabs: disable-block -->
+```python
+from typing import Set, Optional
+
+def bar(baz: Optional[str]) -> Set[str]:
+    ...
+```
+````
+
+Or for whole sections / files
+
+```
+<!-- autopytabs: disable -->
+everything after this will be ignored
+<!-- autopytabs: enable -->
+re-enables conversion again
+```
+
+### Compatibility with `pymdownx.snippets`
+
+If the `pymdownx.snippets` extension is used, make sure that it runs **before** AutoPyTab
+
+<hr>
+
+## Usage with Sphinx
+
+AutPyTabs provides a Sphinx extension `auto_pytabs.sphinx_ext`, enabling its functionality
+for the `.. code-block` and `.. literalinclude` directives.
+
+<h3 id="sphinx-config">Configuration</h3>
+
+#### Example configuration
+
+```python
+extensions = ["auto_pytabs.sphinx_ext", "sphinx_design"]
+
+auto_pytabs_min_version = (3, 7)  # optional
+auto_pytabs_max_version = (3, 11)  # optional
+auto_pytabs_tab_title_template = "Python {min_version}+"  # optional 
+# auto_pytabs_no_cache = True  # disabled file system caching
+# auto_pytabs_compat_mode = True  # enable compatibility mode
+```
+
+#### Available configuration options
+
+| Name                             | Default                   | Description                                      |
+| -------------------------------- | ------------------------- | ------------------------------------------------ |
+| `auto_pytabs_min_version`        | `(3, 7)`                  | Minimum python version to generate code for      |
+| `auto_pytabs_max_version`        | `(3, 7)`                  | Maximum python version to generate code for      |
+| `auto_pytabs_tab_title_template` | `"Python {min_version}+"` | Template for tab titles                          |
+| `auto_pytabs_no_cache`           | `False`                   | Disable file system caching                      |
+| `auto_pytabs_compat_mode`        | `False`                   | Enable [compatibility mode](#compatibility-mode) |
+
+<h3 id="sphinx-examples">Examples</h3>
+
+**Input**
+
+```rst
+.. code-block:: python
+
+   from typing import Optional, Dict
+   
+   def foo(bar: Optional[str]) -> Dict[str, str]:
+       ...
+```
+
+**Equivalent ReST**
+
+```rst
+.. tab-set::
+
+   .. tab-item:: Python 3.7+
+   
+       .. code-block:: python
+       
+          from typing import Optional, Dict
+      
+          def foo(bar: Optional[str]) -> Dict[str, str]:
+              ...
+
+   .. tab-item:: Python 3.9+
+   
+      .. code-block:: python
+      
+          from typing import Optional
+          
+          
+          def foo(bar: Optional[str]) -> dict[str, str]:
+              ...
+
+   .. tab-item:: Python 3.10+
+   
+      .. code-block:: python
+      
+          def foo(bar: str | None) -> dict[str, str]:
+              ...
+
+```
+
+### Directives
+
+AutoPyTabs overrides the built-in `code-block` and `literal-include` directives,
+extending them with auto-upgrade and tabbing functionality, which means no special
+directives, and therefore changes to existing documents are needed.
+
+Additionally, a `:no-upgrade:` option is added to the directives, which can be used to
+selectively fall back the default behaviour.
+
+Two new directives are provided as well:
+
+- `.. pytabs-code-block::`
+- `.. pytabs-literalinclude::`
+
+which by default act exactly like `.. code-block` and `.. literalinclude` respectively,
+and are mainly to provide AutoPyTab's functionality in [compatibility mode](#compatibility-mode).
+
+### Compatibility mode
+
+If you don't want the default behaviour of directive overrides, and instead wish to use the
+`.. pytabs-` directives manually (e.g. because of compatibility issues with other extensions
+or because you only want to apply it to select code blocks) you can make use AutoPyTabs' compatibility
+mode. To enable it, simply use the `auto_pytabs_compat_mode = True` in `conf.py`. Now, only content within `.. pytabs-`
+directives will be upgraded.
+
+### Compatibility with other extensions
+
+Normally the directive overrides don't cause any problems and are very convenient,
+since no changes to existing documents have to be made. However, if other extensions are included,
+which themselves override one of those directives, one of them will inadvertently override the other,
+depending on the order they're defined in `extensions`.
+
+To combat this, you can use the [compatibility mode](#compatibility-mode) extension instead, which
+only includes the new directives.
+
+If you control the conflicting overrides, you can alternatively inherit from
+`auto_py_tabs.sphinx_ext.CodeBlockOverride` and `auto_py_tabs.sphinx_ext.LiteralIncludeOverride`
+instead of `sphinx.directives.code.CodeBlock` and `sphinx.directives.code.LiteralInclude` respectively.
 
-setup(**setup_kwargs)
```

