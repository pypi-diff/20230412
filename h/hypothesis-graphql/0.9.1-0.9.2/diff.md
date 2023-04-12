# Comparing `tmp/hypothesis-graphql-0.9.1.tar.gz` & `tmp/hypothesis_graphql-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-graphql-0.9.1.tar", max compression
+gzip compressed data, was "hypothesis_graphql-0.9.2.tar", max compression
```

## Comparing `hypothesis-graphql-0.9.1.tar` & `hypothesis_graphql-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/LICENSE
--rw-r--r--   0        0        0     4306 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/README.md
--rw-r--r--   0        0        0     1570 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      117 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/__init__.py
--rw-r--r--   0        0        0        0 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/__init__.py
--rw-r--r--   0        0        0     1808 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/aliases.py
--rw-r--r--   0        0        0      847 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/ast.py
--rw-r--r--   0        0        0      179 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/containers.py
--rw-r--r--   0        0        0     1822 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/factories.py
--rw-r--r--   0        0        0     3896 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/primitives.py
--rw-r--r--   0        0        0    20922 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/strategy.py
--rw-r--r--   0        0        0     1409 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/validation.py
--rw-r--r--   0        0        0      176 2022-09-02 07:38:48.609079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/cache.py
--rw-r--r--   0        0        0     1486 2022-09-02 07:38:48.613079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/nodes.py
--rw-r--r--   0        0        0        0 2022-09-02 07:38:48.613079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/py.typed
--rw-r--r--   0        0        0      140 2022-09-02 07:38:48.613079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/strategies.py
--rw-r--r--   0        0        0      681 2022-09-02 07:38:48.613079 hypothesis-graphql-0.9.1/src/hypothesis_graphql/types.py
--rw-r--r--   0        0        0     5296 1970-01-01 00:00:00.000000 hypothesis-graphql-0.9.1/setup.py
--rw-r--r--   0        0        0     5845 1970-01-01 00:00:00.000000 hypothesis-graphql-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4306 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/README.md
+-rw-r--r--   0        0        0     1616 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      117 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/__init__.py
+-rw-r--r--   0        0        0     1808 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/aliases.py
+-rw-r--r--   0        0        0      847 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/ast.py
+-rw-r--r--   0        0        0      179 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/containers.py
+-rw-r--r--   0        0        0     1822 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/factories.py
+-rw-r--r--   0        0        0     3896 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/primitives.py
+-rw-r--r--   0        0        0    20922 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/strategy.py
+-rw-r--r--   0        0        0     1409 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/validation.py
+-rw-r--r--   0        0        0      176 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/cache.py
+-rw-r--r--   0        0        0     1486 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/nodes.py
+-rw-r--r--   0        0        0        0 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/py.typed
+-rw-r--r--   0        0        0      140 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/strategies.py
+-rw-r--r--   0        0        0      681 2022-11-07 21:19:20.795278 hypothesis_graphql-0.9.2/src/hypothesis_graphql/types.py
+-rw-r--r--   0        0        0     5296 1970-01-01 00:00:00.000000 hypothesis_graphql-0.9.2/setup.py
+-rw-r--r--   0        0        0     5947 1970-01-01 00:00:00.000000 hypothesis_graphql-0.9.2/PKG-INFO
```

### Comparing `hypothesis-graphql-0.9.1/LICENSE` & `hypothesis_graphql-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/README.md` & `hypothesis_graphql-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/pyproject.toml` & `hypothesis_graphql-0.9.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hypothesis-graphql"
-version = "0.9.1"
+version = "0.9.2"
 description = "Hypothesis strategies for GraphQL queries"
 keywords = ["hypothesis", "graphql", "testing"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Framework :: Hypothesis",
     "Intended Audience :: Developers",
@@ -12,28 +12,29 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Testing",
 ]
 authors = ["Dmitry Dygalo <dadygalo@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Stranger6667/hypothesis-graphql"
 license = "MIT"
 include = ["src/hypothesis_graphql/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 hypothesis = ">=5.8.0,<7.0"
 graphql-core = ">=3.1.0,<3.3.0"
-attrs = ">20.3.0,<=21.4.0"
+attrs = ">20.3.0,<=22.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.0"
 
 [tool.black]
 line-length = 120
 target_version = ["py37"]
```

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/aliases.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/aliases.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/ast.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/ast.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/factories.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/factories.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/primitives.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/primitives.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/strategy.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/_strategies/validation.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/_strategies/validation.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/nodes.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/nodes.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/src/hypothesis_graphql/types.py` & `hypothesis_graphql-0.9.2/src/hypothesis_graphql/types.py`

 * *Files identical despite different names*

### Comparing `hypothesis-graphql-0.9.1/setup.py` & `hypothesis_graphql-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 packages = \
 ['hypothesis_graphql', 'hypothesis_graphql._strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['attrs>20.3.0,<=21.4.0',
+['attrs>20.3.0,<=22.1.0',
  'graphql-core>=3.1.0,<3.3.0',
  'hypothesis>=5.8.0,<7.0']
 
 setup_kwargs = {
     'name': 'hypothesis-graphql',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Hypothesis strategies for GraphQL queries',
     'long_description': '# hypothesis-graphql\n\n[![Build](https://github.com/Stranger6667/hypothesis-graphql/workflows/build/badge.svg)](https://github.com/Stranger6667/hypothesis-graphql/actions)\n[![Coverage](https://codecov.io/gh/Stranger6667/hypothesis-graphql/branch/master/graph/badge.svg)](https://codecov.io/gh/Stranger6667/hypothesis-graphql/branch/master)\n[![Version](https://img.shields.io/pypi/v/hypothesis-graphql.svg)](https://pypi.org/project/hypothesis-graphql/)\n[![Python versions](https://img.shields.io/pypi/pyversions/hypothesis-graphql.svg)](https://pypi.org/project/hypothesis-graphql/)\n[![Chat](https://img.shields.io/discord/938139740912369755)](https://discord.gg/VnxfdFmBUp)\n[![License](https://img.shields.io/pypi/l/hypothesis-graphql.svg)](https://opensource.org/licenses/MIT)\n\n<h4 align="center">\nGenerate queries matching your GraphQL schema, and use them to verify your backend implementation\n</h4>\n\nIt is a Python library that provides a set of [Hypothesis](https://github.com/HypothesisWorks/hypothesis/tree/master/hypothesis-python) strategies that\nlet you write tests parametrized by a source of examples.\nGenerated queries have arbitrary depth and may contain any subset of GraphQL types defined in the input schema.\nThey expose edge cases in your code that are unlikely to be found otherwise.\n\n[Schemathesis](https://github.com/schemathesis/schemathesis) provides a higher-level interface around this library and finds server crashes automatically.\n\n## Usage\n\n`hypothesis-graphql` provides the `from_schema` function, which takes a GraphQL schema and returns a Hypothesis strategy for\nGraphQL queries matching the schema:\n\n```python\nfrom hypothesis import given\nfrom hypothesis_graphql import from_schema\nimport requests\n\n# Strings and `graphql.GraphQLSchema` are supported\nSCHEMA = """\ntype Book {\n  title: String\n  author: Author\n}\n\ntype Author {\n  name: String\n  books: [Book]\n}\n\ntype Query {\n  getBooks: [Book]\n  getAuthors: [Author]\n}\n\ntype Mutation {\n  addBook(title: String!, author: String!): Book!\n  addAuthor(name: String!): Author!\n}\n"""\n\n\n@given(from_schema(SCHEMA))\ndef test_graphql(query):\n    # Will generate samples like these:\n    #\n    # {\n    #   getBooks {\n    #     title\n    #   }\n    # }\n    #\n    # mutation {\n    #   addBook(title: "H4Z\\u7869", author: "\\u00d2"){\n    #     title\n    #   }\n    # }\n    response = requests.post("http://127.0.0.1/graphql", json={"query": query})\n    assert response.status_code == 200\n    assert response.json().get("errors") is None\n```\n\nIt is also possible to generate queries or mutations separately with `hypothesis_graphql.queries` and `hypothesis_graphql.mutations`.\n\n### Customization\n\nTo restrict the set of fields in generated operations use the `fields` argument:\n\n```python\n@given(from_schema(SCHEMA, fields=["getAuthors"]))\ndef test_graphql(query):\n    # Only `getAuthors` will be generated\n    ...\n```\n\nIt is also possible to generate custom scalars. For example, `Date`:\n\n```python\nfrom hypothesis import strategies as st, given\nfrom hypothesis_graphql import from_schema, nodes\n\nSCHEMA = """\nscalar Date\n\ntype Query {\n  getByDate(created: Date!): Int\n}\n"""\n\n\n@given(\n    from_schema(\n        SCHEMA,\n        custom_scalars={\n            # Standard scalars work out of the box, for custom ones you need\n            # to pass custom strategies that generate proper AST nodes\n            "Date": st.dates().map(nodes.String)\n        },\n    )\n)\ndef test_graphql(query):\n    # Example:\n    #\n    #  { getByDate(created: "2000-01-01") }\n    #\n    ...\n```\n\nThe `hypothesis_graphql.nodes` module includes a few helpers to generate various node types:\n\n- `String` -> `graphql.StringValueNode`\n- `Float` -> `graphql.FloatValueNode`\n- `Int` -> `graphql.IntValueNode`\n- `Object` -> `graphql.ObjectValueNode`\n- `List` -> `graphql.ListValueNode`\n- `Boolean` -> `graphql.BooleanValueNode`\n- `Enum` -> `graphql.EnumValueNode`\n- `Null` -> `graphql.NullValueNode` (a constant, not a function)\n\nThey exist because classes like `graphql.StringValueNode` can\'t be directly used in `map` calls due to kwarg-only arguments.\n\n## License\n\nThe code in this project is licensed under [MIT license](https://opensource.org/licenses/MIT).\nBy contributing to `hypothesis-graphql`, you agree that your contributions will be licensed under its MIT license.\n',
     'author': 'Dmitry Dygalo',
     'author_email': 'dadygalo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Stranger6667/hypothesis-graphql',
```

### Comparing `hypothesis-graphql-0.9.1/PKG-INFO` & `hypothesis_graphql-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-graphql
-Version: 0.9.1
+Version: 0.9.2
 Summary: Hypothesis strategies for GraphQL queries
 Home-page: https://github.com/Stranger6667/hypothesis-graphql
 License: MIT
 Keywords: hypothesis,graphql,testing
 Author: Dmitry Dygalo
 Author-email: dadygalo@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -16,23 +16,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: attrs (>20.3.0,<=21.4.0)
+Requires-Dist: attrs (>20.3.0,<=22.1.0)
 Requires-Dist: graphql-core (>=3.1.0,<3.3.0)
 Requires-Dist: hypothesis (>=5.8.0,<7.0)
 Project-URL: Repository, https://github.com/Stranger6667/hypothesis-graphql
 Description-Content-Type: text/markdown
 
 # hypothesis-graphql
```

