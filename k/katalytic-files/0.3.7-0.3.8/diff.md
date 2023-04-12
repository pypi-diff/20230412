# Comparing `tmp/katalytic-files-0.3.7.tar.gz` & `tmp/katalytic-files-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.3.7.tar", last modified: Wed Apr 12 15:24:17 2023, max compression
+gzip compressed data, was "katalytic-files-0.3.8.tar", last modified: Wed Apr 12 17:54:56 2023, max compression
```

## Comparing `katalytic-files-0.3.7.tar` & `katalytic-files-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0       87 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.gitignore
--rw-r--r--   0        0        0      841 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.gitlab-ci.yml
--rw-r--r--   0        0        0      367 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.travis.yml
--rw-r--r--   0        0        0      197 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/LICENSE.txt
--rw-r--r--   0        0        0     1905 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/README.md
--rw-r--r--   0        0        0     1608 2023-04-12 15:24:16.396681 katalytic-files-0.3.7/pyproject.toml
--rw-r--r--   0        0        0       14 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/requirements.txt
--rw-r--r--   0        0        0      123 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/build.sh
--rw-r--r--   0        0        0     1460 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/build_check_release.sh
--rw-r--r--   0        0        0      234 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/cleanup.sh
--rw-r--r--   0        0        0     1270 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/pytest.sh
--rw-r--r--   0        0        0     6428 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/release.py
--rw-r--r--   0        0        0      403 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/setup.sh
--rw-r--r--   0        0        0     1707 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/venv.sh
--rw-r--r--   0        0        0    11060 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/src/katalytic/files.py
--rw-r--r--   0        0        0    39566 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/tests/test_files.py
--rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.gitlab-ci.yml
+-rw-r--r--   0        0        0      376 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.travis.yml
+-rw-r--r--   0        0        0      349 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/LICENSE.txt
+-rw-r--r--   0        0        0     1905 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/README.md
+-rw-r--r--   0        0        0     1609 2023-04-12 17:54:50.784596 katalytic-files-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/requirements.txt
+-rw-r--r--   0        0        0      234 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1270 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/pytest.sh
+-rw-r--r--   0        0        0     2209 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/release.sh
+-rw-r--r--   0        0        0      403 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/setup.sh
+-rw-r--r--   0        0        0     1707 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/venv.sh
+-rw-r--r--   0        0        0    11060 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/src/katalytic/files.py
+-rw-r--r--   0        0        0    39566 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/tests/test_files.py
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.8/PKG-INFO
```

### Comparing `katalytic-files-0.3.7/.gitignore` & `katalytic-files-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/.gitlab-ci.yml` & `katalytic-files-0.3.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/LICENSE.txt` & `katalytic-files-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/README.md` & `katalytic-files-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/pyproject.toml` & `katalytic-files-0.3.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.3.7"
+version = "0.3.8"
+
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-files-0.3.7/scripts/build_check_release.sh` & `katalytic-files-0.3.8/scripts/release.sh`

 * *Files 20% similar despite different names*

```diff
@@ -17,33 +17,59 @@
 	command rm -rf **/*.egg-info
 	command rm -rf **/__pycache__
 	command rm -rf **/.pytest_cache
 	command rm -rf **/venv
 
 	python -m venv venv
 	source venv/bin/activate
+	python -m pip install --quiet --quiet twine flit packaging
+	python -m pip install --quiet --quiet python-semantic-release==7.29.0
+}
+
+check_build(){
+	pkg="$1"
+	twine check dist/*
+	if [ $? -eq 0 ]; then
+		echo "[twine] ok"
+	else
+		echo "[twine] Check failed. Exiting."
+		exit 1
+	fi
+
+	python -m pip install --quiet --quiet dist/katalytic-files*.tar.gz
+	python -c "from $pkg import __version__; print(__version__)"
+	if [ $? -eq 0 ]; then
+		echo "[sdist] ok"
+	else
+		echo "[sdist] Import failed. Exiting."
+		exit 1
+	fi
+
+	python -m pip install --quiet --quiet dist/katalytic_files-*-py3-none-any.whl
+	python -c "from $pkg import __version__; print(__version__)"
+	if [ $? -eq 0 ]; then
+		echo "[wheel] ok"
+	else
+		echo "[wheel] Import failed. Exiting."
+		exit 1
+	fi
 }
 
+
 create_pypirc(){
-	  message=$(echo "
+	message=$(echo "
 [distutils]
 index-servers =
   pypi
 
 [pypi]
 repository = https://upload.pypi.org/legacy/
 username = __token__
 password = $TWINE_PASSWORD
-
-
-[gitlab]
-repository = https://gitlab.com/api/v4/projects/<project-id>/packages/pypi/
-username = gitlab-ci-token
-password =
-" | sed -e 's/^[[:blank:]]{4}//' -e 's/[[:blank:]]*$//')
+" )
 
 	echo "$message" > ~/.pypirc
 	chmod 666 ~/.pypirc
 }
 
 main(){
 	current_version=$(grep -P 'version = (.*)' pyproject.toml | grep -Po '[.0-9]+')
@@ -51,27 +77,28 @@
 	echo "Package: '$pkg'"
 	echo "Current: '$current_version'"
 	echo ""
 
 	rm -rf **/dist
 	rm -rf **/build
 	create_pypirc
-
 	create_env
-	python -m pip install --quiet --quiet twine flit packaging
-	pip install --quiet --quiet python-semantic-release==7.29.0
 
 	# bump -> build -> check
 	semantic-release version
-	flit build
-	twine check dist/*
 	if [ $? -ne 0 ]; then
-		echo "twine check failed, exiting."
-		exit 1
+		# this executes when none of the commits are prefixed with "fix" or "feat"
+		# or when something really bad happened
+		echo "No version bump. Exiting."
+		exit 0
 	fi
 
+	flit build
+	check_build "$pkg"
+
 	# release -> push
 	flit publish --repository pypi
-	git push --tags
+	git config credential.helper '!f() { printf "%s\n" "username=vali19th" "password=$GITLAB_TOKEN"; };f'
+	git push --tags https://gitlab.com/katalytic/katalytic-files.git HEAD:refs/heads/main
 }
 
 main
```

### Comparing `katalytic-files-0.3.7/scripts/conda.sh` & `katalytic-files-0.3.8/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/scripts/find_requirements.py` & `katalytic-files-0.3.8/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/scripts/venv.sh` & `katalytic-files-0.3.8/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/src/katalytic/files.py` & `katalytic-files-0.3.8/src/katalytic/files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/tests/test_files.py` & `katalytic-files-0.3.8/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.7/PKG-INFO` & `katalytic-files-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.3.7
+Version: 0.3.8
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

