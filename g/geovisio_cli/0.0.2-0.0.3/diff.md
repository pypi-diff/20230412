# Comparing `tmp/geovisio_cli-0.0.2.tar.gz` & `tmp/geovisio_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.0.2.tar", last modified: Fri Apr  7 08:41:33 2023, max compression
+gzip compressed data, was "geovisio_cli-0.0.3.tar", last modified: Wed Apr 12 20:09:04 2023, max compression
```

## Comparing `geovisio_cli-0.0.2.tar` & `geovisio_cli-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       47 2023-03-16 08:30:13.568567 geovisio_cli-0.0.2/.gitignore
--rw-r--r--   0        0        0     1732 2023-03-16 08:40:11.895987 geovisio_cli-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      773 2023-04-07 08:22:05.974833 geovisio_cli-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-04-02 21:10:50.265060 geovisio_cli-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-10 13:13:14.819914 geovisio_cli-0.0.2/LICENSE
--rw-r--r--   0        0        0      551 2023-03-14 15:06:36.234347 geovisio_cli-0.0.2/Makefile
--rw-r--r--   0        0        0     4639 2023-04-07 08:20:10.192636 geovisio_cli-0.0.2/README.md
--rw-r--r--   0        0        0     2181 2023-04-07 08:20:10.192636 geovisio_cli-0.0.2/USAGE.md
--rw-r--r--   0        0        0       53 2023-04-07 08:20:45.913314 geovisio_cli-0.0.2/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     1572 2023-04-06 12:23:20.847931 geovisio_cli-0.0.2/geovisio_cli/auth.py
--rw-r--r--   0        0        0       90 2023-03-10 13:13:14.819914 geovisio_cli-0.0.2/geovisio_cli/exception.py
--rw-r--r--   0        0        0     3446 2023-04-07 08:20:10.192636 geovisio_cli-0.0.2/geovisio_cli/main.py
--rw-r--r--   0        0        0      173 2023-03-14 15:06:36.234347 geovisio_cli-0.0.2/geovisio_cli/model.py
--rw-r--r--   0        0        0    12827 2023-04-07 08:20:10.192636 geovisio_cli-0.0.2/geovisio_cli/sequence.py
--rw-r--r--   0        0        0      896 2023-03-14 15:53:57.628418 geovisio_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 13:13:14.819914 geovisio_cli-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-03-10 13:13:14.819914 geovisio_cli-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-10 13:13:14.823914 geovisio_cli-0.0.2/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-10 13:13:14.827914 geovisio_cli-0.0.2/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-10 13:13:14.827914 geovisio_cli-0.0.2/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-10 13:13:14.827914 geovisio_cli-0.0.2/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-10 13:13:14.827914 geovisio_cli-0.0.2/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-10 13:13:14.827914 geovisio_cli-0.0.2/tests/integration/__init__.py
--rw-r--r--   0        0        0      865 2023-03-14 15:06:36.234347 geovisio_cli-0.0.2/tests/integration/conftest.py
--rw-r--r--   0        0        0      671 2023-03-14 15:53:57.628418 geovisio_cli-0.0.2/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      319 2023-04-07 08:20:10.192636 geovisio_cli-0.0.2/tests/integration/test_status.py
--rw-r--r--   0        0        0     3042 2023-04-07 08:20:10.192636 geovisio_cli-0.0.2/tests/integration/test_upload.py
--rw-r--r--   0        0        0      528 2023-04-02 21:10:50.265060 geovisio_cli-0.0.2/tests/test_process.py
--rw-r--r--   0        0        0      813 2023-04-02 21:10:50.265060 geovisio_cli-0.0.2/tests/test_sequence.py
--rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 geovisio_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1048 2023-04-12 20:00:20.693628 geovisio_cli-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/LICENSE
+-rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/Makefile
+-rw-r--r--   0        0        0     4639 2023-04-07 07:41:38.712978 geovisio_cli-0.0.3/README.md
+-rw-r--r--   0        0        0     2290 2023-04-11 15:14:50.737428 geovisio_cli-0.0.3/USAGE.md
+-rw-r--r--   0        0        0       53 2023-04-12 20:00:20.693628 geovisio_cli-0.0.3/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     1572 2023-03-14 16:32:00.535627 geovisio_cli-0.0.3/geovisio_cli/auth.py
+-rw-r--r--   0        0        0       90 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     3617 2023-04-11 15:19:40.311478 geovisio_cli-0.0.3/geovisio_cli/main.py
+-rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/geovisio_cli/model.py
+-rw-r--r--   0        0        0    13024 2023-04-11 15:19:40.311478 geovisio_cli-0.0.3/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0      896 2023-03-14 16:32:00.535627 geovisio_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0      671 2023-03-14 16:32:00.535627 geovisio_cli-0.0.3/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      319 2023-04-07 07:41:38.712978 geovisio_cli-0.0.3/tests/integration/test_status.py
+-rw-r--r--   0        0        0     3042 2023-04-07 07:41:38.712978 geovisio_cli-0.0.3/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      528 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/tests/test_process.py
+-rw-r--r--   0        0        0      813 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/tests/test_sequence.py
+-rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 geovisio_cli-0.0.3/PKG-INFO
```

### Comparing `geovisio_cli-0.0.2/.gitlab-ci.yml` & `geovisio_cli-0.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/CHANGELOG.md` & `geovisio_cli-0.0.3/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.0.3] - 2023-04-12
+
+### Added
+- A new `--is-blurred` flag is available on upload command to inform API that it doesn't need to blur pictures
+
+
 ## [0.0.2] - 2023-04-07
 
 ### Fixed
 - Pictures were not sorted in alphabetical or numeric order
 - Add a `--wait` flag to the upload command to wait for geovisio to have processed all pictures
 - Add a `geovisio collection-status` command, to get the status of a collection
 
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.0.1...develop
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...main
+[0.0.3]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...0.0.3
+[0.0.2]: https://gitlab.com/geovisio/cli/-/compare/0.0.1...0.0.2
 [0.0.1]: https://gitlab.com/PanierAvide/geovisio/-/commits/0.0.1
```

### Comparing `geovisio_cli-0.0.2/CODE_OF_CONDUCT.md` & `geovisio_cli-0.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/LICENSE` & `geovisio_cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/Makefile` & `geovisio_cli-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/README.md` & `geovisio_cli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/USAGE.md` & `geovisio_cli-0.0.3/USAGE.md`

 * *Files 5% similar despite different names*

```diff
@@ -71,9 +71,10 @@
 * `--path PATH`: Local path to your sequence folder  [required]
 * `--api-url TEXT`: GeoVisio endpoint URL  [required]
 * `--user TEXT`: GeoVisio user name if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the username will be asked during run.  [env var: GEOVISIO_USER]
 * `--password TEXT`: GeoVisio password if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the password will be asked during run.
 Note: is is advised to wait for prompt without using this variable.  [env var: GEOVISIO_PASSWORD]
-* `--wait / --no-wait`: wait for all pictures to be ready  [default: no-wait]
+* `--wait / --no-wait`: Wait for all pictures to be ready  [default: no-wait]
+* `--is-blurred / --is-not-blurred`: Define if sequence is already blurred or not  [default: is-not-blurred]
 * `--help`: Show this message and exit.
```

### Comparing `geovisio_cli-0.0.2/geovisio_cli/auth.py` & `geovisio_cli-0.0.3/geovisio_cli/auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/geovisio_cli/main.py` & `geovisio_cli-0.0.3/geovisio_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,26 @@
         default=None,
         help="""GeoVisio password if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the password will be asked during run.
 Note: is is advised to wait for prompt without using this variable.
 """,
         envvar="GEOVISIO_PASSWORD",
     ),
-    wait: bool = typer.Option(default=False, help="wait for all pictures to be ready"),
+    wait: bool = typer.Option(default=False, help="Wait for all pictures to be ready"),
+    isBlurred: bool = typer.Option(
+        False,
+        "--is-blurred/--is-not-blurred",
+        help="Define if sequence is already blurred or not",
+    ),
 ):
     """Processes and sends a given sequence on your GeoVisio API"""
 
     geovisio = model.Geovisio(url=api_url, user=user, password=password)
     try:
-        sequence.upload(path, geovisio, wait)
+        sequence.upload(path, geovisio, wait, isBlurred)
     except exception.CliException as e:
         print(
             Panel(
                 f"{e}",
                 title="[red]Error while importing collection",
                 border_style="red",
             )
```

### Comparing `geovisio_cli-0.0.2/geovisio_cli/sequence.py` & `geovisio_cli-0.0.3/geovisio_cli/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,25 +98,27 @@
 
 def process(path: Path) -> SequenceToUpload:
     sequence = _read_sequence(path)
     _check_sequence(sequence)
     return sequence
 
 
-def upload(path: Path, geovisio: Geovisio, wait: bool = False) -> UploadReport:
+def upload(
+    path: Path, geovisio: Geovisio, wait: bool = False, alreadyBlurred: bool = False
+) -> UploadReport:
     # early test that the given url is correct
     _test_geovisio_url(geovisio.url)
 
     sequence = process(path)
 
-    return _publish(sequence, geovisio, wait)
+    return _publish(sequence, geovisio, wait, alreadyBlurred)
 
 
 def _publish(
-    sequence: SequenceToUpload, geovisio: Geovisio, wait: bool
+    sequence: SequenceToUpload, geovisio: Geovisio, wait: bool, alreadyBlurred: bool
 ) -> UploadReport:
     print(f'📂 Publishing "{sequence.title}"')
 
     data = {}
     if sequence.title:
         data["title"] = sequence.title
 
@@ -164,15 +166,18 @@
                 uploading_progress.advance(uploading_task)
                 current_pic_progress.update(
                     current_pic_task, file=p.path.split("/")[-1]
                 )
                 picture_response = s.post(
                     f"{seq_location}/items",
                     files={"picture": open(p.path, "rb")},
-                    data={"position": i},
+                    data={
+                        "position": i,
+                        "isBlurred": "true" if alreadyBlurred else "false",
+                    },
                 )
                 if picture_response.status_code >= 400:
                     body = (
                         picture_response.json()
                         if picture_response.headers.get("Content-Type")
                         == "application/json"
                         else picture_response.text
```

### Comparing `geovisio_cli-0.0.2/pyproject.toml` & `geovisio_cli-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/fixtures/e1.jpg` & `geovisio_cli-0.0.3/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/fixtures/e2.jpg` & `geovisio_cli-0.0.3/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/fixtures/e3.jpg` & `geovisio_cli-0.0.3/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/integration/conftest.py` & `geovisio_cli-0.0.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.0.3/tests/integration/docker-compose-geovisio.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/integration/test_upload.py` & `geovisio_cli-0.0.3/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/test_process.py` & `geovisio_cli-0.0.3/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/tests/test_sequence.py` & `geovisio_cli-0.0.3/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.2/PKG-INFO` & `geovisio_cli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
 Requires-Dist: typer ~= 0.7.0
 Requires-Dist: rich[all] ~= 13.3.0
```

