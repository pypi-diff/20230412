# Comparing `tmp/zeno_evals-0.1.3.tar.gz` & `tmp/zeno_evals-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeno_evals-0.1.3.tar", max compression
+gzip compressed data, was "zeno_evals-0.1.4.tar", max compression
```

## Comparing `zeno_evals-0.1.3.tar` & `zeno_evals-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     1082 2023-04-10 02:23:36.754895 zeno_evals-0.1.3/README.md
--rw-r--r--   0        0        0      464 2023-04-10 02:23:05.871904 zeno_evals-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 21:01:32.056333 zeno_evals-0.1.3/zeno_evals/__init__.py
--rw-r--r--   0        0        0     5858 2023-03-16 14:18:25.747559 zeno_evals-0.1.3/zeno_evals/main.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 zeno_evals-0.1.3/setup.py
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 zeno_evals-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      780 2023-04-11 22:55:02.248492 zeno_evals-0.1.4/README.md
+-rw-r--r--   0        0        0      520 2023-04-11 22:57:53.193770 zeno_evals-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 21:01:32.056333 zeno_evals-0.1.4/zeno_evals/__init__.py
+-rw-r--r--   0        0        0     5128 2023-04-11 22:57:06.636732 zeno_evals-0.1.4/zeno_evals/main.py
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 zeno_evals-0.1.4/setup.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 zeno_evals-0.1.4/PKG-INFO
```

### Comparing `zeno_evals-0.1.3/LICENSE.md` & `zeno_evals-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.3/setup.py` & `zeno_evals-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['fire>=0.5.0,<0.6.0', 'pandas>=1.5.3,<2.0.0', 'zenoml>=0.4.5,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['zeno-evals = zeno_evals.main:cli']}
 
 setup_kwargs = {
     'name': 'zeno-evals',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Visualize OpenAI evals with Zeno',
-    'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n*Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)*\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\nWe include an example looking at the [MedMCQA](https://github.com/openai/evals/pull/141) dataset (Thanks to @SinanAkkoyun):\n\n```bash\nzeno-evals ./example_medicine/example.jsonl --functions_file=./example_medicine/distill.py\n```\n\n### Todo\n\n- [ ] Support model-graded evaluations\n- [ ] Support custom evaluation templates (e.g. BLEU for translation)\n',
+    'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\n```bash\nzeno-evals ./example/example.jsonl\n```\n',
     'author': 'Alex Cabrera',
     'author_email': 'alex.cabrera@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `zeno_evals-0.1.3/PKG-INFO` & `zeno_evals-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno-evals
-Version: 0.1.3
+Version: 0.1.4
 Summary: Visualize OpenAI evals with Zeno
 Author: Alex Cabrera
 Author-email: alex.cabrera@gmail.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,18 +14,17 @@
 Requires-Dist: zenoml (>=0.4.5,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Zeno 🤝 OpenAI Evals
 
 Use [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).
 
-
 https://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov
 
-*Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)*
+_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_
 
 ### Usage
 
 ```bash
 pip install zeno-evals
 ```
 
@@ -35,18 +34,11 @@
 
 ```bash
 zeno-evals /tmp/evallogs/my_eval_cache.jsonl
 ```
 
 ### Example
 
-We include an example looking at the [MedMCQA](https://github.com/openai/evals/pull/141) dataset (Thanks to @SinanAkkoyun):
-
 ```bash
-zeno-evals ./example_medicine/example.jsonl --functions_file=./example_medicine/distill.py
+zeno-evals ./example/example.jsonl
 ```
 
-### Todo
-
-- [ ] Support model-graded evaluations
-- [ ] Support custom evaluation templates (e.g. BLEU for translation)
-
```

