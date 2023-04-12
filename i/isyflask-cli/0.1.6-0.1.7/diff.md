# Comparing `tmp/isyflask_cli-0.1.6.tar.gz` & `tmp/isyflask_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyflask_cli-0.1.6.tar", max compression
+gzip compressed data, was "isyflask_cli-0.1.7.tar", max compression
```

## Comparing `isyflask_cli-0.1.6.tar` & `isyflask_cli-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1371 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/__init__.py
--rw-r--r--   0        0        0       51 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/__main__.py
--rw-r--r--   0        0        0      477 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/cli.py
--rw-r--r--   0        0        0     4980 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/globals.py
--rw-r--r--   0        0        0        0 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/src/model/__init__.py
--rw-r--r--   0        0        0     2503 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/src/model/model.py
--rw-r--r--   0        0        0        0 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/src/project/__init__.py
--rw-r--r--   0        0        0     2261 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/src/project/project.py
--rw-r--r--   0        0        0     1690 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/src/utils/folders.py
--rw-r--r--   0        0        0      712 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/src/utils/strings.py
--rw-r--r--   0        0        0     2263 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/isyflask_cli/src/utils/template_gen.py
--rw-r--r--   0        0        0      536 2023-04-03 04:31:01.874348 isyflask_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 isyflask_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1476 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/__main__.py
+-rw-r--r--   0        0        0      477 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/cli.py
+-rw-r--r--   0        0        0     4980 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/globals.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/model/__init__.py
+-rw-r--r--   0        0        0     2503 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/project/__init__.py
+-rw-r--r--   0        0        0     2261 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/project/project.py
+-rw-r--r--   0        0        0     1690 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/utils/folders.py
+-rw-r--r--   0        0        0      712 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/utils/strings.py
+-rw-r--r--   0        0        0     2263 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/utils/template_gen.py
+-rw-r--r--   0        0        0      738 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 isyflask_cli-0.1.7/PKG-INFO
```

### Comparing `isyflask_cli-0.1.6/README.md` & `isyflask_cli-0.1.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,30 @@
 
 Para _macOS_ o _linux_:
 ````commandline
 python -m venv venv
 source ./venv/Scripts/activate
 ````
 
-Posteriormente instale el cli
+## Instalacion
+Para instalar el CLI ejecute el siguiente comando
+
+```
+python -m pip install --upgrade pip
+```
 
 ````commandline
 pip install isyflask-cli
 ````
 
 Para iniciar un proyecto ejecute el siguiente comando y responda las preguntas que salgan en el prompt:
 
 ````commandline
 isyflask-cli project init
+cd <folder project name>
 pip install -r requirements.txt
 ````
 
 Cambie el directorio al generado en el paso anterior. Utilizando *Docker*, el proyecto se levanta utilizando el siguiente comando:
 
 ````commandline
 docker-compose up
```

### Comparing `isyflask_cli-0.1.6/isyflask_cli/globals.py` & `isyflask_cli-0.1.7/isyflask_cli/globals.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.6/isyflask_cli/src/model/model.py` & `isyflask_cli-0.1.7/isyflask_cli/src/model/model.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.6/isyflask_cli/src/project/project.py` & `isyflask_cli-0.1.7/isyflask_cli/src/project/project.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.6/isyflask_cli/src/utils/folders.py` & `isyflask_cli-0.1.7/isyflask_cli/src/utils/folders.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.6/isyflask_cli/src/utils/strings.py` & `isyflask_cli-0.1.7/isyflask_cli/src/utils/strings.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.6/isyflask_cli/src/utils/template_gen.py` & `isyflask_cli-0.1.7/isyflask_cli/src/utils/template_gen.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.6/PKG-INFO` & `isyflask_cli-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: isyflask-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: Un cli para manejar proyectos de API con flask
+Home-page: https://github.com/DavidCuy/easyflask-cli
 Author: David Cuy
 Author-email: david.cuy.sanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: Documentation, https://github.com/DavidCuy/easyflask-cli
+Project-URL: Repository, https://github.com/DavidCuy/easyflask-cli
 Description-Content-Type: text/markdown
 
 # isyflask-cli
 
 Un cli para manejar proyectos de API con flask.
 
 > Se recomienda la instalación de docker para tener las últimas mejoras y actualizaciones. Algunas características sólo están con docker
@@ -31,24 +34,30 @@
 
 Para _macOS_ o _linux_:
 ````commandline
 python -m venv venv
 source ./venv/Scripts/activate
 ````
 
-Posteriormente instale el cli
+## Instalacion
+Para instalar el CLI ejecute el siguiente comando
+
+```
+python -m pip install --upgrade pip
+```
 
 ````commandline
 pip install isyflask-cli
 ````
 
 Para iniciar un proyecto ejecute el siguiente comando y responda las preguntas que salgan en el prompt:
 
 ````commandline
 isyflask-cli project init
+cd <folder project name>
 pip install -r requirements.txt
 ````
 
 Cambie el directorio al generado en el paso anterior. Utilizando *Docker*, el proyecto se levanta utilizando el siguiente comando:
 
 ````commandline
 docker-compose up
```

