# Comparing `tmp/mukkebude-0.0.2.tar.gz` & `tmp/mukkebude-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mukkebude-0.0.2.tar", max compression
+gzip compressed data, was "mukkebude-0.1.1.tar", max compression
```

## Comparing `mukkebude-0.0.2.tar` & `mukkebude-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1844 2023-04-12 17:08:12.215978 mukkebude-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 14:43:38.566031 mukkebude-0.0.2/mukkeBude/__init__.py
--rw-r--r--   0        0        0     2741 2023-04-12 15:38:06.321369 mukkebude-0.0.2/mukkeBude/mapping.py
--rw-r--r--   0        0        0       99 2023-04-12 14:43:38.574030 mukkebude-0.0.2/mukkeBude/model/__init__.py
--rw-r--r--   0        0        0     7127 2023-04-12 16:49:35.292001 mukkebude-0.0.2/mukkeBude/model/mukke_bude_lstm.py
--rw-r--r--   0        0        0     7621 2023-04-12 16:49:56.352152 mukkebude-0.0.2/mukkeBude/model/mukke_bude_transformer.py
--rw-r--r--   0        0        0      447 2023-04-12 14:43:38.578031 mukkebude-0.0.2/mukkeBude/songs/generated_song_pokemon.mid
--rw-r--r--   0        0        0    17937 2023-04-12 15:35:24.880216 mukkebude-0.0.2/mukkeBude/utils.py
--rw-r--r--   0        0        0     1020 2023-04-12 16:31:27.500232 mukkebude-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 mukkebude-0.0.2/setup.py
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 mukkebude-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1844 2023-04-12 20:40:50.406306 mukkebude-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/__init__.py
+-rw-r--r--   0        0        0     2741 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/mapping.py
+-rw-r--r--   0        0        0       99 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/model/__init__.py
+-rw-r--r--   0        0        0     7127 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/model/mukke_bude_lstm.py
+-rw-r--r--   0        0        0     7621 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/model/mukke_bude_transformer.py
+-rw-r--r--   0        0        0      447 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/songs/generated_song_pokemon.mid
+-rw-r--r--   0        0        0    17937 2023-04-12 20:40:50.410306 mukkebude-0.1.1/mukkeBude/utils.py
+-rw-r--r--   0        0        0     1021 2023-04-12 20:40:50.414306 mukkebude-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 mukkebude-0.1.1/PKG-INFO
```

### Comparing `mukkebude-0.0.2/README.md` & `mukkebude-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mukkebude-0.0.2/mukkeBude/mapping.py` & `mukkebude-0.1.1/mukkeBude/mapping.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.0.2/mukkeBude/model/mukke_bude_lstm.py` & `mukkebude-0.1.1/mukkeBude/model/mukke_bude_lstm.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.0.2/mukkeBude/model/mukke_bude_transformer.py` & `mukkebude-0.1.1/mukkeBude/model/mukke_bude_transformer.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.0.2/mukkeBude/utils.py` & `mukkebude-0.1.1/mukkeBude/utils.py`

 * *Files identical despite different names*

### Comparing `mukkebude-0.0.2/pyproject.toml` & `mukkebude-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mukkeBude"
-version = "0.0.2"
+version = "v0.1.1"
 description = "A music generation library with transformer and lstm models',"
 authors = ["Florian Glaser <Florian.Glaser@ifm.com>", "Florian Herkommer <Florian.Herkommer@ifm.com>", "David Felder <David.Felder@ifm.com>"]
 readme = "README.md"
 homepage = "https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze"
 repository = "https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze"
 packages = [
     { include = "mukkeBude" }
```

### Comparing `mukkebude-0.0.2/setup.py` & `mukkebude-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,90 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['mukkeBude', 'mukkeBude.model']
-
-package_data = \
-{'': ['*'], 'mukkeBude': ['songs/*']}
-
-install_requires = \
-['keras-nlp==0.4.1',
- 'matplotlib>=3.7.1,<4.0.0',
- 'music21>=8.1.0,<9.0.0',
- 'sacremoses==0.0.53',
- 'tensorflow-text==2.10.0',
- 'tensorflow>=2.10.0,<2.11.0']
-
-setup_kwargs = {
-    'name': 'mukkebude',
-    'version': '0.0.2',
-    'description': "A music generation library with transformer and lstm models',",
-    'long_description': '# Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze\nZiel der Studienarbeit ist die Komposition eines kleinen Musikstücks. Die Komposition erfolgt mittels eines Neuronalen Netzes.\n\n# Usage\nHier wird beschrieben wir man das Projekt verwendet.\n\n## Installation\nUm die unter [demos](./demos/) bereitgestellten jupyter-notebook verwenden zu können, muss das Projekt mittels pip installiert werden.\nHierfür gibt es folgende Möglichkeiten:\n\n**GitHub Repo**\n```bash\n# Clone das Repo\ngit clone git@github.com:DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze.git mukkeBude\ncd mukkeBude\n\n# Installieren mittels pip\npip install .\n```\n\n**PyPi**\n```bash\npip install mukkeBude\n```\n\nFür die Verwendung der **Jupyter-Notebooks** muss jupyter-lab zusätzlich installiert werden!\n```bash\npip install jupyterlab\n``` \n\n## Verwendung\nNach einer erfolgreichen installtion kann das modul mittels `import mukkeBude` verwendet werden. Entsprechende Beispiele sind unter [demos](./demos/) zu finden.\n\n# Developing\n\nHier wird beschrieben, wie man seine Entwicklungsumgebung entsprechend vorbereitet, um an dem Projekt zu entwicklen.\nEmpfohlen ist die Verwendung von **Conda**, da hier die Verwendung von der GPU deutlich einfach ist. Bei der Verwendung der anderen Methoden müssen \nunter Umständen weitere Schritte unternommen werden, um die GPU zu verwenden.\n\n## Conda\nInstallation mithilfe von conda:\n\n```bash\nconda env create -f environment.yml\nconda activate tf-gpu\n\n# Enable GPU support on Linux (need to be done in every new shell)\nexport LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/\n```\n\n## Pip\nOhne venv:\n\n```bash\npip install -r requirements-dev.txt\n```\n\nMit venv:\n\n```bash\npython -m venv .venv\nsource .venv/bin/activate\n\npip install -r requirements-dev.txt\n```\n\n## Poetry\n```bash\npoetry install --with=dev\npoetry shell\n```',
-    'author': 'Florian Glaser',
-    'author_email': 'Florian.Glaser@ifm.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9.0,<3.10.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: mukkebude
+Version: 0.1.1
+Summary: A music generation library with transformer and lstm models',
+Home-page: https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze
+Author: Florian Glaser
+Author-email: Florian.Glaser@ifm.com
+Requires-Python: >=3.9.0,<3.10.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: keras-nlp (==0.4.1)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: music21 (>=8.1.0,<9.0.0)
+Requires-Dist: sacremoses (==0.0.53)
+Requires-Dist: tensorflow (>=2.10.0,<2.11.0)
+Requires-Dist: tensorflow-text (==2.10.0)
+Project-URL: Repository, https://github.com/DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze
+Description-Content-Type: text/markdown
+
+# Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze
+Ziel der Studienarbeit ist die Komposition eines kleinen Musikstücks. Die Komposition erfolgt mittels eines Neuronalen Netzes.
+
+# Usage
+Hier wird beschrieben wir man das Projekt verwendet.
+
+## Installation
+Um die unter [demos](./demos/) bereitgestellten jupyter-notebook verwenden zu können, muss das Projekt mittels pip installiert werden.
+Hierfür gibt es folgende Möglichkeiten:
+
+**GitHub Repo**
+```bash
+# Clone das Repo
+git clone git@github.com:DHBW-FN-TIT20/Komposition-eines-Musikstuecks-mittels-Neuronaler-Netze.git mukkeBude
+cd mukkeBude
+
+# Installieren mittels pip
+pip install .
+```
+
+**PyPi**
+```bash
+pip install mukkeBude
+```
+
+Für die Verwendung der **Jupyter-Notebooks** muss jupyter-lab zusätzlich installiert werden!
+```bash
+pip install jupyterlab
+``` 
+
+## Verwendung
+Nach einer erfolgreichen installtion kann das modul mittels `import mukkeBude` verwendet werden. Entsprechende Beispiele sind unter [demos](./demos/) zu finden.
+
+# Developing
+
+Hier wird beschrieben, wie man seine Entwicklungsumgebung entsprechend vorbereitet, um an dem Projekt zu entwicklen.
+Empfohlen ist die Verwendung von **Conda**, da hier die Verwendung von der GPU deutlich einfach ist. Bei der Verwendung der anderen Methoden müssen 
+unter Umständen weitere Schritte unternommen werden, um die GPU zu verwenden.
+
+## Conda
+Installation mithilfe von conda:
+
+```bash
+conda env create -f environment.yml
+conda activate tf-gpu
+
+# Enable GPU support on Linux (need to be done in every new shell)
+export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/
+```
+
+## Pip
+Ohne venv:
+
+```bash
+pip install -r requirements-dev.txt
+```
+
+Mit venv:
+
+```bash
+python -m venv .venv
+source .venv/bin/activate
+
+pip install -r requirements-dev.txt
+```
+
+## Poetry
+```bash
+poetry install --with=dev
+poetry shell
+```
```

