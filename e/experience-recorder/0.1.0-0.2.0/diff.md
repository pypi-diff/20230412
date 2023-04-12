# Comparing `tmp/experience_recorder-0.1.0.tar.gz` & `tmp/experience_recorder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experience_recorder-0.1.0.tar", max compression
+gzip compressed data, was "experience_recorder-0.2.0.tar", max compression
```

## Comparing `experience_recorder-0.1.0.tar` & `experience_recorder-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,12 @@
--rw-r--r--   0        0        0        0 2023-03-13 12:09:49.328112 experience_recorder-0.1.0/experience_recorder/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 12:09:49.328112 experience_recorder-0.1.0/experience_recorder/maths/__init__.py
--rw-r--r--   0        0        0      244 2023-03-13 12:09:49.328112 experience_recorder-0.1.0/experience_recorder/maths/functions.py
--rw-r--r--   0        0        0      683 2023-03-13 12:09:49.328112 experience_recorder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 experience_recorder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/configuration/__init__.py
+-rw-r--r--   0        0        0     8031 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/configuration/configuration.py
+-rw-r--r--   0        0        0      604 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/main.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/perceptions/__init__.py
+-rw-r--r--   0        0        0     2443 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/perceptions/perceptions.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/recorder/__init__.py
+-rw-r--r--   0        0        0     5157 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/recorder/recorder.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/senses/__init__.py
+-rw-r--r--   0        0        0     1440 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/experience_recorder/senses/senses.py
+-rw-r--r--   0        0        0      876 2023-04-12 14:36:40.138680 experience_recorder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 experience_recorder-0.2.0/PKG-INFO
```

### Comparing `experience_recorder-0.1.0/pyproject.toml` & `experience_recorder-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 [tool.poetry]
 name = "experience_recorder"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["frapercan <frapercan1@alum.us.es>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 docopt = "^0.6.2"
+pyautogui = "^0.9.53"
+pynput = "^1.7.6"
+pyyaml = "^6.0"
+pillow = "^9.4.0"
+paddleocr = "^2.6.1.3"
+paddlepaddle = "^2.4.2"
+opencv-python = "4.5.5.64"
+numpy = "^1.24.2"
 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 coverage = {extras = ["toml"], version = "^7.2.1"}
 flake8 = "^6.0.0"
 flake8-bugbear = "^23.2.13"
 taskipy = "^1.10.3"
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
+pytest-catchlog = "^1.2.2"
+
 
 
 
-[tool.poetry.group.dev.dependencies]
-sphinx = "^6.1.3"
-sphinx-rtd-theme = "^1.2.0"
 
 [tool.coverage.run]
-omit = ["*/site-packages/*"]
+omit = ["*/site-packages/*","experience_recorder/main.py"]
 
 [tool.coverage.report]
 fail_under = 100
 
 [tool.taskipy.tasks]
 html_docs = "make html -C docs"
```

