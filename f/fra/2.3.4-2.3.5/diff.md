# Comparing `tmp/fra-2.3.4.tar.gz` & `tmp/fra-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fra-2.3.4.tar", max compression
+gzip compressed data, was "fra-2.3.5.tar", max compression
```

## Comparing `fra-2.3.4.tar` & `fra-2.3.5.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0     1070 2022-11-12 00:43:51.998589 fra-2.3.4/LICENSE
--rw-r--r--   0        0        0     1231 2022-11-21 17:06:17.513278 fra-2.3.4/README.md
--rw-r--r--   0        0        0    85510 2022-11-18 23:58:25.892655 fra-2.3.4/docs/architecture_1.png
--rw-r--r--   0        0        0       41 2022-11-10 21:46:38.135925 fra-2.3.4/migrations/README
--rw-r--r--   0        0        0      857 2022-11-10 21:46:38.140126 fra-2.3.4/migrations/alembic.ini
--rw-r--r--   0        0        0     2745 2022-11-10 22:30:31.183059 fra-2.3.4/migrations/env.py
--rw-r--r--   0        0        0      494 2022-11-10 21:46:38.134009 fra-2.3.4/migrations/script.py.mako
--rw-r--r--   0        0        0     1056 2022-11-21 17:05:52.825375 fra-2.3.4/migrations/versions/222c027bbdec_file_type.py
--rw-r--r--   0        0        0     1239 2022-11-19 00:02:12.323262 fra-2.3.4/migrations/versions/55161145af8f_add_user_recommendations_model.py
--rw-r--r--   0        0        0      937 2022-11-14 22:14:52.600247 fra-2.3.4/migrations/versions/5c34861d9ef9_add_file_to_organization.py
--rw-r--r--   0        0        0     2337 2022-11-12 00:14:27.492884 fra-2.3.4/migrations/versions/78c25d669d9c_first_models.py
--rw-r--r--   0        0        0      956 2022-11-14 22:14:52.600410 fra-2.3.4/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py
--rw-r--r--   0        0        0      757 2022-11-21 17:05:52.833588 fra-2.3.4/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py
--rw-r--r--   0        0        0     1463 2022-11-14 22:14:52.600540 fra-2.3.4/migrations/versions/ff9e18b937bd_.py
--rw-r--r--   0        0        0        0 2022-10-06 23:09:09.223193 fra-2.3.4/motor/__init__.py
--rw-r--r--   0        0        0      237 2022-11-19 00:02:09.843162 fra-2.3.4/motor/adaptors.py
--rw-r--r--   0        0        0     2963 2022-11-21 16:53:19.316907 fra-2.3.4/motor/models.py
--rw-r--r--   0        0        0     5842 2022-11-21 16:59:57.463309 fra-2.3.4/motor/processor.py
--rw-r--r--   0        0        0      376 2022-11-19 00:02:12.326690 fra-2.3.4/motor/tasks.py
--rw-r--r--   0        0        0        0 2022-11-14 20:48:04.103287 fra-2.3.4/organizations/__init__.py
--rw-r--r--   0        0        0      447 2022-11-14 22:14:52.600991 fra-2.3.4/organizations/models.py
--rw-r--r--   0        0        0      776 2022-12-07 19:39:21.851287 fra-2.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-06 23:09:18.030273 fra-2.3.4/server/__init__.py
--rw-r--r--   0        0        0        0 2022-10-12 23:20:39.494785 fra-2.3.4/server/api/__init__.py
--rw-r--r--   0        0        0        0 2022-10-12 23:21:40.343737 fra-2.3.4/server/api/handlers/__init__.py
--rw-r--r--   0        0        0     2207 2022-11-30 23:32:56.293201 fra-2.3.4/server/api/handlers/file_loader.py
--rw-r--r--   0        0        0     1919 2022-11-30 21:58:21.493383 fra-2.3.4/server/api/handlers/organizations.py
--rw-r--r--   0        0        0      813 2022-11-30 21:58:20.525095 fra-2.3.4/server/api/handlers/recommendations.py
--rw-r--r--   0        0        0      632 2022-11-14 22:15:38.953822 fra-2.3.4/server/api/handlers/register_all_handlers.py
--rw-r--r--   0        0        0     2404 2022-11-30 21:59:26.031298 fra-2.3.4/server/api/handlers/user_ratings.py
--rw-r--r--   0        0        0     1237 2022-11-19 00:02:12.323030 fra-2.3.4/server/app.py
--rw-r--r--   0        0        0     1226 2022-12-07 19:39:21.860702 fra-2.3.4/server/config.py
--rw-r--r--   0        0        0      118 2022-11-10 21:37:50.712435 fra-2.3.4/server/database.py
--rw-r--r--   0        0        0      464 2022-12-07 19:39:21.867977 fra-2.3.4/server/rebar.py
--rw-r--r--   0        0        0        0 2022-10-12 23:22:14.683713 fra-2.3.4/server/schemas/__init__.py
--rw-r--r--   0        0        0      445 2022-11-21 15:11:29.984871 fra-2.3.4/server/schemas/file_data.py
--rw-r--r--   0        0        0      276 2022-11-12 00:14:26.099390 fra-2.3.4/server/schemas/general.py
--rw-r--r--   0        0        0      731 2022-11-14 22:14:52.602088 fra-2.3.4/server/schemas/organization.py
--rw-r--r--   0        0        0      950 2022-11-14 21:05:59.496515 fra-2.3.4/server/schemas/user_ratings.py
--rw-r--r--   0        0        0     2213 2022-12-07 19:40:28.628548 fra-2.3.4/setup.py
--rw-r--r--   0        0        0     1976 2022-12-07 19:40:28.628891 fra-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-15 23:08:27.832029 fra-2.3.5/LICENSE
+-rw-r--r--   0        0        0     1446 2023-04-12 00:25:23.546185 fra-2.3.5/README.md
+-rw-r--r--   0        0        0    85510 2023-03-15 23:08:27.836029 fra-2.3.5/docs/architecture_1.png
+-rw-r--r--   0        0        0       41 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/README
+-rw-r--r--   0        0        0      857 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/alembic.ini
+-rw-r--r--   0        0        0     2745 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/script.py.mako
+-rw-r--r--   0        0        0     1056 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/222c027bbdec_file_type.py
+-rw-r--r--   0        0        0     1239 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/55161145af8f_add_user_recommendations_model.py
+-rw-r--r--   0        0        0      937 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/5c34861d9ef9_add_file_to_organization.py
+-rw-r--r--   0        0        0     2337 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/78c25d669d9c_first_models.py
+-rw-r--r--   0        0        0      956 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py
+-rw-r--r--   0        0        0      757 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py
+-rw-r--r--   0        0        0     1463 2023-03-15 23:08:30.335994 fra-2.3.5/migrations/versions/ff9e18b937bd_.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/motor/__init__.py
+-rw-r--r--   0        0        0      237 2023-03-15 23:08:30.335994 fra-2.3.5/motor/adaptors.py
+-rw-r--r--   0        0        0     2963 2023-03-15 23:08:30.335994 fra-2.3.5/motor/models.py
+-rw-r--r--   0        0        0     5842 2023-03-15 23:08:30.335994 fra-2.3.5/motor/processor.py
+-rw-r--r--   0        0        0      376 2023-03-15 23:08:30.335994 fra-2.3.5/motor/tasks.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/organizations/__init__.py
+-rw-r--r--   0        0        0      447 2023-03-15 23:08:30.335994 fra-2.3.5/organizations/models.py
+-rw-r--r--   0        0        0      804 2023-04-12 00:22:24.590617 fra-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/__init__.py
+-rw-r--r--   0        0        0     2207 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/file_loader.py
+-rw-r--r--   0        0        0     1919 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/organizations.py
+-rw-r--r--   0        0        0      813 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/recommendations.py
+-rw-r--r--   0        0        0      632 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/register_all_handlers.py
+-rw-r--r--   0        0        0     2404 2023-03-15 23:08:30.335994 fra-2.3.5/server/api/handlers/user_ratings.py
+-rw-r--r--   0        0        0     1237 2023-03-15 23:08:30.335994 fra-2.3.5/server/app.py
+-rw-r--r--   0        0        0     1226 2023-03-15 23:08:30.335994 fra-2.3.5/server/config.py
+-rw-r--r--   0        0        0      118 2023-03-15 23:08:30.335994 fra-2.3.5/server/database.py
+-rw-r--r--   0        0        0      464 2023-04-12 00:22:34.571618 fra-2.3.5/server/rebar.py
+-rw-r--r--   0        0        0        0 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/__init__.py
+-rw-r--r--   0        0        0      445 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/file_data.py
+-rw-r--r--   0        0        0      276 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/general.py
+-rw-r--r--   0        0        0      731 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/organization.py
+-rw-r--r--   0        0        0      950 2023-03-15 23:08:30.335994 fra-2.3.5/server/schemas/user_ratings.py
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 fra-2.3.5/PKG-INFO
```

### Comparing `fra-2.3.4/LICENSE` & `fra-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/README.md` & `fra-2.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ## Requirements
 * pyenv (optional but recommended)
 * poetry
 * python 3.9+
 * postgres
 * redis
+* docker (optional)
 
 ## Installation
 * create a virtualenv
     >pyenv virtualenv 3.9.15 fra
     >pyenv activate fra
 * create a database and update the config.py file with the name and host
     >psql; create database fra; \q
@@ -33,14 +34,21 @@
     > flask --app server/app run
 
 -- For async jobs that process recommendations
 
     > celery -A motor.tasks worker  --loglevel=info  
 
 
+## Running the app with docker
+
+- Run the docker-compose
+   > docker-compose up
+
+That command will start all the services and the web server can be accessed via browser on http://localhost:5000
+
 OpenAPI docs will be online on YOURDOMAIN/api/swagger/ui
 
 Follow this order to be able to get recommendations:
 1. create an organization
 2. add users to the organization
 3. add the files with the data (some examples on example_data folder)
 4. add file mapping
```

### Comparing `fra-2.3.4/docs/architecture_1.png` & `fra-2.3.5/docs/architecture_1.png`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/alembic.ini` & `fra-2.3.5/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/env.py` & `fra-2.3.5/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/versions/222c027bbdec_file_type.py` & `fra-2.3.5/migrations/versions/222c027bbdec_file_type.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/versions/55161145af8f_add_user_recommendations_model.py` & `fra-2.3.5/migrations/versions/55161145af8f_add_user_recommendations_model.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/versions/5c34861d9ef9_add_file_to_organization.py` & `fra-2.3.5/migrations/versions/5c34861d9ef9_add_file_to_organization.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/versions/78c25d669d9c_first_models.py` & `fra-2.3.5/migrations/versions/78c25d669d9c_first_models.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py` & `fra-2.3.5/migrations/versions/9cce5410d6c2_add_user_rating_to_organization.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py` & `fra-2.3.5/migrations/versions/ea52bc400e9b_remove_blob_file_from_db.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/migrations/versions/ff9e18b937bd_.py` & `fra-2.3.5/migrations/versions/ff9e18b937bd_.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/motor/models.py` & `fra-2.3.5/motor/models.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/motor/processor.py` & `fra-2.3.5/motor/processor.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/pyproject.toml` & `fra-2.3.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fra"
-version = "2.3.4"
+version = "2.3.5"
 description = "Simple Recommendation System, content based."
 authors = ["Eliecer Daza"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/elin3t/fra"
 packages = [
     { include = "server"},
@@ -18,18 +18,19 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.5.0"
 flask-rebar = "^2.2.1"
 Flask-Migrate = "^3.1.0"
-psycopg2 = "^2.9.5"
 redis = "^4.3.4"
 celery = "^5.2.7"
 Flask-CeleryExt = "^0.4.3"
+psycopg2-binary = "^2.9.5"
+gunicorn = "^20.1.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20.0"
 black = "^22.10.0"
 flake8 = "^5.0.4"
 mypy = "^0.982"
```

### Comparing `fra-2.3.4/server/api/handlers/file_loader.py` & `fra-2.3.5/server/api/handlers/file_loader.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/api/handlers/organizations.py` & `fra-2.3.5/server/api/handlers/organizations.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/api/handlers/recommendations.py` & `fra-2.3.5/server/api/handlers/recommendations.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/api/handlers/register_all_handlers.py` & `fra-2.3.5/server/api/handlers/register_all_handlers.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/api/handlers/user_ratings.py` & `fra-2.3.5/server/api/handlers/user_ratings.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/app.py` & `fra-2.3.5/server/app.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/config.py` & `fra-2.3.5/server/config.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/schemas/organization.py` & `fra-2.3.5/server/schemas/organization.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/server/schemas/user_ratings.py` & `fra-2.3.5/server/schemas/user_ratings.py`

 * *Files identical despite different names*

### Comparing `fra-2.3.4/PKG-INFO` & `fra-2.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: fra
-Version: 2.3.4
+Version: 2.3.5
 Summary: Simple Recommendation System, content based.
 Home-page: https://gitlab.com/elin3t/fra
 License: MIT
 Author: Eliecer Daza
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask-CeleryExt (>=0.4.3,<0.5.0)
 Requires-Dist: Flask-Migrate (>=3.1.0,<4.0.0)
 Requires-Dist: celery (>=5.2.7,<6.0.0)
 Requires-Dist: flask-rebar (>=2.2.1,<3.0.0)
+Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
-Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: redis (>=4.3.4,<5.0.0)
 Project-URL: Repository, https://gitlab.com/elin3t/fra
 Description-Content-Type: text/markdown
 
 # FRA
 Fra is a Recommendation based framework. It was created with the idea of have an option for creating content-based recommendations easily via API.
 
@@ -29,14 +32,15 @@
 
 ## Requirements
 * pyenv (optional but recommended)
 * poetry
 * python 3.9+
 * postgres
 * redis
+* docker (optional)
 
 ## Installation
 * create a virtualenv
     >pyenv virtualenv 3.9.15 fra
     >pyenv activate fra
 * create a database and update the config.py file with the name and host
     >psql; create database fra; \q
@@ -54,14 +58,21 @@
     > flask --app server/app run
 
 -- For async jobs that process recommendations
 
     > celery -A motor.tasks worker  --loglevel=info  
 
 
+## Running the app with docker
+
+- Run the docker-compose
+   > docker-compose up
+
+That command will start all the services and the web server can be accessed via browser on http://localhost:5000
+
 OpenAPI docs will be online on YOURDOMAIN/api/swagger/ui
 
 Follow this order to be able to get recommendations:
 1. create an organization
 2. add users to the organization
 3. add the files with the data (some examples on example_data folder)
 4. add file mapping
```

