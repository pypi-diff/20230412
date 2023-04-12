# Comparing `tmp/activetune-0.0.8.tar.gz` & `tmp/activetune-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activetune-0.0.8.tar", last modified: Mon Apr 10 10:54:25 2023, max compression
+gzip compressed data, was "activetune-0.0.9.tar", last modified: Wed Apr 12 13:25:11 2023, max compression
```

## Comparing `activetune-0.0.8.tar` & `activetune-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:54:25.817835 activetune-0.0.8/
--rw-rw-rw-   0        0        0       89 2023-04-10 10:54:25.817835 activetune-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      969 2023-03-24 12:36:44.000000 activetune-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 10:54:25.801507 activetune-0.0.8/activetune/
--rw-rw-rw-   0        0        0       47 2023-04-10 10:53:34.000000 activetune-0.0.8/activetune/__init__.py
--rw-rw-rw-   0        0        0     2783 2023-04-10 10:53:10.000000 activetune-0.0.8/activetune/api.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:54:25.817835 activetune-0.0.8/activetune.egg-info/
--rw-rw-rw-   0        0        0       89 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 12:09:14.000000 activetune-0.0.8/activetune.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-10 10:54:25.000000 activetune-0.0.8/activetune.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 10:54:25.817835 activetune-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      350 2023-04-10 10:53:38.000000 activetune-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:25:11.345137 activetune-0.0.9/
+-rw-rw-rw-   0        0        0       89 2023-04-12 13:25:11.345137 activetune-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2023-03-24 12:36:44.000000 activetune-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 13:25:11.345137 activetune-0.0.9/activetune/
+-rw-rw-rw-   0        0        0       47 2023-04-12 13:22:26.000000 activetune-0.0.9/activetune/__init__.py
+-rw-rw-rw-   0        0        0     2788 2023-04-12 13:22:12.000000 activetune-0.0.9/activetune/api.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:25:11.345137 activetune-0.0.9/activetune.egg-info/
+-rw-rw-rw-   0        0        0       89 2023-04-12 13:25:11.000000 activetune-0.0.9/activetune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-12 13:25:11.000000 activetune-0.0.9/activetune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:25:11.000000 activetune-0.0.9/activetune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-20 12:09:14.000000 activetune-0.0.9/activetune.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-12 13:25:11.000000 activetune-0.0.9/activetune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-12 13:25:11.000000 activetune-0.0.9/activetune.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 13:25:11.345137 activetune-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      350 2023-04-12 13:22:32.000000 activetune-0.0.9/setup.py
```

### Comparing `activetune-0.0.8/README.md` & `activetune-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `activetune-0.0.8/activetune/api.py` & `activetune-0.0.9/activetune/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 "token": self.token,
                 "dataset_id": dataset_id,
                 "input": input,
                 "model_output": model_output,
                 "model_id": model_id,
                 "expected_output": expected_output,
                 "feedback": feedback,
-                "meta": json.dumps(meta),
+                "meta_json": json.dumps(meta),
             },
         ).text[1:-1]
 
     def get_data(self, dataset_id: str):
         return requests.get(
             self.url + "/api/get_data", {"token": self.token, "dataset_id": dataset_id}
         ).json()
```

