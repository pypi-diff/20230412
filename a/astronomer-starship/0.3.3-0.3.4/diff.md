# Comparing `tmp/astronomer-starship-0.3.3.tar.gz` & `tmp/astronomer-starship-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomer-starship-0.3.3.tar", last modified: Fri Mar 24 15:08:59 2023, max compression
+gzip compressed data, was "astronomer-starship-0.3.4.tar", last modified: Wed Apr 12 15:12:20 2023, max compression
```

## Comparing `astronomer-starship-0.3.3.tar` & `astronomer-starship-0.3.4.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.565908 astronomer-starship-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-24 15:08:59.565908 astronomer-starship-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/aeroscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/aeroscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/aeroscope/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/aeroscope/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/aeroscope/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.557907 astronomer-starship-0.3.3/aeroscope/plugins/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/aeroscope/plugins/templates/aeroscope/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/aeroscope/plugins/templates/aeroscope/formhelper.html
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/aeroscope/plugins/templates/aeroscope/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/aeroscope/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/astronomer_starship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-24 15:08:59.000000 astronomer-starship-0.3.3/astronomer_starship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-24 15:08:59.000000 astronomer-starship-0.3.3/astronomer_starship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 15:08:59.000000 astronomer-starship-0.3.3/astronomer_starship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-24 15:08:59.000000 astronomer-starship-0.3.3/astronomer_starship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-24 15:08:59.000000 astronomer-starship-0.3.3/astronomer_starship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 15:08:59.000000 astronomer-starship-0.3.3/astronomer_starship.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-24 15:08:59.565908 astronomer-starship-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/starship/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/starship/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/services/astrohub_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/services/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/starship/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.565908 astronomer-starship-0.3.3/starship/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/static/js/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/static/js/idiomorph.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/static/js/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    25717 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/static/js/tippy.js
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/static/tail-spin.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.561907 astronomer-starship-0.3.3/starship/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.565908 astronomer-starship-0.3.3/starship/templates/starship/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:08:59.565908 astronomer-starship-0.3.3/starship/templates/starship/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/dag_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/env_checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/github_loop.html
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/migrate_connection_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/migrate_variable_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/target_deployment_select.html
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/test_connection_label.html
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/token_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/components/user_label.html
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/connections.html
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/dags.html
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/env.html
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/migration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-24 15:08:37.000000 astronomer-starship-0.3.3/starship/templates/starship/variables.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/aeroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/aeroscope/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.185887 astronomer-starship-0.3.4/aeroscope/plugins/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/formhelper.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/aeroscope/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/astronomer_starship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 15:12:20.000000 astronomer-starship-0.3.4/astronomer_starship.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/starship/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/starship/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/services/astrohub_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/services/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.189888 astronomer-starship-0.3.4/starship/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.193888 astronomer-starship-0.3.4/starship/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/htmx.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/idiomorph.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25717 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/js/tippy.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/static/tail-spin.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.185887 astronomer-starship-0.3.4/starship/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.193888 astronomer-starship-0.3.4/starship/templates/starship/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:12:20.197888 astronomer-starship-0.3.4/starship/templates/starship/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/dag_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/env_checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/github_loop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/migrate_connection_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/migrate_pool_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/migrate_variable_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/tabs_loading.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/target_deployment_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/target_deployment_select_loading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/test_connection_label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/token_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/components/user_label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/connections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/dags.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/env.html
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/migration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/pools.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 15:12:01.000000 astronomer-starship-0.3.4/starship/templates/starship/variables.html
```

### Comparing `astronomer-starship-0.3.3/PKG-INFO` & `astronomer-starship-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: astronomer-starship
-Version: 0.3.3
+Version: 0.3.4
 Summary: Migrations to Astro Cloud
 Home-page: UNKNOWN
 Author: ade@astronomer.io
 License: UNKNOWN
 Description: Astronomer Starship Plugin
         ==========================
         
@@ -66,16 +66,26 @@
         2. In the table displaying the variables that can be migrated, click the ``Migrate`` button for each connection that needs to be sent to the Target Deployment
         
         .. image:: https://github.com/astronomer/starship/raw/master/astronomer-starship/images/variables-migrate.png
            :width: 800
         
         3. Once the ``Migrate`` button is clicked, the variable will be sent to the Target Deployment and will show as ``Migrated ✅`` in the plugin UI:
         
-        .. image:: https://github.com/astronomer/starship/raw/master/astronomer-starship/images/variables-migrate-complete.png
-           :width: 800
+        
+        Migrating Airflow Pools
+        ---------------------------
+        
+        To migrate pools from your source Airflow meta-database:
+        
+        1. Click on the ``Pools`` tab:
+        2. In the table displaying the pools that can be migrated, click the ``Migrate`` button for each pool that needs to be sent to the Target Deployment
+        
+        .. image:: images/pools-migrate.png
+        
+        3. Once the ``Migrate`` button is clicked, the pool will be created in the Target Deployment and will show as ``Migrated ✅`` in the plugin UI:
         
         Migrating Environment Variables
         -------------------------------
         
         To migrate environment variables from your source Airflow:
         
         1. Click on the ``Environment Variables`` tab:
```

### Comparing `astronomer-starship-0.3.3/README.rst` & `astronomer-starship-0.3.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -59,16 +59,26 @@
 2. In the table displaying the variables that can be migrated, click the ``Migrate`` button for each connection that needs to be sent to the Target Deployment
 
 .. image:: https://github.com/astronomer/starship/raw/master/astronomer-starship/images/variables-migrate.png
    :width: 800
 
 3. Once the ``Migrate`` button is clicked, the variable will be sent to the Target Deployment and will show as ``Migrated ✅`` in the plugin UI:
 
-.. image:: https://github.com/astronomer/starship/raw/master/astronomer-starship/images/variables-migrate-complete.png
-   :width: 800
+
+Migrating Airflow Pools
+---------------------------
+
+To migrate pools from your source Airflow meta-database:
+
+1. Click on the ``Pools`` tab:
+2. In the table displaying the pools that can be migrated, click the ``Migrate`` button for each pool that needs to be sent to the Target Deployment
+
+.. image:: images/pools-migrate.png
+
+3. Once the ``Migrate`` button is clicked, the pool will be created in the Target Deployment and will show as ``Migrated ✅`` in the plugin UI:
 
 Migrating Environment Variables
 -------------------------------
 
 To migrate environment variables from your source Airflow:
 
 1. Click on the ``Environment Variables`` tab:
```

### Comparing `astronomer-starship-0.3.3/aeroscope/operators.py` & `astronomer-starship-0.3.4/aeroscope/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/aeroscope/plugins/__init__.py` & `astronomer-starship-0.3.4/aeroscope/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/aeroscope/plugins/templates/aeroscope/main.html` & `astronomer-starship-0.3.4/aeroscope/plugins/templates/aeroscope/main.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/aeroscope/util.py` & `astronomer-starship-0.3.4/aeroscope/util.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/astronomer_starship.egg-info/PKG-INFO` & `astronomer-starship-0.3.4/astronomer_starship.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: astronomer-starship
-Version: 0.3.3
+Version: 0.3.4
 Summary: Migrations to Astro Cloud
 Home-page: UNKNOWN
 Author: ade@astronomer.io
 License: UNKNOWN
 Description: Astronomer Starship Plugin
         ==========================
         
@@ -66,16 +66,26 @@
         2. In the table displaying the variables that can be migrated, click the ``Migrate`` button for each connection that needs to be sent to the Target Deployment
         
         .. image:: https://github.com/astronomer/starship/raw/master/astronomer-starship/images/variables-migrate.png
            :width: 800
         
         3. Once the ``Migrate`` button is clicked, the variable will be sent to the Target Deployment and will show as ``Migrated ✅`` in the plugin UI:
         
-        .. image:: https://github.com/astronomer/starship/raw/master/astronomer-starship/images/variables-migrate-complete.png
-           :width: 800
+        
+        Migrating Airflow Pools
+        ---------------------------
+        
+        To migrate pools from your source Airflow meta-database:
+        
+        1. Click on the ``Pools`` tab:
+        2. In the table displaying the pools that can be migrated, click the ``Migrate`` button for each pool that needs to be sent to the Target Deployment
+        
+        .. image:: images/pools-migrate.png
+        
+        3. Once the ``Migrate`` button is clicked, the pool will be created in the Target Deployment and will show as ``Migrated ✅`` in the plugin UI:
         
         Migrating Environment Variables
         -------------------------------
         
         To migrate environment variables from your source Airflow:
         
         1. Click on the ``Environment Variables`` tab:
```

### Comparing `astronomer-starship-0.3.3/astronomer_starship.egg-info/SOURCES.txt` & `astronomer-starship-0.3.4/astronomer_starship.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,22 @@
 starship/static/js/popper.js
 starship/static/js/tippy.js
 starship/templates/starship/connections.html
 starship/templates/starship/dags.html
 starship/templates/starship/env.html
 starship/templates/starship/main.html
 starship/templates/starship/migration.html
+starship/templates/starship/pools.html
 starship/templates/starship/variables.html
 starship/templates/starship/components/dag_row.html
 starship/templates/starship/components/env_checkbox.html
 starship/templates/starship/components/github_loop.html
 starship/templates/starship/components/migrate_connection_button.html
+starship/templates/starship/components/migrate_pool_button.html
 starship/templates/starship/components/migrate_variable_button.html
 starship/templates/starship/components/tabs.html
+starship/templates/starship/components/tabs_loading.html
 starship/templates/starship/components/target_deployment_select.html
+starship/templates/starship/components/target_deployment_select_loading.html
 starship/templates/starship/components/test_connection_label.html
 starship/templates/starship/components/token_modal.html
 starship/templates/starship/components/user_label.html
```

### Comparing `astronomer-starship-0.3.3/setup.cfg` & `astronomer-starship-0.3.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = astronomer-starship
-version = 0.3.3
+version = 0.3.4
 description = Migrations to Astro Cloud
 author = ade@astronomer.io
 long_description = file: README.rst
 
 [options]
 include_package_data = True
 python_requires = >=3.7, <4
 packages = find_namespace:
 install_requires = 
-	pydash
+	pydash<7
 	python-graphql-client
 	requests
 	cachetools
 	pygithub
 
 [options.entry_points]
 airflow.plugins =
```

### Comparing `astronomer-starship-0.3.3/starship/main.py` & `astronomer-starship-0.3.4/starship/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from urllib.parse import urlparse
 
 from cachetools.func import ttl_cache
 from airflow.plugins_manager import AirflowPlugin
 from airflow import models
 
 from airflow.www import auth
@@ -17,31 +18,30 @@
 
 import requests
 
 from pydash import at
 
 from python_graphql_client import GraphqlClient
 
-
 bp = Blueprint(
     "starship",
     __name__,
     template_folder="templates",
     static_folder="static",
     static_url_path="/static/starship",
 )
 
 
 class AstroMigration(AppBuilderBaseView):
     default_view = "main"
 
     def __init__(self):
         super().__init__()
-        self.local_client = LocalAirflowClient()
-        self.astro_client = AstroClient()
+        self.local_client: LocalAirflowClient = LocalAirflowClient()
+        self.astro_client: AstroClient = AstroClient()
 
     def get_astro_username(self, token):
         if not token:
             pass
 
         headers = {"Authorization": f"Bearer {token}"}
         client = GraphqlClient(
@@ -79,17 +79,18 @@
     def astro_deployments(self, token):
         if not token:
             return {}
 
         headers = {"Authorization": f"Bearer {token}"}
 
         orgs = self.astro_orgs(token)
+        short_name = os.getenv("STARSHIP_ORG_SHORTNAME", [_ for _ in orgs.values()][0]['shortName'])
 
         # FIXME use the first org for now. change to a select in the near term.
-        url = f"https://api.astronomer.io/v1alpha1/organizations/{[_ for _ in orgs.values()][0]['shortName']}/deployments"
+        url = f"https://api.astronomer.io/v1alpha1/organizations/{short_name}/deployments"
 
         try:
             api_rv = requests.get(url, headers=headers).json()["deployments"]
 
             return {deploy["id"]: deploy for deploy in (api_rv or [])}
         except Exception as exc:
             print(exc)
@@ -105,14 +106,21 @@
     def get_astro_variables(self, deployment_url: str, token: str):
         resp = requests.get(
             f"{deployment_url}/api/v1/variables",
             headers={"Authorization": f"Bearer {token}"},
         )
         return resp.json()["variables"]
 
+    def get_astro_pools(self, deployment_url: str, token: str):
+        resp = requests.get(
+            f"{deployment_url}/api/v1/pools",
+            headers={"Authorization": f"Bearer {token}"},
+        )
+        return resp.json()["pools"]
+
     @ttl_cache(ttl=1)
     def get_astro_connections(self, deployment_url: str, token: str):
         resp = requests.get(
             f"{deployment_url}/api/v1/connections",
             headers={"Authorization": f"Bearer {token}"},
         )
         return resp.json()["connections"]
@@ -178,14 +186,24 @@
         data = {
             "component": "variables",
             "vars": {var.key: var for var in self.local_client.get_variables()},
         }
 
         return self.render_template("starship/variables.html", data=data)
 
+    @expose("/tabs/pools")
+    @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_VARIABLE)])
+    def tabs_pools(self):
+        data = {
+            "component": "pools",
+            "pools": {pool.pool: pool for pool in self.local_client.get_pools()},
+        }
+
+        return self.render_template("starship/pools.html", data=data)
+
     @expose("/tabs/connections")
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONNECTION)])
     def tabs_conns(self):
         data = {
             "component": "connections",
             "conns": {
                 conn.conn_id: conn for conn in self.local_client.get_connections()
@@ -215,28 +233,29 @@
         deployment_url = self.get_deployment_url(deployment)
 
         if request.method == "POST":
             local_connections = {
                 conn.conn_id: conn for conn in self.local_client.get_connections()
             }
 
-            requests.post(
+            r = requests.post(
                 f"{deployment_url}/api/v1/connections",
                 headers={"Authorization": f"Bearer {session.get('token')}"},
                 json={
                     "connection_id": local_connections[conn_id].conn_id,
                     "conn_type": local_connections[conn_id].conn_type,
                     "host": local_connections[conn_id].host,
                     "login": local_connections[conn_id].login,
                     "schema": local_connections[conn_id].schema,
                     "port": local_connections[conn_id].port,
                     "password": local_connections[conn_id].password or "",
                     "extra": local_connections[conn_id].extra,
                 },
             )
+            r.raise_for_status()
 
         deployment_conns = self.get_astro_connections(
             deployment_url, session.get("token")
         )
 
         is_migrated = conn_id in [
             remote_conn["connection_id"] for remote_conn in deployment_conns
@@ -284,31 +303,62 @@
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_VARIABLE)])
     def button_migrate_variable(self, variable: str, deployment: str):
         deployment_url = self.get_deployment_url(deployment)
 
         if request.method == "POST":
             local_vars = {var.key: var for var in self.local_client.get_variables()}
 
-            requests.post(
+            r = requests.post(
                 f"{deployment_url}/api/v1/variables",
                 headers={"Authorization": f"Bearer {session.get('token')}"},
                 json={"key": variable, "value": local_vars[variable].val},
             )
+            r.raise_for_status()
 
         remote_vars = self.get_astro_variables(deployment_url, session.get("token"))
 
         is_migrated = variable in [remote_var["key"] for remote_var in remote_vars]
 
         return self.render_template(
             "starship/components/migrate_variable_button.html",
             variable=variable,
             deployment=deployment,
             is_migrated=is_migrated,
         )
 
+    @expose(
+        "/button/migrate/pool/<string:deployment>/<string:pool_name>",
+        methods=("GET", "POST"),
+    )
+    @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_VARIABLE)])
+    def button_migrate_pool(self, pool_name: str, deployment: str):
+        deployment_url = self.get_deployment_url(deployment)
+
+        if request.method == "POST":
+            pool = [p for p in self.local_client.get_pools() if p.pool == pool_name][0]
+
+            r = requests.post(
+                f"{deployment_url}/api/v1/pools",
+                headers={"Authorization": f"Bearer {session.get('token')}"},
+                json={"name": pool_name, "slots": pool.slots, "description": pool.description},
+            )
+            print(r.request.body)
+            r.raise_for_status()
+
+        remote_vars = self.get_astro_pools(deployment_url, session.get("token"))
+
+        is_migrated = any((True for remote_var in remote_vars if remote_var.get("name", "") == pool_name))
+
+        return self.render_template(
+            "starship/components/migrate_pool_button.html",
+            pool=pool_name,
+            deployment=deployment,
+            is_migrated=is_migrated,
+        )
+
     @expose("/button/migrate/env/<string:deployment>", methods=("POST",))
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_CONFIG)])
     def button_migrate_env(self, deployment: str):
         import os
 
         deployments = self.astro_deployments(session.get("token"))
 
@@ -339,17 +389,17 @@
             }
             for remote_var in deployments[deployment]["deploymentSpec"][
                 "environmentVariables"
             ]
         }
 
         for _, key in (
-            (key, value)
-            for (key, value) in request.form.items()
-            if key != "csrf_token" and key not in remote_vars.keys()
+                (key, value)
+                for (key, value) in request.form.items()
+                if key != "csrf_token" and key not in remote_vars.keys()
         ):
             remote_vars.setdefault(
                 key,
                 {
                     "key": key,
                     "value": os.environ[key],
                     "isSecret": False,
@@ -412,21 +462,21 @@
     @auth.has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_DAG)])
     def dag_cutover_row_get(self, deployment: str, dag_id: str):
         return self.dag_cutover_row(deployment, dag_id)
 
     @expose(
         "/component/row/dags/<string:deployment>/<string:dest>/<string:dag_id>/<string:action>",
         methods=(
-            "GET",
-            "POST",
+                "GET",
+                "POST",
         ),
     )
     @auth.has_access([(permissions.ACTION_CAN_EDIT, permissions.RESOURCE_DAG)])
     def dag_cutover_row(
-        self, deployment: str, dag_id: str, dest: str = "local", action: str = None
+            self, deployment: str, dag_id: str, dest: str = "local", action: str = None
     ):
         if dest not in ["local", "astro"]:
             raise Exception("dest must be 'local' or 'astro'")
 
         dag = self.local_client.get_dags()[dag_id]
         deployment_url = self.get_deployment_url(deployment)
         token = session.get("token")
@@ -478,15 +528,15 @@
             )
             return f"https:/{url.netloc}/{url.path}"
 
 
 v_appbuilder_view = AstroMigration()
 
 v_appbuilder_package = {
-    "name": "Starship 🛸",
+    "name": "Migration Tool 🚀 Starship",
     "category": "Astronomer",
     "view": v_appbuilder_view,
 }
 
 
 class StarshipPlugin(AirflowPlugin):
     name = "starship"
```

### Comparing `astronomer-starship-0.3.3/starship/services/astrohub_client.py` & `astronomer-starship-0.3.4/starship/services/astrohub_client.py`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/services/local_client.py` & `astronomer-starship-0.3.4/starship/services/local_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from airflow.utils.session import provide_session
 from sqlalchemy.orm import Session
 
 
 class LocalAirflowClient:
     @provide_session
     def get_variables_from_metastore(self, session: Session):
@@ -14,14 +16,21 @@
     def get_connections(self, session: Session):
         from airflow.models import Connection
 
         connections = session.query(Connection).order_by(Connection.conn_id).all()
         return connections
 
     @provide_session
+    def get_pools(self, session: Session) -> List['Pool']:
+        from airflow.models import Pool
+
+        pools = session.query(Pool).all()
+        return pools
+
+    @provide_session
     def get_variables(self, session: Session):
         from airflow.models import Variable
 
         vars = session.query(Variable).order_by(Variable.key).all()
         return vars
 
     def get_dags(self):
```

### Comparing `astronomer-starship-0.3.3/starship/static/js/htmx.min.js` & `astronomer-starship-0.3.4/starship/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/static/js/idiomorph.min.js` & `astronomer-starship-0.3.4/starship/static/js/idiomorph.min.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/static/js/popper.js` & `astronomer-starship-0.3.4/starship/static/js/popper.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/static/js/tippy.js` & `astronomer-starship-0.3.4/starship/static/js/tippy.js`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/static/tail-spin.svg` & `astronomer-starship-0.3.4/starship/static/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/components/dag_row.html` & `astronomer-starship-0.3.4/starship/templates/starship/components/dag_row.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/components/migrate_connection_button.html` & `astronomer-starship-0.3.4/starship/templates/starship/components/migrate_connection_button.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/components/tabs.html` & `astronomer-starship-0.3.4/starship/templates/starship/components/tabs.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,25 @@
     <ul class="nav nav-tabs">
         <li class="nav-item {{ 'active' if data.component == 'connections' }}">
             <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_conns') }}">Connections</a>
         </li>
         <li class="nav-item {{ 'active' if data.component == 'variables' }}">
             <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_vars') }}">Variables</a>
         </li>
+        <li class="nav-item {{ 'active' if data.component == 'pools' }}">
+            <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_pools') }}">Pools</a>
+        </li>
 <!--        <li class="nav-item {{ 'active' if data.component == 'env' }}">-->
 <!--            <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_env') }}">Environment Variables</a>-->
 <!--        </li>-->
         <li class="nav-item {{ 'active' if data.component == 'dags' }}">
             <a class="nav-link" hx-get="{{ url_for('AstroMigration.tabs_dags') }}">DAGs cutover</a>
         </li>
     </ul>
 </div>
-<div class="tab-content">
-  <div class="container">
-  {% block body %}
-  <!-- Tab content goes here -->
-  {% endblock %}
-  </div>
+<div class="tab-content" id="tabs-content">
+    <div class="container">
+        {% block body %}
+        <!-- Tab content goes here -->
+        {% endblock %}
+    </div>
 </div>
```

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/components/target_deployment_select.html` & `astronomer-starship-0.3.4/starship/templates/starship/components/target_deployment_select.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
                     <label for="selectedAstroDeployment" class="form-label">Target Deployment</label>
                 </div>
                 <div class="col-lg-6">
                     <select id="selectedAstroDeployment" class="form-control" name="selectedAstroDeployment">
                         <option value="">Select deployment</option>
                         {% if deployments %}
                         {% for deploy in deployments.values() %}
-                        <option value="{{deploy.id}}" {{
-                        'selected' if deploy.id == session.selectedAstroDeployment}}>
-                        {{deploy.label}}</option>
+                        <option value="{{deploy.id}}" {{'selected' if deploy.id == session.selectedAstroDeployment}}>
+                        {{deploy.label}}
+                        </option>
                         {% endfor %}
                         {% endif %}
                     </select>
                 </div>
                 <div class="col-lg-3">
                     <button type="submit" class="btn btn-primary mb3-l">Select</button>
                 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
 Current user
 {{ username }} (Logout)
 Target Deployment
 {% if deployments %} {% for deploy in deployments.values() %}
-{ 'selected' if deploy.id == session.selectedAstroDeployment}}> {
-{deploy.label}}
+{'selected' if deploy.id == session.selectedAstroDeployment}}> {{deploy.label}}
 {% endfor %} {% endif %}
 Select
```

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/components/token_modal.html` & `astronomer-starship-0.3.4/starship/templates/starship/components/token_modal.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/connections.html` & `astronomer-starship-0.3.4/starship/templates/starship/connections.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/dags.html` & `astronomer-starship-0.3.4/starship/templates/starship/dags.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/env.html` & `astronomer-starship-0.3.4/starship/templates/starship/env.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/main.html` & `astronomer-starship-0.3.4/starship/templates/starship/main.html`

 * *Files identical despite different names*

### Comparing `astronomer-starship-0.3.3/starship/templates/starship/variables.html` & `astronomer-starship-0.3.4/starship/templates/starship/variables.html`

 * *Files identical despite different names*

