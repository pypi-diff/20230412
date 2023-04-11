# Comparing `tmp/sphinxcontrib_autoyaml-1.1.0.tar.gz` & `tmp/sphinxcontrib_autoyaml-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_autoyaml-1.1.0.tar", max compression
+gzip compressed data, was "sphinxcontrib_autoyaml-1.1.1.tar", max compression
```

## Comparing `sphinxcontrib_autoyaml-1.1.0.tar` & `sphinxcontrib_autoyaml-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1079 2022-06-01 16:36:32.434862 sphinxcontrib_autoyaml-1.1.0/LICENSE
--rw-r--r--   0        0        0     2543 2022-07-11 20:04:21.210557 sphinxcontrib_autoyaml-1.1.0/README.md
--rw-r--r--   0        0        0      841 2023-02-12 15:27:26.360271 sphinxcontrib_autoyaml-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6889 2022-07-11 19:35:24.596703 sphinxcontrib_autoyaml-1.1.0/sphinxcontrib/autoyaml/__init__.py
--rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 sphinxcontrib_autoyaml-1.1.0/setup.py
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 sphinxcontrib_autoyaml-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2022-06-01 16:36:32.434862 sphinxcontrib_autoyaml-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2543 2022-07-11 20:04:21.210557 sphinxcontrib_autoyaml-1.1.1/README.md
+-rw-r--r--   0        0        0      841 2023-04-11 23:12:56.040721 sphinxcontrib_autoyaml-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7481 2023-04-11 22:34:15.766793 sphinxcontrib_autoyaml-1.1.1/sphinxcontrib/autoyaml/__init__.py
+-rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 sphinxcontrib_autoyaml-1.1.1/setup.py
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 sphinxcontrib_autoyaml-1.1.1/PKG-INFO
```

### Comparing `sphinxcontrib_autoyaml-1.1.0/LICENSE` & `sphinxcontrib_autoyaml-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_autoyaml-1.1.0/README.md` & `sphinxcontrib_autoyaml-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_autoyaml-1.1.0/pyproject.toml` & `sphinxcontrib_autoyaml-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'sphinxcontrib-autoyaml'
-version = '1.1.0'
+version = '1.1.1'
 description = 'Sphinx autodoc extension for documenting YAML files from comments'
 authors = ['Jakub Pieńkowski <jakub+sphinxcontrib-autoyaml@jakski.name>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/Jakski/sphinxcontrib-autoyaml'
 packages = [
   { include = "sphinxcontrib" },
```

### Comparing `sphinxcontrib_autoyaml-1.1.0/sphinxcontrib/autoyaml/__init__.py` & `sphinxcontrib_autoyaml-1.1.1/sphinxcontrib/autoyaml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ruamel.yaml.main import compose_all
 from ruamel.yaml.nodes import (
     MappingNode,
     SequenceNode,
     ScalarNode,
 )
+from ruamel.yaml import SafeLoader, Loader
 from docutils.statemachine import ViewList
 from docutils.parsers.rst import Directive
 from docutils import nodes
 from sphinx.util import logging
 from sphinx.util.docutils import switch_source_input
 from sphinx.errors import ExtensionError
 
@@ -23,15 +24,15 @@
         self.parent = parent
         self.children = []
         self.comments = comments
         if value is None:
             self.comment = None
         else:
             # Flow-style entries may attempt to incorrectly reuse comments
-            self.comment = self.comments.pop(value.start_mark.line + 1, None)
+            self.comment = self.comments.pop(self.value.start_mark.line + 1, None)
 
     def add_child(self, value):
         node = TreeNode(value, self.comments, self)
         self.children.append(node)
         return node
 
     def remove_child(self):
@@ -110,23 +111,29 @@
                     tree = tree.parent
                 unvisited.pop()
                 continue
             for node_item in node.value[index:]:
                 index += 1
                 unvisited[-1] = (node, index)
                 subtree = None
+                node_key = None
+                node_value = None
                 if isinstance(node, SequenceNode):
                     node_value = node_item
                 elif isinstance(node, MappingNode):
                     node_key, node_value = node_item
                     # Using complex structures for keys in YAML is possible as
                     # well, but it's currently not handled.
                     if not isinstance(node_key, ScalarNode):
                         continue
                     subtree = tree.add_child(node_key)
+                for i in (node_key, node_value):
+                    if isinstance(i, ScalarNode):
+                        for i in range(i.start_mark.line, i.end_mark.line + 1):
+                            comments.pop(i + 1, None)
                 if isinstance(node_value, (MappingNode, SequenceNode)) and (
                     len(unvisited) + 1 <= self.config.autoyaml_level
                     or self.config.autoyaml_level == 0
                 ):
                     unvisited.append((node_value, 0))
                     if subtree is not None:
                         tree = subtree
@@ -165,19 +172,25 @@
             unvisited.pop()
         return tree.comment
 
     def _parse_file(self, source_file):
         with open(source_file, "r") as f:
             source = f.read()
         comments = self._get_comments(source, source_file)
-        for doc in compose_all(source):
+        if self.config.autoyaml_safe_loader:
+            loader = SafeLoader
+        else:
+            loader = Loader
+        for doc in compose_all(source, loader):
             docs = self._generate_documentation(self._parse_document(doc, comments))
             if docs is not None:
                 yield docs
 
 
 def setup(app):
     app.add_directive("autoyaml", AutoYAMLDirective)
     app.add_config_value("autoyaml_root", "..", "env")
     app.add_config_value("autoyaml_doc_delimiter", "###", "env")
     app.add_config_value("autoyaml_comment", "#", "env")
     app.add_config_value("autoyaml_level", 1, "env")
+    # Set to false to preserve backward compatibility.
+    app.add_config_value("autoyaml_safe_loader", False, "env")
```

### Comparing `sphinxcontrib_autoyaml-1.1.0/setup.py` & `sphinxcontrib_autoyaml-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Sphinx>=3.5.1', 'ruamel.yaml>=0.16.12,<0.17.0']
 
 setup_kwargs = {
     'name': 'sphinxcontrib-autoyaml',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Sphinx autodoc extension for documenting YAML files from comments',
     'long_description': '# sphinxcontrib-autoyaml\n\nThis Sphinx autodoc extension documents YAML files from comments. Documentation\nis returned as reST definitions, e.g.:\n\nThis document:\n\n```\n###\n# Enable Nginx web server.\nenable_nginx: true\n\n###\n# Enable Varnish caching proxy.\nenable_varnish: true\n```\n\nwould be turned into text:\n\n```\nenable_nginx\n\n   Enable Nginx web server.\n\nenable_varnish\n\n   Enable Varnish caching proxy.\n```\n\nSee `tests/examples/output/*.yml` and `tests/examples/output/*.txt` for\nmore examples.\n\n`autoyaml` will take into account only comments which first line starts with\n`autoyaml_doc_delimiter`.\n\n## Usage\n\nYou can use `autoyaml` directive, where you want to extract comments\nfrom YAML file, e.g.:\n\n```\nSome title\n==========\n\nDocumenting single YAML file.\n\n.. autoyaml:: some_yml_file.yml\n```\n\n## Options\n\nOptions available to use in your configuration:\n\n- *autoyaml_root*(`..`)\n  Look for YAML files relatively to this directory.\n- *autoyaml_doc_delimiter*(`###`)\n  Character(s) which start a documentation comment.\n- *autoyaml_comment*(`#`)\n  Comment start character(s).\n- *autoyaml_level*(`1`)\n  Parse comments from nested structures n-levels deep.\n\n## Installing\n\nIssue command:\n\n```\npip install sphinxcontrib-autoyaml\n```\n\nAnd add extension in your project\'s ``conf.py``:\n\n```\nextensions = ["sphinxcontrib.autoyaml"]\n```\n\n## Caveats\n\n### Mapping keys nested in sequences\n\nSequences are traversed as well, but they are not represented in output\ndocumentation. This extension focuses only on documenting mapping keys. It means\nthat structure like this:\n\n```yaml\nkey:\n  ###\n  # comment1\n  - - inner_key1: value\n      ###\n      # comment2\n      inner_key2: value\n  ###\n  # comment3\n  - inner_key3: value\n```\n\nwill be flattened, so it will appear as though inner keys exist directly under\n`key`. Duplicated key documentation will be duplicated in output as well. See\n`tests/examples/output/comment-in-nested-sequence.txt` and\n`tests/examples/output/comment-in-nested-sequence.yml` to get a better\nunderstanding how sequences are processed.\n\n### Complex mapping keys\n\nYAML allows for complex mapping keys like so:\n\n```yaml\n[1, 2]: value\n```\n\nThese kind of keys won\'t be documented in output, because it\'s unclear how they\nshould be represented as a string.\n\n### Flow-style entries\n\nYAML allows writing complex data structures in single line like JSON.\nDocumentation is generated only for the first key in such entry, so this:\n\n```yaml\n###\n# comment\nkey: {key1: value, key2: value, key3: value}\n```\n\nwould yield documentation only for `key`.\n',
     'author': 'Jakub Pieńkowski',
     'author_email': 'jakub+sphinxcontrib-autoyaml@jakski.name',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Jakski/sphinxcontrib-autoyaml',
```

### Comparing `sphinxcontrib_autoyaml-1.1.0/PKG-INFO` & `sphinxcontrib_autoyaml-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-autoyaml
-Version: 1.1.0
+Version: 1.1.1
 Summary: Sphinx autodoc extension for documenting YAML files from comments
 Home-page: https://github.com/Jakski/sphinxcontrib-autoyaml
 License: MIT
 Author: Jakub Pieńkowski
 Author-email: jakub+sphinxcontrib-autoyaml@jakski.name
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 3 - Alpha
```

