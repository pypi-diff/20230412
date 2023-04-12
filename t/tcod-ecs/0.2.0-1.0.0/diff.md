# Comparing `tmp/tcod-ecs-0.2.0.tar.gz` & `tmp/tcod-ecs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod-ecs-0.2.0.tar", last modified: Wed Mar 29 07:54:11 2023, max compression
+gzip compressed data, was "tcod-ecs-1.0.0.tar", last modified: Wed Apr 12 01:34:08 2023, max compression
```

## Comparing `tcod-ecs-0.2.0.tar` & `tcod-ecs-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ecs-0.2.0/.flake8
--rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ecs-0.2.0/.gitattributes
--rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ecs-0.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1536 2023-03-23 23:43:11.397588 tcod-ecs-0.2.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     4409 2023-03-27 00:31:15.054038 tcod-ecs-0.2.0/.gitignore
--rw-r--r--   0        0        0      772 2023-03-25 01:31:11.142017 tcod-ecs-0.2.0/.readthedocs.yml
--rw-r--r--   0        0        0     1325 2023-03-23 23:46:53.826542 tcod-ecs-0.2.0/.vscode/launch.json
--rw-r--r--   0        0        0     1452 2023-03-29 04:50:48.892084 tcod-ecs-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0     1238 2023-03-23 23:46:52.209465 tcod-ecs-0.2.0/.vscode/tasks.json
--rw-r--r--   0        0        0      277 2022-12-11 01:04:39.899008 tcod-ecs-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-03-26 20:09:04.799655 tcod-ecs-0.2.0/LICENSE
--rw-r--r--   0        0        0     7692 2023-03-29 07:39:07.207779 tcod-ecs-0.2.0/README.md
--rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ecs-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      115 2023-03-24 00:06:33.545046 tcod-ecs-0.2.0/docs/api.rst
--rw-r--r--   0        0        0     2072 2023-03-24 00:06:35.156705 tcod-ecs-0.2.0/docs/conf.py
--rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ecs-0.2.0/docs/head.md
--rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ecs-0.2.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ecs-0.2.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-03-25 01:28:10.449866 tcod-ecs-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     3498 2023-03-28 23:14:23.963767 tcod-ecs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    20649 2023-03-29 07:53:46.277712 tcod-ecs-0.2.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     4044 2023-03-29 02:09:03.723709 tcod-ecs-0.2.0/tcod/ecs/test_ecs.py
--rw-r--r--   0        0        0     8664 1970-01-01 00:00:00.000000 tcod-ecs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ecs-1.0.0/.flake8
+-rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ecs-1.0.0/.gitattributes
+-rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ecs-1.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1706 2023-04-09 03:23:14.272745 tcod-ecs-1.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     4409 2023-03-27 00:31:15.054038 tcod-ecs-1.0.0/.gitignore
+-rw-r--r--   0        0        0      772 2023-03-25 01:31:11.142017 tcod-ecs-1.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1325 2023-03-23 23:46:53.826542 tcod-ecs-1.0.0/.vscode/launch.json
+-rw-r--r--   0        0        0     1493 2023-04-12 00:56:27.890449 tcod-ecs-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1238 2023-03-23 23:46:52.209465 tcod-ecs-1.0.0/.vscode/tasks.json
+-rw-r--r--   0        0        0      327 2023-04-12 01:32:27.757712 tcod-ecs-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1100 2023-03-26 20:09:04.799655 tcod-ecs-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8642 2023-04-12 01:06:47.372874 tcod-ecs-1.0.0/README.md
+-rw-r--r--   0        0        0      581 2023-04-12 01:13:36.306949 tcod-ecs-1.0.0/conftest.py
+-rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ecs-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0      115 2023-03-24 00:06:33.545046 tcod-ecs-1.0.0/docs/api.rst
+-rw-r--r--   0        0        0     2072 2023-03-24 00:06:35.156705 tcod-ecs-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ecs-1.0.0/docs/head.md
+-rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ecs-1.0.0/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ecs-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-03-25 01:28:10.449866 tcod-ecs-1.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     3569 2023-04-12 01:31:24.101693 tcod-ecs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    29235 2023-04-12 01:30:58.631013 tcod-ecs-1.0.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0     7285 2023-04-12 01:13:36.373623 tcod-ecs-1.0.0/tcod/ecs/test_ecs.py
+-rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 tcod-ecs-1.0.0/PKG-INFO
```

### Comparing `tcod-ecs-0.2.0/.gitattributes` & `tcod-ecs-1.0.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/.github/workflows/python-package.yml` & `tcod-ecs-1.0.0/.github/workflows/python-package.yml`

 * *Files 12% similar despite different names*

```diff
@@ -27,35 +27,38 @@
     steps:
       - uses: actions/checkout@v3
       - name: Install isort
         run: pip install isort
       - name: isort
         run: isort tcod/ --check --diff
 
-  flake8:
+  ruff:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
-      - name: Install Flake8
-        run: pip install Flake8
-      - name: Flake8
-        run: flake8 tcod/
+      - name: Install Ruff
+        run: pip install ruff
+      - name: Ruff
+        run: ruff .
 
   test:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
-        name: Setup Python
+        name: Setup Python ${{ matrix.python-version }}
         with:
-          python-version: "3.8"
+          python-version: ${{ matrix.python-version }}
       - name: Install package
         run: pip install -e ".[test]"
       - name: Mypy
         uses: liskin/gh-problem-matcher-wrap@v1
         with:
           linters: mypy
-          run: mypy --show-column-numbers
+          run: mypy --show-column-numbers --python-version ${{ matrix.python-version }}
       - name: Run tests
         run: pytest --cov-report=xml
       - name: Upload coverage
         uses: codecov/codecov-action@v3
```

### Comparing `tcod-ecs-0.2.0/.gitignore` & `tcod-ecs-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/.readthedocs.yml` & `tcod-ecs-1.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/.vscode/launch.json` & `tcod-ecs-1.0.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/.vscode/settings.json` & `tcod-ecs-1.0.0/.vscode/settings.json`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,18 @@
     ],
     "editor.formatOnSave": true,
     "files.trimFinalNewlines": true,
     "files.insertFinalNewline": true,
     "files.trimTrailingWhitespace": true,
     "cSpell.words": [
         "automodule",
+        "autouse",
         "Benesch",
         "codecov",
+        "doctests",
         "dtype",
         "genindex",
         "hashable",
         "intersphinx",
         "isort",
         "ivar",
         "libtcod",
```

### Comparing `tcod-ecs-0.2.0/.vscode/tasks.json` & `tcod-ecs-1.0.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/LICENSE` & `tcod-ecs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/README.md` & `tcod-ecs-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,36 +44,45 @@
 
 New entities can be created with `World.new_entity`.
 An entity always knows about its assigned world.
 Worlds only know about their entities once the entity is assigned a name, component, tag, or relation.
 An entity is identified by its "Python identity" rather than with a low-level stand-in identifier.
 
 ```py
-
 >>> entity = world.new_entity(name="MyEntity")  # Name is optional and can be any hashable, not just str.
 >>> entity
 <Entity name='MyEntity'>
 >>> entity.world is world  # Worlds can always be accessed from their entity.
 True
 >>> world.named["MyEntity"]  # Named entities can be accessed with `World.named`.
 <Entity name='MyEntity'>
 >>> world.named.get("Missing") is None  # `World.named` acts like a dictionary, including assignment and `.get()`.
 True
 
 ```
 
+## Serialization
+
+Worlds are normal Python objects and can be pickled as long as all stored components can be pickled.
+
+```py
+>>> import pickle
+>>> pickled_data: bytes = pickle.dumps(world)
+>>> world = pickle.loads(pickled_data)
+
+```
+
 ## Components
 
 Components are instances of any Python type.
 These can be accessed, assigned, or removed from entities via the dict-like `Entity.components` attribute.
 The type is used as the key to access the component.
 The types used can be custom classes or standard Python types.
 
 ```py
-
 >>> import attrs
 >>> entity = world.new_entity()
 >>> entity.components[int] = 42
 >>> entity.components[int]
 42
 >>> int in entity.components
 True
@@ -179,33 +188,41 @@
 >>> set(world.Q.all_of(tags=["player"])) == {entity}
 True
 
 ```
 
 ## Relations
 
-
+Use `Entity.relation_components[component_key][target] = component` to associate a relation with data.
+Use `Entity.relation_tags[tag] = target` to associate a tag exclusively with a target entity.
+Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
+Tags and relations share the same space then queried, so tags can not be in the format of a component key.
+Relations are unidirectional.
 
 ```py
+>>> @attrs.define
+... class OrbitOf:  # OrbitOf component.
+...     dist: int
+>>> LandedOn = "LandedOn"  # LandedOn tag.
 >>> star = world.new_entity()
 >>> planet = world.new_entity()
 >>> moon = world.new_entity()
 >>> ship = world.new_entity()
 >>> player = world.new_entity()
 >>> moon_rock = world.new_entity()
->>> OrbitOf = "OrbitOf"
->>> LandedOn = "LandedOn"
->>> planet.relations[OrbitOf] = star
->>> moon.relations[OrbitOf] = planet
->>> ship.relations[LandedOn] = moon
->>> moon_rock.relations[LandedOn] = moon
->>> player.relations[LandedOn] = moon_rock
+>>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
+>>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
+>>> ship.relation_tags[LandedOn] = moon
+>>> moon_rock.relation_tags[LandedOn] = moon
+>>> player.relation_tags[LandedOn] = moon_rock
 >>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
 True
->>> set(world.Q.all_of(relations=[(OrbitOf, None)])) == {planet, moon}
+>>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
+True
+>>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
 True
->>> set(world.Q.all_of(relations=[(LandedOn, None)])) == {ship, moon_rock, player}
+>>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
 True
->>> set(world.Q.all_of(relations=[(LandedOn, None)]).none_of(relations=[(LandedOn, moon)])) == {player}
+>>> set(world.Q.all_of(relations=[(LandedOn, ...)]).none_of(relations=[(LandedOn, moon)])) == {player}
 True
 
 ```
```

### Comparing `tcod-ecs-0.2.0/docs/Makefile` & `tcod-ecs-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/docs/conf.py` & `tcod-ecs-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/docs/make.bat` & `tcod-ecs-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tcod-ecs-0.2.0/pyproject.toml` & `tcod-ecs-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "tcod-ecs"
 authors = [{ name = "Kyle Benesch", email = "4b796c65+github@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
@@ -47,15 +47,15 @@
 line_length = 120
 profile = "black"
 skip_gitignore = true
 
 [tool.mypy] # https://mypy.readthedocs.io/en/stable/config_file.html
 files = "**/*.py"
 explicit_package_bases = true
-python_version = "3.8"
+python_version = "3.10"            # Type check Python version with EllipsisType.
 warn_unused_configs = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
```

### Comparing `tcod-ecs-0.2.0/PKG-INFO` & `tcod-ecs-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 0.2.0
+Version: 1.0.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions >=4.4.0
@@ -70,36 +70,45 @@
 
 New entities can be created with `World.new_entity`.
 An entity always knows about its assigned world.
 Worlds only know about their entities once the entity is assigned a name, component, tag, or relation.
 An entity is identified by its "Python identity" rather than with a low-level stand-in identifier.
 
 ```py
-
 >>> entity = world.new_entity(name="MyEntity")  # Name is optional and can be any hashable, not just str.
 >>> entity
 <Entity name='MyEntity'>
 >>> entity.world is world  # Worlds can always be accessed from their entity.
 True
 >>> world.named["MyEntity"]  # Named entities can be accessed with `World.named`.
 <Entity name='MyEntity'>
 >>> world.named.get("Missing") is None  # `World.named` acts like a dictionary, including assignment and `.get()`.
 True
 
 ```
 
+## Serialization
+
+Worlds are normal Python objects and can be pickled as long as all stored components can be pickled.
+
+```py
+>>> import pickle
+>>> pickled_data: bytes = pickle.dumps(world)
+>>> world = pickle.loads(pickled_data)
+
+```
+
 ## Components
 
 Components are instances of any Python type.
 These can be accessed, assigned, or removed from entities via the dict-like `Entity.components` attribute.
 The type is used as the key to access the component.
 The types used can be custom classes or standard Python types.
 
 ```py
-
 >>> import attrs
 >>> entity = world.new_entity()
 >>> entity.components[int] = 42
 >>> entity.components[int]
 42
 >>> int in entity.components
 True
@@ -205,34 +214,42 @@
 >>> set(world.Q.all_of(tags=["player"])) == {entity}
 True
 
 ```
 
 ## Relations
 
-
+Use `Entity.relation_components[component_key][target] = component` to associate a relation with data.
+Use `Entity.relation_tags[tag] = target` to associate a tag exclusively with a target entity.
+Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
+Tags and relations share the same space then queried, so tags can not be in the format of a component key.
+Relations are unidirectional.
 
 ```py
+>>> @attrs.define
+... class OrbitOf:  # OrbitOf component.
+...     dist: int
+>>> LandedOn = "LandedOn"  # LandedOn tag.
 >>> star = world.new_entity()
 >>> planet = world.new_entity()
 >>> moon = world.new_entity()
 >>> ship = world.new_entity()
 >>> player = world.new_entity()
 >>> moon_rock = world.new_entity()
->>> OrbitOf = "OrbitOf"
->>> LandedOn = "LandedOn"
->>> planet.relations[OrbitOf] = star
->>> moon.relations[OrbitOf] = planet
->>> ship.relations[LandedOn] = moon
->>> moon_rock.relations[LandedOn] = moon
->>> player.relations[LandedOn] = moon_rock
+>>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
+>>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
+>>> ship.relation_tags[LandedOn] = moon
+>>> moon_rock.relation_tags[LandedOn] = moon
+>>> player.relation_tags[LandedOn] = moon_rock
 >>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
 True
->>> set(world.Q.all_of(relations=[(OrbitOf, None)])) == {planet, moon}
+>>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
+True
+>>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
 True
->>> set(world.Q.all_of(relations=[(LandedOn, None)])) == {ship, moon_rock, player}
+>>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
 True
->>> set(world.Q.all_of(relations=[(LandedOn, None)]).none_of(relations=[(LandedOn, moon)])) == {player}
+>>> set(world.Q.all_of(relations=[(LandedOn, ...)]).none_of(relations=[(LandedOn, moon)])) == {player}
 True
 
 ```
```

